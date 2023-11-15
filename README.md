### stm32-sim800

This sim800 library is wroten by C programming language for stm32 microcontroller. The HAL library is used for wrote stm32 program.

### guidance for use library
**init sim800 module**

In first step you must write this code for prepare sim800 module :

     GSM_init();
This function has return value:

1 : sim800 module is ready to use.

0 : there is a problem in initializing module(you can check ret variable for debug)

**read received SMS**

     GSM_read_message();

received message and number are stored in these buffers:

        { receive_message[RX_BUFFER_SIZE]}
        { receive_message_number[RECEIVE_NUMBER_SIZE]}

