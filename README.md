# **ToastLib**

ToastLib is Library for Customize Toast.

**_Methods_** for implement

  // ToastEnum.SHORT or ToastEnum.LONG
  <br /> 
  .**duration**(ToastEnum enum)
    <br /> <br /> 
  // Toast background color
  <br /> 
  .**backgroundColor**(int backgroundColor)
 <br /> <br /> 
  // Toast content textcolor
  <br /> 
  .**textColor**(int textColor)
  <br /> <br /> 
  // Toast content textsize (in SP), default is 20
  <br /> 
  .**textSize**(int size)
  <br /> <br /> 
  // Typeface for applying font to text
  <br /> 
  .**typeface**(Typeface ttf)
  <br /> <br /> 
  // true or false, for style bold to content
  <br /> 
  .**isBold**(boolean isBold)
  <br /> <br /> 
  // to apply fontAwesome icon, put fa-string in param
  <br /> 
  .**icon**(String faString)
  <br /> <br /> 
  // to add icon (drawable) in toast
  <br /> 
  .**icon**(int icon)
  <br />  <br /> 
  // to apply tint color on icon
  <br /> 
  .**iconColor**(int iconColor)
  <br /> <br /> 
  // icon size in dp, default is (24, 24)
  <br /> 
  .**iconSize**(int w, int h)
  <br /> <br />
  // corner radius for content, default is 4dp
  <br /> 
  .**corner**(int radius)
  <br /> <br />
  // margin from bottom/top (if Gravity is top then margin count from TOP and same for Bottom), default is 36
  <br /> 
  .**margin**(int margin)
  <br /> <br /> 
  // padding for inner content (default is 4)
  <br /> 
  .**padding**(int padding)
  <br /> <br />
  // space between icon and content, default is 8
  <br /> 
  .**spacing**(int spacing)
  <br /> <br /> 
  // toast UI stroke width and strokecolor
  <br /> 
  .**stroke**(int strokeWidth, int strokeColor)
  <br /> <br /> 
  // Gravity for placing toast (_NOTE_: .margin apply only for TOP and BOTTOM Gravity)
  <br /> 
  .**gravity**(int Gravity)
  <br /> <br /> 
  // to show toast
  <br /> 
  .**show**()

**Usage**
<br />
 new ToastLib.Builder(this, "Login Success")<br />
                 <tab/>.duration(ToastEnum.SHORT)<br />
                 .backgroundColor(ContextCompat.getColor(this, R.color.green))<br />
                 .textColor(ContextCompat.getColor(this, R.color.black))<br />
                 .textSize(18)<br />
                 .typeface(Typeface.createFromAsset(getAssets(), "fonts/OpenSans-Regular.ttf"))<br />
                 .isBold(true)<br />
                 .icon(getString(R.string.fa_success))<br />
                 .icon(R.drawable.ic_check_black_24dp)<br />
                 .iconColor(ContextCompat.getColor(this, R.color.black))<br />
                 .iconSize(24, 24)<br />
                 .corner(8)<br />
                 .margin(56)<br />
                 .padding(36)<br />
                 .spacing(16)<br />
                 .stroke(2, ContextCompat.getColor(this, R.color.dark_green))<br />
                 .gravity(Gravity.BOTTOM)<br />
                 .show();
<br /> <br />
![alt tag](https://raw.githubusercontent.com/droidbyme/ToastLibrary/master/screenshots/screen1.png)
 <br />

**For Success Toast** <br />
ToastLib.success(this, "Success", Typeface.createFromAsset(getAssets(), "fonts/OpenSans-Regular.ttf"));
 <br /> <br />
![alt tag](https://raw.githubusercontent.com/droidbyme/ToastLibrary/master/screenshots/screen2.png)

**For Error Toast** <br />
ToastLib.error(this, "Ooops! Try Again..", Typeface.createFromAsset(getAssets(), "fonts/OpenSans-Regular.ttf"));
 <br /> <br />
 <br />
![alt tag](https://raw.githubusercontent.com/droidbyme/ToastLibrary/master/screenshots/screen3.png)

 <br />
 **For Loading/Progress Toast** <br />
 ToastLib.progress(this, "Loading..", Typeface.createFromAsset(getAssets(), "fonts/OpenSans-Regular.ttf"));
![alt tag](https://raw.githubusercontent.com/droidbyme/ToastLibrary/master/screenshots/screen4.png)
 <br /> <br />