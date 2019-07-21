Build steps:

1)Use QT5+ to open 3 projects CheckAllx86Instructions1, ExecuteOpCode, OpCodeToText_objDump
2) fix the path in CheckAllx86Instructions1.main.cpp:
#define EXECUTEOPCODE "../build-ExecuteOpCode-Desktop_Qt_5_9_1_GCC_64bit-Debug/ExecuteOpCode"
#define GETOPCODEINSTRUCTION "../build-OpCodeToText_objDump-Desktop_Qt_5_9_1_GCC_64bit-Debug/OpCodeToText_objDump"
3.0) we generate every opcode (with certain exceptions) , 
3.1) we execute the exception using ExecuteOpCode
3.2) we use OpCodeToText_objDump to convert the opcode to readable instruction
