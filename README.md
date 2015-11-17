# DropAnimationView
---

Using Android Property Animation to implement the animation of leaves falling.

# Demo
---
![preview_drop_animation](preview_drop_animation.gif)

# Gradle dedependency
    compile 'com.waynell.library:drop-animation-view:1.0'
    
# Usage
---
First, add following code into your layout xml

    <com.waynell.library.DropAnimationView
        android:id="@+id/drop_animation_view"
        android:layout_width="match_parent"
        android:layout_height="match_parent"
        app:minSize="30dp"
        app:maxSize="50dp"
        app:largePercent="80%"
        app:rate="100"
        app:xAnimate="true"
        app:yAnimate="true"
        app:rotationAnimate="true"/>

Second, find this view and set drawables id

    DropAnimationView view = (DropAnimationView) findViewById(R.id.drop_animation_view);
    view.setDrawables(R.drawable.leaf_1,
            R.drawable.leaf_2,
            R.drawable.leaf_3,
            R.drawable.leaf_4,
            R.drawable.leaf_5,
            R.drawable.leaf_6);

finally, call startAnimation() begin doing animation.

