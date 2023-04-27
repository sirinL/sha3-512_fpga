CN:  
修改了`padding1.v`中的填充，从 `0x01`     修改为   `0x06`  
在SHA3标准化时，NIST修改了填充算法，修改为   `N|01|10*1`  
将字节中的位从低位到高位排列，填充结果从`10000000`修改为`01100000`  
  
EN:  
Modify `padding1.v` module, from `0x01`    to       `0x06`  
Reorder bits from LSB to MSB, result of padding from `10000000` to `01100000`  

| Hex | 0x01  | 0x06|
|:---：|：---：|：---：|
|Bin|00000001|00000110|
|Reordered|10000000|01100000|
