Clue Coffee Scale
============

.. image:: https://img.shields.io/badge/code%20style-black-000000.svg
    :target: https://github.com/psf/black
    :alt: Code Style: Black

The Clue Coffee Scale is a CircuitPython project designed to measure the weight of the ground
coffee beans or the extraction output to achieve repeatable results for your preferred brew.
To measure the contents of a container, the scale can be zeroed with a push of the Clue's ``A``
button to subtract the container's tare weight.

The scale uses a load cell sensor that consists of a very sensitive resistance array (a strain gauge)
attached to a metal bending beam. The specialized `NAU7802 Analog-to-Digital Converter (ADC)` breakout
board connects to the load cell and measures the slight changes in the array's differential voltage,
calculating the weight of the mass placed on the load cell.

The Clue interfaces with the `NAU7802 ADC` board and automatically updates a colorful graphics display
showing the results in both ounces and grams.

.. image:: https://github.com/CedarGroveStudios/Clue_Coffee_Scale/blob/master/media/clue_scale_01.jpg
   :width: 400
   :align: center
   :alt: Clue Coffee Scale in Action

Dependencies
=============
Hardware components:

* `CLUE - nRF52840 Express with Bluetooth LE, Adafruit PID: 4500 <https://www.adafruit.com/product/4500>`_
* `Clear Acrylic Enclosure + Hardware Kit for Adafruit CLUE, Adafruit PID: 4675 <https://www.adafruit.com/product/4675>`_
* `Strain Gauge Load Cell - 4 Wires - 1Kg, Adafruit PID: 4540 (or equivalent) <https://www.adafruit.com/product/4540>`_
* `NAU7802 24-Bit ADC - STEMMA QT / Qwiic, Adafruit PID: 4538 <https://www.adafruit.com/product/4538>`_
* `STEMMA QT / Qwiic JST SH 4-pin Cable - 100mm Long, Adafruit PID: 4210 <https://www.adafruit.com/product/4210>`_
* `3 x AAA Battery Holder with On/Off Switch and 2-Pin JST, Adafruit PID: 727 <https://www.adafruit.com/product/727>`_
* `USB cable - USB A to Micro-B - 3 foot long, Adafruit PID: 592 (or equivalent) <https://www.adafruit.com/product/592>`_
* `Clear Adhesive Squares - 6 pack - UGlu Dashes, Adafruit PID: 4813 <https://www.adafruit.com/product/4813>`_
* `Aluminum Extrusion Corner Brace Support (for 20x20), Adafruit PID: 1155 <https://www.adafruit.com/product/1155>`_
* `Coupling Plate - 3 Holes - 20x20 Aluminum Extrusion, Adafruit PID: 1216 <https://www.adafruit.com/product/1216>`_
* `Cross-Plate for 2020 Aluminum Extrusion, Adafruit PID: 1220 <https://www.adafruit.com/product/1220>`_
* `Wire Ferrule Kit - 800 pieces, Adafruit PID: 5131 <https://www.adafruit.com/product/5131>`_

Software dependencies:

* `Adafruit CircuitPython <https://github.com/adafruit/circuitpython>`_

... the font file:

* ``helvB24.bdf`` (placed into the project's ``fonts`` folder):

The font file can be found in the `fonts <https://github.com/CedarGroveStudios/Clue_Coffee_Scale/tree/master/bundle/fonts>`_ folder in the project bundle of the `Clue_Coffee_Scale` repository.

... the following CircuitPython Libraries (placed into the project's ``lib`` folder):

* ``adafruit_apds9960``
* ``adafruit_bitmap_font``
* ``adafruit_bmp280``
* ``adafruit_clue``
* ``adafruit_display_shapes``
* ``adafruit_display_text``
* ``adafruit_lis3mdl``
* ``adafruit_lsm6ds``
* ``adafruit_register``
* ``adafruit_sht31d``
* ``cedargrove_nau7802``
* ``neopixel``
* ``simpleio``

CircuitPython libraries can be found in the latest `Adafruit CircuitPython Library distribution <https://circuitpython.org/libraries>`_
or installed individually using `circup <https://github.com/adafruit/circup>`_.

.. image:: https://github.com/CedarGroveStudios/Clue_Coffee_Scale/blob/master/media/clue_scale_03.png
   :width: 400
   :align: center
   :alt: The Display Screen
