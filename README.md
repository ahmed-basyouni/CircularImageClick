# CircularImageClick
A custom ImageButton that invoke onClickListener only when touch is inside the circle not outside (rectangle area of button)

# Demo

<p align="center">
  <img src="https://github.com/AndroidArk/CircularImageClick/blob/master/demo.gif?raw=true" width="350"/>
</p>

<h1> How to use it</h1>

simply inside your xml use the custom view like the following

```
<PackageName.CircularClickImageButton
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:id="@+id/circleButton"
        android:background="@android:color/transparent"
        android:src="@drawable/button_state"/>\
```

then inside your code <b>setOnCircleClickListener</b> like the following

```
imageButton.setOnCircleClickListener(new CircularClickImageButton.OnCircleClickListener() {
            @Override
            public void onClick(View v) {
                Toast.makeText(MainActivity.this, "Clicked" , Toast.LENGTH_SHORT).show();
            }
        });
```

###License
MIT License

Copyright (c) 2017 AndroidArk (Ahmed Basyouni)

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
