<template>
  <navbar_buyer />
  <div class="container">
    <div class="row">
      <div class="col-md-12">
        <h1 style="margin-top: 15px">Cart</h1>
      </div>
      <div class="col-md-12">
        <a href="/shippingandpayment"
          ><button type="button" class="btn btn-dark">
            Shipping and payment method
          </button></a
        >
      </div>
    </div>
  </div>
  <footer_app />
</template>

<script>
// @ is an alias to /src
import navbar_buyer from "@/components/navbar_buyer.vue";
import footer_app from "@/components/footer_app.vue";

export default {
  name: "Cart",
  components: {
    navbar_buyer,
    footer_app,
  },
};
</script>
