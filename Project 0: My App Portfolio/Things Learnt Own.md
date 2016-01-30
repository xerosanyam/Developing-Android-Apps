### Customize button
1. Shadow: android:background="@android:drawable/dialog_holo_light_frame"
2. http://angrytools.com/android/button/
	
### Change color of button on button press
orderin of item is important

	drawable/buttonshape.xml
	<?xml version="1.0" encoding="utf-8"?>
	<selector xmlns:android="http://schemas.android.com/apk/res/android">
		<item android:state_pressed="true">
			<shape android:shape="rectangle">
				<corners android:radius="14dp" />
				<solid android:color="#b2dfdb" />
				<stroke android:width="3dp" android:color="#00695c" />
			</shape>
		</item>
		<item>
			<shape android:shape="rectangle">
				<corners android:radius="14dp" />
				<solid android:color="#ffffff" />
				<stroke android:width="1dp" android:color="#00695c" />
			</shape>
		</item>
	</selector>

### Vibration on button press
1.    <uses-permission android:name="android.permission.VIBRATE"></uses-permission>
2.    import android.os.Vibrator;
      Vibrator myvib= (Vibrator)this.getSystemService(VIBRATOR_SERVICE);
      myvib.vibrate(15);
