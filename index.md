<?xml version="1.0" encoding="utf-8"?>
<android.support.design.widget.CoordinatorLayout xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    android:layout_width="match_parent"
    android:background="@android:color/white"
    android:fitsSystemWindows="true"
    android:layout_height="match_parent">
    <android.support.design.widget.AppBarLayout
        android:id="@+id/appbar"
        android:layout_width="match_parent"
        android:layout_height="wrap_content">
        <android.support.design.widget.CollapsingToolbarLayout
            android:layout_width="wrap_content"
            android:layout_height="wrap_content">
            <android.support.v7.widget.Toolbar
                android:id="@+id/mTbComicTime"
                android:layout_width="match_parent"
                android:layout_height="wrap_content"
                android:background="@color/primary"
                android:elevation="@dimen/toolbar_elevation"
                android:theme="@style/ThemeOverlay.AppCompat.Dark.ActionBar"
                app:contentInsetStartWithNavigation="0dp"
                app:navigationIcon="@drawable/ic_toolbar_back"
                app:title="时间表" />
        </android.support.design.widget.CollapsingToolbarLayout>
        
    </android.support.design.widget.AppBarLayout>

    <android.support.design.widget.TabLayout
            android:id="@+id/mTbComicTimeTab"
            android:layout_width="match_parent"
            android:layout_height="wrap_content"
            android:layout_below="@id/mTbComicTime" />
    
   
    <android.support.v4.view.ViewPager
        android:id="@+id/mVpComic_time"
        android:layout_width="match_parent"
        android:layout_height="match_parent"
        android:layout_below="@id/mTbComicTime" />
</android.support.design.widget.CoordinatorLayout>
