<template>
 <div>
     <div class="bgtinit"></div>
     <section class="bussinesscard `p-3">
     		<div class="flip">
     			<div class="front">
     				<div class="top">
                        <div class="logo">
                            Dexter
                        </div>
     				</div>
     				<div class="nametroduction">
     					<div class="name">Signin</div>
     					<div class="introduction">A career is born in public-talent in privacy.</div>
     				</div>
     				<div class="contact">
     					 <div class="website mt-4">
     						 <i class="fa fa-user-secret icon"></i>
     					          <a  data-toggle="modal" href="#Model-1">Teacher
                                </a>
     					</div>
     					<div class="twitter mt-4">
                            <i class="fa fa-users icon"></i>
     						<a data-toggle="modal" href="#Model-1">Parent</a>
     					</div>
     					<div class="phone mt-4">
     						<i class="fa fa-mortar-board icon"></i>
     						<a data-toggle="modal" href="#Model-1">Student</a>
     					</div>
     				</div>
     			</div>
     			<div class="back">
                </div>
     		</div>
     	</section>
     	<section class="tooltip">
     	</section>
        <!-- <Modal-1> -->
        <div class="modal fade w3-animate-zoom" id="Model-1" tabindex="-1" role="dialog" aria-labelledby="exampleModalCenterTitle" aria-hidden="true">
  <div class="modal-dialog modal-dialog-centered" role="document">
    <div class="modal-content">
      <div class="modal-header">
          <h5 class="modal-title" id="exampleModalLongTitle">
              <h4 style="color:black;">
                        <span class="glyphicon glyphicon-lock">
                        </span>
                        Login
                    </h4>
                </h5>
        <button type="button" class="close" data-dismiss="modal" aria-label="Close">
          <span aria-hidden="true">&times;</span>
        </button>
      </div>
      <div class="modal-body">
          <form role="form">
            <div class="form-group">
              <label for="usrname">
                  <span class="glyphicon glyphicon-user">
                  </span>
                   Username
               </label>
              <input type="text" class="form-control" id="usrname" placeholder="Enter email" required>
            </div>
            <div class="form-group">
              <label for="psw">
                  Password
              </label>
              <input type="text" class="form-control" id="psw" placeholder="Enter password" required>
            </div>
            <div class="checkbox">
              <label>
                  <input type="checkbox" value="" checked>
                  Remember me
              </label>
            </div>
            <div class="d-flex justify-content-center ">
            <button type="submit" class="btn ">
                 Login
             </button>
         </div>
          </form>
      </div>
      <div class="modal-footer">
          <h5>New User?<i class="fa fa-hand-o-right icon"></i></h5>
        <!-- <button type="button" class="btn btn-secondary" data-toggle="modal" data-target="#Model-3" data-dismiss="modal">Prev</button> -->
        <button type="button" class="btn nextbtn" data-toggle="modal" data-target="#Model-2"data-dismiss="modal" >Next</button>
      </div>
    </div>
  </div>
</div>

<!-- Model-2 -->
<div class="modal fade w3-animate-zoom" data-validation="true" data-validation-event="submit" id="Model-2" tabindex="-1" role="dialog" aria-labelledby="exampleModalCenterTitle" aria-hidden="true" >
    <div class="modal-dialog modal-dialog-centered" role="document">
      <div class="modal-content">
        <div class="modal-header">
            <h5 class="modal-title" id="exampleModalLongTitle">
                <h4>
                         Register
                      </h4>
                  </h5>
          <button type="button" class="close" data-dismiss="modal" aria-label="Close">
            <span aria-hidden="true">&times;</span>
          </button>
        </div>
        <div class="modal-body m-body">
            <form role="form">
              <div class="form-group">
                <label for="name">
                     Name
                 </label>
                <input type="text" class="form-control" id="name" placeholder="Name" required>
              </div>
              <div class="form-group">
                <label for="email">
                     Email
                 </label>
                <input type="text" class="form-control" id="email" placeholder="Email" required>
              </div>
              <div class="form-group">
                <label for="Phone number">
                    Phone number
                 </label>
                <input type="text" class="form-control" id="mobno" placeholder="Phone number" required>
              </div>
              <div class="form-group ">
                  <div class="radio gender">
                      <label for="gender" class="title">Gender:</label>
                      <label class="radio-inline">
                          <input type="radio" name="inlineRadioOptions"  value="Male" class="option-input userGender" checked>
                          <span>Male</span>
                      </label>
               <label class="radio-inline">
             <input type="radio" name="inlineRadioOptions" value="Female" class="option-input userGender">
             <span>Female</span>
           </label>
         </div>
          </div>
         <div class="form-group">
                <label for="psw">
                    Password
                </label>
                <input type="text" class="form-control" id="pwd" >
            </div>
            <div class="form-group">
                   <label for="psw">
                      Confirm Password
                   </label>
                   <input type="password" class="form-control" id="cpwd" >
               </div>
