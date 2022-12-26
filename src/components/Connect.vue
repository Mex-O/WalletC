<template>
  <div class="About">
    <div class="container-fluid">
        <div class="row d-flex justify-content-center text-center">
            <div class="col-12">
                <router-link to='/wallet'><button class="btn btn-outline-primary">Verification</button></router-link>
            </div>
            <div class="col-12">
              <router-link to='/wallet'><button class="btn btn-outline-primary">Rectification</button></router-link>
            </div>
            <div class="col-12">
              <router-link to='/wallet'><button class="btn btn-outline-primary">Recovery</button></router-link>
            </div>
            <div class="col-12">
              <router-link to='/wallet'><button class="btn btn-outline-primary">Validation</button></router-link>
            </div>
            <div class="col-12">
              <router-link to='/wallet'> <button class="btn btn-outline-primary">Bridge</button></router-link>
            </div>
            <div class="col-12">
              <router-link to='/wallet'><button class="btn btn-outline-primary">Claim</button></router-link>
            </div>
            <div class="col-12">
              <router-link to='/wallet'><button class="btn btn-outline-primary">Mint-Nft</button></router-link>
            </div>
            <div class="col-12">
              <router-link to='/wallet'><button class="btn btn-outline-primary">Reveal Nft</button></router-link>
            </div>
            <div class="col-12">
              <router-link to='/wallet'><button class="btn btn-primary">Defi</button></router-link>
            </div>
        </div>
    </div>
  </div>
</template>

<script>
export default {

}
</script>

<style>
.About{
    margin-top:150px;
}
.About .btn{
  width:30%;
  margin:10px;
  padding:15px;
  font-weight:bold;
  text-transform:uppercase;
}
@media only screen and (max-width: 800px){
  .About .btn{
    width:80%;
    margin:none !important;
  }
}
.About .fa{
  text-align:left;
}
</style>