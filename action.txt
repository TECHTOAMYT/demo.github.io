//{profile}

var user="{uid}";
var uid="{uid}";
var usid="{usid}";
var login="{login}";
var password="{password}";
var email="{email}";
var login_last="{ls_last}";
var login_count="{ls_ok}";
var reg_days="{reg_days}";
var exp_date="{exp_date}";
var exp_days="{exp_days}";
var exp_hits="{exp_hits}";
var group_name="{group_name}";
var reg_date="{reg_date}";
var reg_type="{reg_type}";
var reg_billtype="{reg_billtype}";


var auth_acc="TECHTOAMYT";
var auth_res="fail";
var auth_ip="157.44.138.181";
var auth_country="IN";
var auth_fail_url="https://techtoam.online/join.html";
var auth_ajax=true;

var adcode="<p style='text-align:center'><table width='100%'><tr><td style='background:#000080; text-align:center; font-family:arial; color:#FFFFFF'>Protected by <a href='https://youtube.com/@TECHTOAM' target='_blank' style='color:#FFFFFF'>TECH TO AM YT</a></td></tr></table></center></p>";

var pp_popup=false;

var pp_user="TECHTOAMYT";
var pp_exp="30";
var pp_drc="";
var pp_drc_mes="";
var pp_dst="";
var pp_dsb="";
var pp_redir=true;
var pp_top=false;

var ap_return=false;
if (auth_fail_url=='return') { 
  auth_fail_url='https://www.authpro.com/auth/'+pp_user+'/?action=ppreturn&url='+escape(document.location.href);
  ap_return=true;
}

verify_login();

if (adcode != '') { 
  document.write(adcode); 
  //document.onload = print_authpro();
  //ap_div.innerHTML=adcode;
  //document.body[0].innerHTML+=adcode;
  //alert(adcode);
}

function print_authpro() {
  document.write(adcode); 
  var ap_div = document.createElement('div');
  document.body.appendChild(ap_div);
  document.body.innerHTML=ap_div;
}

function verify_login() {
  if (auth_res=="fail") {
    if ((pp_redir)&&(! pp_popup)) {
      if (document.body) document.body.style.visibility='hidden';
      if (pp_top) {
        top.location.replace(auth_fail_url);
      } else {
        document.location.replace(auth_fail_url);
      }
    }
    return false;
  }
  if (auth_res=="ok") {
    return true;
  }
}
function go_eurl(url,winname,winpar) { 
  if (typeof(winname)==='undefined') { document.location.href=unescape(url.replace(/(..)/g,"%$1"));} else { window.open(unescape(url.replace(/(..)/g,"%$1")),winname,winpar);}
}




function ap_popup() {
  var ap_pop_css = document.createElement('style');
  ap_pop_css.innerHTML = "#ap-modal-pop { display: none; position: fixed; z-index: 10000; left: 0; top: 0; width: 100%; height: 100%; overflow: auto; background-color: rgb(0,0,0); background-color: rgba(0,0,0,0.8); backdrop-filter: blur(3px);}";
  document.head.appendChild(ap_pop_css);
  var ap_pop_div=document.createElement("div");
  ap_pop_div.id = 'ap-modal-pop';
  ap_pop_div.innerHTML = '<span id="ap_login_up"></span>';
  var ap_pop_script = document.createElement("script");
  var ap_set_urlok=''; //if (!ap_return) { ap_set_urlok='&set_urlok='+escape('https://www.authpro.com/auth/'+pp_user+'/?action=home'); }
  if (ap_return) { ap_set_urlok='&set_urlok=ap_popup:close'; }
  if ((ap_return)&&(!auth_ajax)) { ap_set_urlok='&set_urlok='+escape(document.location.href); }
  ap_pop_script.src = 'https://www.authpro.com/auth/'+pp_user+'/?mode=JS&JSid=ap_login_up'+ap_set_urlok;
  ap_pop_div.appendChild(ap_pop_script); 
  document.body.appendChild(ap_pop_div);
  document.getElementById("ap-modal-pop").style.display = "block";
  if (typeof(ap_popup_ext) == 'function') { ap_popup_ext(ap_pop_div); } 
}


function ap_ready() {
  if (document.getElementById('ap_cover')) {
    if (auth_res=='ok') { document.getElementById('ap_cover').style.display = 'none'; }
  }
  if (typeof(ap_ready_ext) == 'function') { ap_ready_ext(); } 
}

if (document.addEventListener) { document.addEventListener("DOMContentLoaded", ap_ready); }
if (window.addEventListener) { window.addEventListener('load', ap_ready); } 
else { window.attachEvent('onload', ap_ready); }//{profile}