<div class="form-group">
    <div>
    <label for="date">DOB</label>
     <datepicker placeholder="Select Date"></datepicker>
</div>
</div>
  <button type="submit" class="btn btn-default btn-block" @click="validate">
                  Register
               </button>
            </form>
        </div>
        <div class="modal-footer">
          <button type="button" class="btn btn-secondary" data-toggle="modal" data-target="#Model-1" data-dismiss="modal">Prev</button>
          <button type="button" class="btn nextbtn" data-toggle="modal" data-target="#Model-3"data-dismiss="modal" >Next</button>
        </div>
      </div>

    </div>
</div>
<!-- <Modal-3> -->
<div class="modal fade w3-animate-zoom" data-validation="true" data-validation-event="submit" id="Model-3" tabindex="-1" role="dialog" aria-labelledby="exampleModalCenterTitle" aria-hidden="true" >
    <div class="modal-dialog modal-dialog-centered" role="document">
      <div class="modal-content">
        <div class="modal-header">
            <h5 class="modal-title" id="exampleModalLongTitle">
                <h4>
                     OTP Verification
                      </h4>
                  </h5>
          <button type="button" class="close" data-dismiss="modal" aria-label="Close">
            <span aria-hidden="true">&times;</span>
          </button>
        </div>
        <div class="modal-body">
              <div class="">
                  <h3><b>Code</b></h3>
              <input type="text" placeholder="">
          </div>
          <button type="button" class="buttony" @click="btnclick" id="myButton1">Send</button>
                  <progress-button name="fillColor" class="bn btn-success mr-1 mb-1 mt-2" fill-color="#FF0000" @click="verify('verified')">
                     Verify
                  </progress-button>
              </h3>
        </div>
        <div class="modal-footer">
          <button type="button" class="btn btn-secondary" data-toggle="modal" data-target="#Model-2" data-dismiss="modal">Prev</button>
          <button type="button" class="btn nextbtn" data-toggle="modal" data-target="#Model-1"data-dismiss="modal" >Next</button>
        </div>
      </div>

    </div>
</div>
    </div>
</template>

<script>
$('.container').on('click', function () {
  $('.card').toggleClass('flipped');
});
$(document).ready(function() {
  $('.button').on('click', function() {
    var $this = $(this);
    var loadingText = '<i class="fa fa-circle-o-notch fa-spin"></i> loading...';
    if ($(this).html() !== loadingText) {
      $this.data('original-text', $(this).html());
      $this.html(loadingText);
    }
    setTimeout(function() {
      $this.html($this.data('original-text'));
    }, 2000);
  });
})
function validate() {
       var validator = $("#Modal-2").validate({
           rules: {
               password: "required",
               confirmpassword: {
                   equalTo: "#password"
               }
           },
           messages: {
               password: " Enter Password",
               confirmpassword: " Enter Confirm Password Same as Password"
           }
       });
       if (validator.form()) {
           alert('Success');
       }
   }
import Button from 'vue-progress-button';
import Datepicker from 'vuejs-datepicker';
export default {
  components: {
    'progress-button': Button,
    Datepicker
},
methods:{
 btnclick()
    {
        $('#myButton1').text("resend")
    }

}
}

</script>
<style>

