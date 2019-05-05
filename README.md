# EX4
## 1.总体
![总体](https://github.com/PresidentChao/EX4/blob/master/1.png)
## 2.In-line preferences
### 
    <PreferenceCategory android:title="In-line preferences">
        <CheckBoxPreference
            android:key="checkbox_preference"
            android:summary="This a checkbox"
            android:title="Checkbox_preference"/>
    </PreferenceCategory>
![linearlayout](https://github.com/PresidentChao/EX4/blob/master/2.png)
## 3.Dialog-based preferences
### 
    <PreferenceCategory android:title="Dialog-based preferences">
        <EditTextPreference
            android:dialogTitle="Enter your favorite animal"
            android:title="EditTextPreference"
            android:key="edittext_preference"
            android:summary="An example that uses an edit text dialog"/>
        <ListPreference
            android:entries="@array/options"
            android:entryValues="@array/options"
            android:dialogTitle="Choose one"
            android:summary="An example that use a list dialog"
            android:title="List prefernce"
            android:key="list_preference"/>
        <!--需要补充列表项的数据来源-->
    </PreferenceCategory>
![linearlayout](https://github.com/PresidentChao/EX4/blob/master/3.png)
![linearlayout](https://github.com/PresidentChao/EX4/blob/master/4.png)
## 4.Launch preferences
### 
    <PreferenceCategory android:title="Launch preferences">
        <PreferenceScreen
            android:key="screen_preference"
            android:summary="Shows another screen of preferences"
            android:title="Screen preference">
            <CheckBoxPreference
                android:key="next_scrren_checkbox_preference"
                android:summary="Preference that is on the next screen but same hierarchy"
                android:title="Toggle preference"/>
        </PreferenceScreen>
        <PreferenceScreen
            android:summary="Launches an Activity from an intent"
            android:title="Intent preference"/>
        <intent
            android:action="android.intent.action.VIEW"
            android:data="http://www.baidu.com"/>
    </PreferenceCategory>
![linearlayout](https://github.com/PresidentChao/EX4/blob/master/5.png)
![linearlayout](https://github.com/PresidentChao/EX4/blob/master/6.png)
## 5.Preference attributes
### 
    <PreferenceCategory android:title="Preference attributes">
        <CheckBoxPreference
            android:key="parent_checkbox_preference"
            android:summary="This is visually parent"
            android:title="Parent checkbox preference" />
        <!-- 子类的可见类型是由样式属性定义的 -->
        <CheckBoxPreference
            android:dependency="parent_checkbox_preference"
            android:key="child_checkbox_preference"
            android:summary="This is visually a child"
            android:title="Child checkbox preference" />
    </PreferenceCategory>
![linearlayout](https://github.com/PresidentChao/EX4/blob/master/7.png)
![linearlayout](https://github.com/PresidentChao/EX4/blob/master/8.png)
