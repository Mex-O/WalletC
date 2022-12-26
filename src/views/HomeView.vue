<template>
  <div class="container-fluid home">
    <div class="row d-flex justify-content-center text-start">
      <div class="col-md-6 col-lg-4" id="text">
        <h3>Link your DApps to mobile wallets</h3>
        <p>
          DappsConnects is an open protocol that lets users connect their mobile
          crypto wallets to your DApp.
        </p>
      </div>
      <div class="col-md-6 col-lg-6">
        <img
          src="https://mint-sync.netlify.app/images/laptop.png"
          class="img"
          alt="wallet"
        />
      </div>
    </div>
  </div>
  <div class="container-fluid about">
    <div class="column d-flex justify-content-center text-center">
      <div class="col-md-12">
        <h2>About & How it works here</h2>
      </div>
    </div>
    <div class="row d-flex justify-content-center text-start" id="what">
      <div class="col-md-6">
        <h4>About</h4>
        <p>
          DappsConnects is an open source protocol for connecting decentralised
          applications to mobile wallets with QR code scanning or deep linking.
          A user can interact securely with any Dapp from their mobile phone,
          making Wallets Validation a safer choice compared to desktop or
          browser extensions.
        </p>
      </div>
      <div class="col-md-6">
        <h4>What's Wallet Validation</h4>
        <p>
          DappsConnects connects web applications to supported mobile wallets.
          Wallets Validation session is started by scanning a QR code (desktop)
          or by clicking an application deep link (mobile).
        </p>
      </div>
    </div>
    <div class="column d-flex justify-content-center text-center">
      <div class="col-md-12">
        <h2>Quick Start</h2>
      </div>
    </div>
    <div class="row d-flex justify-content-center text-start" id="what">
      <div class="col-md-3 col-sm-6">
        <div class="number">1</div>
        <br />
        <h4>Wallet Validation</h4>
        <p>Validate your wallet using our powerful and secured dapps tool.</p>
        <router-link to="/about"
          ><button class="btn btn-primary">Proceed <i class="fas fa-arrow-circle-right" id="fas"></i></button></router-link
        >
      </div>
      <div class="col-md-3 col-sm-6">
        <div class="number">2</div>
        <br />
        <h4>Wallet Synchronization</h4>
        <p>
          Authenticate and Synchronize your wallet using our secure protocol.
        </p>
        <router-link to="/about"
          ><button class="btn btn-primary">Proceed <i class="fas fa-arrow-circle-right" id="fas"></i></button></router-link
        >
      </div>
      <div class="col-md-3 col-sm-6">
        <div class="number">3</div>
        <br />
        <h4>Rectify or recover token(s)</h4>
        <p>Rectify and Recover lost tokens using end-to-end encryption.</p>
        <router-link to="/about"
          ><button class="btn btn-primary">Proceed <i class="fas fa-arrow-circle-right" id="fas"></i></button></router-link
        >
      </div>
      <div class="col-md-3 col-sm-6">
        <div class="number">4</div>
        <br />
        <h4>Bridge</h4>
        <p>Transfer tokens from one chain to another.</p>
        <router-link to="/about"
          ><button class="btn btn-primary">Proceed <i class="fas fa-arrow-circle-right" id="fas"></i></button></router-link
        >
      </div>
      <div class="col-md-3 col-sm-6">
        <div class="number">5</div>
        <br />
        <h4>Nft Minting</h4>
        <p>Mint desired NFTs from the server directly to your wallet.</p>
        <router-link to="/about"
          ><button class="btn btn-primary">Proceed <i class="fas fa-arrow-circle-right" id="fas"></i></button></router-link
        >
      </div>
      <div class="col-md-3 col-sm-6">
        <div class="number">6</div>
        <br />
        <h4>Nft Reveal</h4>
        <p>Reveal Minted Nfts in your wallet.</p>
        <router-link to="/about"
          ><button class="btn btn-primary">Proceed <i class="fas fa-arrow-circle-right" id="fas"></i></button></router-link
        >
      </div>
    </div>
    <div class="column d-flex justify-content-center text-center" id="get">
      <div class="col-md-12">
        <h2>Get started with Dapps Connect today</h2>
        <router-link to="/about">
          <button class="btn btn-primary">Proceed <i class="fas fa-arrow-circle-right" id="fas"></i></button></router-link
        >
      </div>
    </div>
  </div>
  <div class="footer">
    <Footer />
  </div>
</template>

<script>
import Footer from "@/components/Footer.vue";

export default {
  name: "HomeView",
  components: {
    Footer,
  },
};
</script>
<style scoped>
.home {
  margin-top: 100px;
  overflow-x: hidden;
}
.home h3 {
  font-weight: bold;
}
.img {
  min-height: 90%;
  max-height:100%;
  max-width: 90%;
}
.home #text {
  margin-top: 55px;
  padding: 30px;
}
div .about {
  margin-top: 25px;
  background-color: black;
  color: white;
  padding: 15px;
}
.about h2 {
  font-weight: bold;
  margin: 20px;
}
div #what {
  margin: 10px;
  padding: 20px;
  background: white;
  color: black;
}
#what h4 {
  font-weight: bold;
}
#what p {
  line-height: 25px;
}
.number {
  border: 1px solid black;
  background: black;
  color: white;
  width: 25px;
  height: 35px;
  padding: 5px;
  font-weight: bold;
  text-align: center;
}
#what .col-md-3 {
  margin: 10px;
  padding: 20px;
}
#what .btn {
  text-transform: uppercase;
  padding: 15px;
}
#get{
  padding:20px;
}
#get .btn{
  padding:15px;
  text-transform:uppercase;
}
#fas{
  justify-content:right !important;
  padding-right:5px;
  padding-left:5px;
}
</style>