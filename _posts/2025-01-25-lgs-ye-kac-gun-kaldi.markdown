---
layout: default
title: "LGS’ye Kaç Gün Kaldı?"
date: 2025-01-25 00:00:00 +0000
---

# LGS’ye Kaç Gün Kaldı?
### LGS Tarihi: 15 Haziran 2025
  
<p id="countdown" style="text-align: center; font-size: 60px; margin-top: 0px;"></p>

<script>
// Set the date we're counting down to
var countDownDate = new Date("2025/06/15 09:30:00").getTime();

// Update the count down every 1 second
var x = setInterval(function() {

  // Get today's date and time
  var now = new Date().getTime();
    
  // Find the distance between now and the count down date
  var distance = countDownDate - now;
    
  // Time calculations for days, hours, minutes and seconds
  var days = Math.floor(distance / (1000 * 60 * 60 * 24));
  var hours = Math.floor((distance % (1000 * 60 * 60 * 24)) / (1000 * 60 * 60));
  var minutes = Math.floor((distance % (1000 * 60 * 60)) / (1000 * 60));
  var seconds = Math.floor((distance % (1000 * 60)) / 1000);
    
  // Output the result in an element with id="countdown"
  document.getElementById("countdown").innerHTML = days + " Gün | " + hours + " Saat | "
  + minutes + " Dakika | " + seconds + " Saniye ";
    
  // If the count down is over, write some text 
  if (distance < 0) {
    clearInterval(x);
    document.getElementById("demo").innerHTML = "EXPIRED";
  }
}, 1000);
</script>