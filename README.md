<html>
   <head>
      <title>The jQuery Example</title>
      <script type="text/javascript" src="http://ajax.googleapis.com/ajax/libs/jquery/2.1.3/jquery.min.js"></script>
      
      <script src="myScript.js"></script>
      <link rel="stylesheet" type="text/css" href="style.css">
   </head>
   
   <body>
   
      <p>Click for Specs:</p>
      <span id="result"> </span>
      
      <div id="division">
       <img src="http://www.8-bitcentral.com/images/nintendo/n64/console.jpg" class="picSize">

      </div>
          <div id="ps1" class="picsize">
            <img src="http://2.bp.blogspot.com/-kt7kez1Rkh4/TeTWloblCgI/AAAAAAAAA4E/k7o1jqfYtsA/s1600/ps1+console.png" class="picSize">
         </div>
                <div id="xb360">
                  <img src="http://www.socialshopping.com/images/couponimages/org_1_Bigoutlet-Microsoft-xbox-360-elite-console-120G-XB360-E120GH-.jpg" class="picSize">
               </div>
                      <div id="ps4">
                        <img style="-webkit-user-select: none; cursor: zoom-in;" src="http://static.neuerdings.com/1370949204/ps4_1.jpg" class="picSize">
                     </div>
   </body>
</html>

// css code

 #division
 { margin:10px;
 	padding:12px; 
 	 width:300px;}


.picSize
{
	width:300px;
	height:300px;
}
.border {
	border:1px solid;
}
 // js code
 
 $(document).ready(function() {
            $("#division").click(function () {
               $(this).replaceWith("<li>The Nintendo 64's central processing unit (CPU) is the NEC VR4300</li>");
            });
         });
    $(document).ready(function() {
            $("#ps1").click(function () {
               $(this).replaceWith("<li>The Ps1 CPU: 32-bit RISC (33.9MHz)</li>");
            });
         });
      $(document).ready(function() {
            $("#xb360").click(function () {
               $(this).replaceWith("<li>The xb360 128 VMX-128 registers per hardware thread</li>");
            });
         });
        $(document).ready(function() {
            $("#ps4").click(function () {
               $(this).replaceWith("<li>Ethernet x1, IEEE 802.11b/g/n (2.4 GHz only), Bluetooth 2.1+EDR</li>");
            });
         });
