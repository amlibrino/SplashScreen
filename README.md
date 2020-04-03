# SplashScreen
une animation à l'ouverture de l'application

ôtons l'actionBar en modifiant le thème dans style.xml
    <style name="AppTheme" parent="Theme.AppCompat.Light.NoActionBar">


De même dans le MainActivity enlevons l'affichage de la bar d'information:

 protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        // enlevons la bare en haut
        getWindow().setFlags(WindowManager.LayoutParams.FLAG_FULLSCREEN,WindowManager.LayoutParams.FLAG_FULLSCREEN);
        setContentView(R.layout.activity_main);
  
 annimer le splash 
 	
<?xml version="1.0" encoding="utf-8"?>
<set xmlns:android="http://schemas.android.com/apk/res/android">
    <translate
        android:fromXDelta="0%"
        android:fromYDelta="-100%"
        android:duration="2000"/>
    <alpha
        android:fromAlpha="0.1"
        android:toAlpha="1.0"
        android:duration="1500"/>
</set>
