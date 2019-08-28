# parent-frame
Envio de datos de padre a iframe


<h1>Receiver Window</h1>
	<p>
		This document is on the domain: http://demos.matt-west.commmmmm
	</p>
	<div id="message">ffgrg</div>
  <script type="text/javascript">
	
  window.onload = function() {
	


	var messageEle = document.getElementById('message');

	
	function receiveMessage(e) {
		
		messageEle.innerHTML = "Message Received: " + e.data;
		console.log(e.data);
	}

	
	window.addEventListener('message', receiveMessage);
}
</script>