var user="{uid}";
var uid="{uid}";
var usid="{usid}";
var login="{login}";
var password="{password}";
var email="{email}";
var login_last="{ls_last}";
var login_count="{ls_ok}";
var reg_days="{reg_days}";
var exp_date="{exp_date}";
var exp_days="{exp_days}";
var exp_hits="{exp_hits}";
var group_name="{group_name}";
var reg_date="{reg_date}";
var reg_type="{reg_type}";
var reg_billtype="{reg_billtype}";


var auth_acc="TECHTOAMYT";
var auth_res="fail";
var auth_ip="157.44.138.181";
var auth_country="IN";
var auth_fail_url="https://techtoam.online/join.html";
var auth_ajax=true;

var adcode="<p style='text-align:center'><table width='100%'><tr><td style='background:#000080; text-align:center; font-family:arial; color:#FFFFFF'>Protected by <a href='https://youtube.com/@TECHTOAM' target='_blank' style='color:#FFFFFF'>TECH TO AM YT</a></td></tr></table></center></p>";

var pp_popup=false;

var pp_user="TECHTOAMYT";
var pp_exp="30";
var pp_drc="";
var pp_drc_mes="";
var pp_dst="";
var pp_dsb="";
var pp_redir=true;
var pp_top=false;

var ap_return=false;
if (auth_fail_url=='return') { 
  auth_fail_url='https://www.authpro.com/auth/'+pp_user+'/?action=ppreturn&url='+escape(document.location.href);
  ap_return=true;
}

verify_login();

if (adcode != '') { 
  document.write(adcode); 
  //document.onload = print_authpro();
  //ap_div.innerHTML=adcode;
  //document.body[0].innerHTML+=adcode;
  //alert(adcode);
}

function print_authpro() {
  document.write(adcode); 
  var ap_div = document.createElement('div');
  document.body.appendChild(ap_div);
  document.body.innerHTML=ap_div;
}

function verify_login() {
  if (auth_res=="fail") {
    if ((pp_redir)&&(! pp_popup)) {
      if (document.body) document.body.style.visibility='hidden';
      if (pp_top) {
        top.location.replace(auth_fail_url);
      } else {
        document.location.replace(auth_fail_url);
      }
    }
    return false;
  }
  if (auth_res=="ok") {
    return true;
  }
}
function go_eurl(url,winname,winpar) { 
  if (typeof(winname)==='undefined') { document.location.href=unescape(url.replace(/(..)/g,"%$1"));} else { window.open(unescape(url.replace(/(..)/g,"%$1")),winname,winpar);}
}




function ap_popup() {
  var ap_pop_css = document.createElement('style');
  ap_pop_css.innerHTML = "#ap-modal-pop { display: none; position: fixed; z-index: 10000; left: 0; top: 0; width: 100%; height: 100%; overflow: auto; background-color: rgb(0,0,0); background-color: rgba(0,0,0,0.8); backdrop-filter: blur(3px);}";
  document.head.appendChild(ap_pop_css);
  var ap_pop_div=document.createElement("div");
  ap_pop_div.id = 'ap-modal-pop';
  ap_pop_div.innerHTML = '<span id="ap_login_up"></span>';
  var ap_pop_script = document.createElement("script");
  var ap_set_urlok=''; //if (!ap_return) { ap_set_urlok='&set_urlok='+escape('https://www.authpro.com/auth/'+pp_user+'/?action=home'); }
  if (ap_return) { ap_set_urlok='&set_urlok=ap_popup:close'; }
  if ((ap_return)&&(!auth_ajax)) { ap_set_urlok='&set_urlok='+escape(document.location.href); }
  ap_pop_script.src = 'https://www.authpro.com/auth/'+pp_user+'/?mode=JS&JSid=ap_login_up'+ap_set_urlok;
  ap_pop_div.appendChild(ap_pop_script); 
  document.body.appendChild(ap_pop_div);
  document.getElementById("ap-modal-pop").style.display = "block";
  if (typeof(ap_popup_ext) == 'function') { ap_popup_ext(ap_pop_div); } 
}


function ap_ready() {
  if (document.getElementById('ap_cover')) {
    if (auth_res=='ok') { document.getElementById('ap_cover').style.display = 'none'; }
  }
  if (typeof(ap_ready_ext) == 'function') { ap_ready_ext(); } 
}

if (document.addEventListener) { document.addEventListener("DOMContentLoaded", ap_ready); }
if (window.addEventListener) { window.addEventListener('load', ap_ready); } 
else { window.attachEvent('onload', ap_ready); }
