# VerificationCode
验证码

servlet,controller
	Gcode gcode  = new Gcode();
	
        String txt = gcode.outputVerifyImage(125, 60, 4, response);

web
	<img id="img" src="IndexServlet" onclick="change()"></img>
	<script type="text/javascript">
		function change(){
			document.getElementById("img").src="IndexServlet?"+Math.random();
		}
		
