Reset Baseline Levels to Zero
=============================

#. In ArArCalc, open the Baseline Calibrations dialog box `File>Internal Databases>Baseline Calibrations`.
    .. image:: figures/baseline_calibration_path.png
        :width: 400

#. Set the time range from 14 days to present.
#. Note the weighted average value for each of the collectors.
    .. image:: figures/baseline_calibration_dialog_box.png
        :width: 800

#. In this case ... ::

    L2 = -0.0091
    L1 = -0.0113
    AX = -0.0064
    H1 = -0.0090
    H2 = +0.0031

#. Write down these numbers and their respective cups and open ArArExperiments and the `Manage` console.
    .. image:: figures/ArArEXPERIMENTS_manage_offsets.png
        :width: 800

#. In the `Manage` dialog box there are two columns.
    * ``UFC Offset [fA]`` - These are the current offsets.
    * ``Additional Offset [fA]`` - This is where you will enter in the values that were obtained in the previous steps (note, the cups are in the reverse order).
        .. image:: figures/ArArEXPERIMENTS_additional_offsets.png
            :width: 800

#. After entering in the values of each of the cups, `click` the ``Update XX Offset`` button.
#. The ``UFC Offset [fA]`` value should be refreshed with the new offset values.
#. Note these new values
#. Open `Instrument Control` and the ``Detector Setup`` dialog box.
    .. image:: figures/InstrumentControl_ArgusVI_tab.png
        :width: 800

#. This will bring up the ``Detector Setup Wizard``
    .. image:: figures/InstrumentControl_dector_setup_wizard.png
        :width: 800


#. From the previous step, paste the calculated ``UFC Offset [fA]`` values into the ``UFC Offset [fA]`` column in the ``Detector Setup Wizard`` window.
#. Click ``Apply Changes``.
#. Shutdown and restart the computer and ``Instrument Control``. Open the ``Detector Setup Wizard`` window again and confirm the values were entered.