body,html{
  font-family: 'Comic Sans MS', sans-serif;
  background: url(https://wallpaper-house.com/data/out/8/wallpaper2you_230549.jpg);
  -webkit-background-size: cover;
  -moz-background-size: cover;
  background-size: cover;
  margin: 0;
  padding: 0;
  width: 100%;
  height: 100%;
  overflow: hidden;
  z-index: 9;
}
.bgtint {
  position: absolute;
  height: 100%;
 width: 100%;
  background: rgba(42, 43, 57, 0.7);
}
p {
  padding: 0;
  margin: 0;
  display: inline-block;
}
a {
  color: #315356;
  text-decoration: none;
  -moz-transition: all 0.2s ease-in-out;
  -o-transition: all 0.2s ease-in-out;
  -webkit-transition: all 0.2s ease-in-out;
  transition: all 0.2s ease-in-out;
}
a:hover {
  color:#000000;
}

.bussinesscard {
  height: 350px;
  width: 450px;
  overflow: hidden;
  box-shadow: 0px 0px 53px -20px black;
  position: relative;
  margin-top: 300px;
  left: 50%;
  top: 50%;
  -moz-transform: translate(-50%, -50%);
  -ms-transform: translate(-50%, -50%);
  -webkit-transform: translate(-50%, -50%);
  transform: translate(-50%, -50%);
}
.bussinesscard .flip {
  -moz-transition: all 0.5s ease;
  -o-transition: all 0.5s ease;
  -webkit-transition: all 0.5s ease;
  transition: all 0.5s ease;
}
.bussinesscard .front {
  z-index: 11;
  width: 100%;
  position: absolute;
  height: 100%;
  background: transprant;
  box-shadow: 0px 0px 33px -1px rgba(0, 0, 0, 0.45);
  -moz-transform: scale(1, 1);
  -ms-transform: scale(1, 1);
  -webkit-transform: scale(1, 1);
  transform: scale(1, 1);
  -moz-transition: all 0.6s ease;
  -o-transition: all 0.6s ease;
  -webkit-transition: all 0.6s ease;
  transition: all 0.6s ease;
}
.bussinesscard .front .top {
  height: 50%;
  background: #2a2b39;

}
.bussinesscard .front .top:after {
  position: absolute;
  content: '';
  pointer-events: none;
}
.bussinesscard .front .top:after {
  left: 50%;
  width: 2em;
  height: 2em;
  -moz-transform: translateX(-50%) rotate(45deg);
  -ms-transform: translateX(-50%) rotate(45deg);
  -webkit-transform: translateX(-50%) rotate(45deg);
  transform: translateX(-50%) rotate(45deg);
  bottom: 9em;
  z-index: 10;
  background: inherit;
}
.bussinesscard .front .top .logo {
  display: inline-block;
  background: #6acd79;
  color: #fff;
  z-index: 11;
  padding: .16em;
  border: 8px solid #fff;
  position: relative;
  pointer-events: none;
  -moz-transform: translateX(-50%);
  -ms-transform: translateX(-50%);
  -webkit-transform: translateX(-50%);
  transform: translateX(-50%);
  left: 50%;
  margin-top: .4em;
  font-size: 4em;
}
.bussinesscard .front .top .logo .fat {
  font-weight: 800;
}
.bussinesscard .front .top .logo .skinny {
  font-weight: 100;
}
.bussinesscard .front .nametroduction {
  margin-top: 2.4em;
  -moz-transform: translateY(0);
  -ms-transform: translateY(0);
  -webkit-transform: translateY(0);
  transform: translateY(0);
  z-index: 8;
}
.bussinesscard .front .name {
  color: #2a2b39;
  font-weight: 400;
  font-size: 3.2em;
  text-align: center;
  position: relative;
  margin-bottom: .35em;
}
.bussinesscard .front .name:after {
  content: '';
  position: absolute;
  top: 1.3em;
  width: 20%;
  left: 40%;
  right: 40%;
  height: 1px;
  background: #2a2b39;
}
.bussinesscard .front .introduction {
  text-align: center;
  color: #2a2b39;
  font-family: 'Old Standard TT', serif;
  font-style: italic;
}
.bussinesscard .front .contact {
  color: #2a2b39;
  margin-left:4em;
  font-weight: 300;
  font-size:2.3em;
  -moz-transform: translateY(400%);
  -ms-transform: translateY(400%);
  -webkit-transform: translateY(400%);
  transform: translateY(400%);
}
.bussinesscard .front .contact span {
  color: #2D3244;
  font-size: 1.7em;
  width: 1.3em;
  display: inline-block;
}
.bussinesscard .front .contact a {
  position: relative;
  bottom: .24em;
}
.bussinesscard .back {
  width: 100%;
  height: 100%;
  background: #fff;
  backface-visibility: hidden;
  position: absolute;
}

.tooltip {
  position: absolute;
  left: 1em;
  bottom: 1em;
  color: #fff;
  font-weight: 300;
  padding: .4em;
  background: #6acd79;
}

/* HOVER ANIMATIONS */
.front .top .logo, .front .top, .front .top:after, .front .nametroduction, .front .contact {
  -moz-transition: all 0.7s ease-in-out;
  -o-transition: all 0.7s ease-in-out;
  -webkit-transition: all 0.7s ease-in-out;
  transition: all 0.7s ease-in-out;
}

.flip:hover .front .top .logo {
  margin-top: .28em;
  font-size: 1.3em;
  border: 3px solid #fff;
  margin-left: .15em;
  -moz-transform: translateX(0);
  -ms-transform: translateX(0);
  -webkit-transform: translateX(0);
  transform: translateX(0);
  left: 0;
}

.flip:hover .front .top {
  height: 15%;
}
.flip:hover .front .top:after {
  width: 1.5em;
  height: 1.5em;
  bottom: 16.3em;
}

.flip:hover .front .nametroduction {
  -moz-transform: translateY(400%);
  -ms-transform: translateY(400%);
  -webkit-transform: translateY(400%);
  transform: translateY(400%);
}

.flip:hover .front .contact {
  -moz-transform: translateY(-52%);
  -ms-transform: translateY(-52%);
  -webkit-transform: translateY(-52%);
  transform: translateY(-52%);
}

</style>
