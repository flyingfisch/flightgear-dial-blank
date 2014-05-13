README
======

A blank instrument for FlightGear.

How to use
----------
Just include it in your model xml like so:

    <model>
        <name>extraleftbottom1</name>
        <path>Models/Instruments/blank/blank.xml</path>
        <offsets>
            <x-m>2.02548</x-m>
            <y-m>-.4571852</y-m>
            <z-m>.2109746</z-m>
         </offsets>
    </model>


How to customize
----------------

### Change size
The instrument is 8cm in diameter. If you need it to be larger or smaller, use an overlay like this:

    <model>
        <name>extraleftbottom1</name>
        <path>Models/Instruments/blank/blank.xml</path>
        <offsets>
            <x-m>2.02548</x-m>
            <y-m>-.4571852</y-m>
            <z-m>.2109746</z-m>
         </offsets>

        <overlay>
            <animation n="100">
                <type>scale</type>
                <property>constants/zero</property>
                <!-- scale multipliers go here. The ones below will make the gauge 6cm in diameter. -->
                <x-offset>.75</x-offset>
                <y-offset>.75</y-offset>
                <z-offset>.75</z-offset>
            </animation>
        </overlay>
    </model>

### Change logo
The default logo is Beechcraft, if you want to change it, just change blank.png. Some premade logos are already made; if you want to use one, just rename the relevent one to blank.png