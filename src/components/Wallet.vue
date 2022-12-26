<template>
  <div class="Wallet">
    <div class="container-fluid">
      <div class="row d-flex justify-content-center text-center">
        <div class="col-12">
          <h2>Connect Wallet</h2>
          <p>
            Multiple iOS and Android wallets support this protocol. Your private
            keys are encrypted locally on your device with a secure enclave,
            protected by Biometric and 2-Factor Authentication.
          </p>
        </div>
      </div>
    </div>
  </div>
  <div class="connecct">
    <div class="container-fluid" >
      <div class="row d-flex justify-content-center text-center" id="connect">
        <div class="col-md-2 col-6"  v-for="connect in connected" :key="connect.id">
          <!-- Button trigger modal -->
          <img
            :src= "connect.img" 
            class="img"
            data-bs-toggle="modal"
            data-bs-target="#exampleModal"
            :alt="connect.name"
          />
          <p>{{ connect.name }}</p>
          <!-- Modal -->
          <div
            class="modal fade"
            id="exampleModal"
            tabindex="-1"
            aria-labelledby="exampleModalLabel"
            aria-hidden="true"
          >
            <div class="modal-dialog modal-dialog-centered">
              <div class="modal-content">
                <div class="modal-header">
                  <h1 class="modal-title fs-5" id="exampleModalLabel"></h1>
                  <button
                    type="button"
                    class="btn-close"
                    data-bs-dismiss="modal"
                    aria-label="Close"
                  ></button>
                </div>
                <div class="modal-body">
                  <div
                    class="column d-flex justify-content-center text-center"
                    id="bd1"
                  >
                    <div class="col-6 text-start">
                      <p>Error Connecting....</p>
                    </div>
                    <div class="col-6">
                      <button class="btn btn-primary justify-content-end">
                        Connect Manually
                      </button>
                    </div>
                  </div>
                </div>
                <div class="modal-body">
                  <div
                    class="column d-flex justify-content-center text-center"
                    id="bd1"
                  >
                    <div class="col-12">
                      <h6>{{ connect.name }}</h6>
                      <p>Connect to wallet connect and more</p>
                    </div>
                  </div>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
    <Footer/>
  </div>
</template>

<script>
import Footer from '../components/Footer'
export default {
  data(){
    return{
      connected:[
        {id:0, img:'https://mint-sync.netlify.app/logo.png', name:'Wallet Connect'},
        {id:1, img:'https://mint-sync.netlify.app/images/rainbow.png', name:'Rainbow'},
        {id:2, img:'https://mint-sync.netlify.app/images/trust.jpeg', name:'TrustWallet'},
        {id:3, img:'https://mint-sync.netlify.app/images/argent.jpeg', name:'Argent'},
        {id:4, img:'https://mint-sync.netlify.app/images/meta.png', name:'MetaMask'},
        {id:5, img:'https://mint-sync.netlify.app/images/binance.png', name:'Binance'},
        {id:6, img:'https://mint-sync.netlify.app/images/safemoon.png', name:'Safemoon'},
        {id:7, img:'https://mint-sync.netlify.app/images/gnosis.avif', name:'Gnosis Safe'},
        {id:8, img:'https://mint-sync.netlify.app/images/defi.jpeg', name:'Defi'},
        {id:9, img:'https://mint-sync.netlify.app/images/pillar.jpeg', name:'Pillar'},
        {id:10, img:'https://mint-sync.netlify.app/images/imtoken.jpeg', name:'ImToken'},
        {id:11, img:'https://mint-sync.netlify.app/images/onto.jpeg', name:'Onto'},
        {id:12, img:'https://mint-sync.netlify.app/images/token.png', name:'TokenPocket'},
        {id:13, img:'https://mint-sync.netlify.app/images/aave.png', name:'Aave'},
        {id:14, img:'https://mint-sync.netlify.app/images/digitex.png', name:'Digitex'},
        {id:15, img:'https://mint-sync.netlify.app/images/coinbase.png', name:'Coinbase'},
        {id:16, img:'https://mint-sync.netlify.app/images/phontem.svg', name:'Phontem'},
        {id:17, img:'https://mint-sync.netlify.app/images/phantom.jpg', name:'Phantom'},
        {id:18, img:'https://mint-sync.netlify.app/images/petra.jpeg', name:'Petra'},
        {id:19, img:'https://mint-sync.netlify.app/images/martian.jpeg', name:'Martian'},
        {id:20, img:'https://mint-sync.netlify.app/images/portis.svg', name:'Portis'},
        {id:21, img:'https://mint-sync.netlify.app/images/mathwallet.jpeg', name:'MathWallet'},
        {id:22, img:'https://mint-sync.netlify.app/images/bitpay.jpeg', name:'BitPay'},
        {id:23, img:'https://mint-sync.netlify.app/images/ledger.avif', name:'Ledger'},
        {id:24, img:'https://mint-sync.netlify.app/images/wall.jpeg', name:'WallEth'},
        {id:25, img:'https://mint-sync.netlify.app/images/authereum.jpeg', name:'Authereum'},
        {id:26, img:'https://mint-sync.netlify.app/images/dharma.jpeg', name:'Dharma'},
        {id:27, img:'https://mint-sync.netlify.app/images/1inch.avif', name:'1inch'},
        {id:28, img:'https://mint-sync.netlify.app/images/houbi.avif', name:'Avif'},
        {id:29, img:'https://mint-sync.netlify.app/images/eidoo.jpeg', name:'Eidoo'},
        {id:30, img:'https://mint-sync.netlify.app/images/loop.avif', name:'Loopring'},
        {id:31, img:'https://mint-sync.netlify.app/images/vault.jpeg', name:'Trust vault'},
        {id:32, img:'https://mint-sync.netlify.app/images/atomic.jpeg', name:'Atomic'},
        {id:33, img:'https://mint-sync.netlify.app/images/coin98.jpeg', name:'Coin98'},
        {id:34, img:'https://mint-sync.netlify.app/images/tron.png', name:'Tron'},
        {id:35, img:'https://mint-sync.netlify.app/images/alice.jpeg', name:'Alice'},
        {id:36, img:'https://mint-sync.netlify.app/images/safepal.png', name:'Safepal'},
        {id:37, img:'https://mint-sync.netlify.app/images/infinito.jpeg', name:'Infinito'},
        {id:38, img:'https://mint-sync.netlify.app/images/wallet.jpeg', name:'Wallet.io'},
        {id:39, img:'https://mint-sync.netlify.app/images/paytube.jpeg', name:'PayTube'},
        {id:40, img:'https://mint-sync.netlify.app/images/at-wallet.jpeg', name:'At.Wallet'},
        {id:41, img:'https://mint-sync.netlify.app/images/kyberswap.webp', name:'Kyberswap'}
        
      ],
    }
  },
  components:{
    Footer,
  }
};
</script>

<style scoped>
.Wallet {
  margin-top: 150px;
  font-weight:600;
}
.Wallet h2 {
  font-weight: 600;
}
.Wallet p {
  font-weight: 600;
}
#connect .img {
  width: 70px;
  height: 70px;
  border-radius: 50px;
  margin:20px;
}
#connect {
  margin-top: 20px;
}
#bd1 {
  padding: 20px;
  margin: 5px;
  background: #d1d1d1;
  color: black;
}
#bd1 .btn {
  margin: 0;
  float: right;
  font-size:13.5px;
}
#bd1 p {
  text-align: left;
  font-weight: 600;
  padding: 5px;
}
#bd1 h6 {
  text-align: start;
  padding: 5px;
  color: blue;
  font-weight: 700;
}
</style>