Pulse Counter
=============

概述
--------

The PCNT (Pulse Counter) module is designed to count the number of rising and/or falling edges of an input signal. Each pulse counter unit has a 16-bit signed counter register and two channels that can be configured to either increment or decrement the counter. Each channel has a signal input that accepts signal edges to be detected, as well as a control input that can be used to enable or disable the signal input. The inputs have optional filters that can be used to discard unwanted glitches in the signal.

应用程序示例
-------------------

Pulse counter with control signal and event interrupt example: :example:`peripherals/pcnt`.

API 参考手册
-------------

头文件
^^^^^^^^^^^^

  * :component_file:`driver/include/driver/pcnt.h`


宏
^^^^^^


类型定义
^^^^^^^^^^^^^^^^


枚举
^^^^^^^^^^^^

.. doxygenenum:: pcnt_ctrl_mode_t
.. doxygenenum:: pcnt_count_mode_t
.. doxygenenum:: pcnt_unit_t
.. doxygenenum:: pcnt_channel_t
.. doxygenenum:: pcnt_evt_type_t

结构体
^^^^^^^^^^

.. doxygenstruct:: pcnt_config_t

函数
^^^^^^^^^

.. doxygenfunction:: pcnt_unit_config
.. doxygenfunction:: pcnt_get_counter_value
.. doxygenfunction:: pcnt_counter_pause
.. doxygenfunction:: pcnt_counter_resume
.. doxygenfunction:: pcnt_counter_clear
.. doxygenfunction:: pcnt_intr_enable
.. doxygenfunction:: pcnt_intr_disable
.. doxygenfunction:: pcnt_event_enable
.. doxygenfunction:: pcnt_event_disable
.. doxygenfunction:: pcnt_set_event_value
.. doxygenfunction:: pcnt_get_event_value
.. doxygenfunction:: pcnt_isr_register
.. doxygenfunction:: pcnt_set_pin
.. doxygenfunction:: pcnt_filter_enable
.. doxygenfunction:: pcnt_filter_disable
.. doxygenfunction:: pcnt_set_filter_value
.. doxygenfunction:: pcnt_get_filter_value
.. doxygenfunction:: pcnt_set_mode

