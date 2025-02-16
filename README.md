# Cryptohack_writeup

# 1. ENCODING

(1) ASCII
<br/>

  The following python code was used to obtain the flag<br/>
  <br/>

  ![image](https://github.com/user-attachments/assets/d457d404-40e4-4281-bdcb-1bdacb3b99ee)<br/>
  <br/>

  The flag value obtained is : crypto{ASCII_pr1nt4bl3}<br/>
  <br/>

  --------------------------------------------------------------

(2) HEX
<br/>

  The following python code was used to obtain the flag<br/>
  <br/>
  
  ![image](https://github.com/user-attachments/assets/9f2f64d2-9243-4b04-8787-deb9898fc475) <br/>
  <br/>

  The flag value obtained is : crypto{You_will_be_working_with_hex_strings_a_lot} <br/>
  <br/>

  --------------------------------------------------------------

(3) BASE64
<br/>

  The following python code was used to obtain the flag<br/>
  <br/>

  ![image](https://github.com/user-attachments/assets/00b8b435-e939-4b90-986f-9a3db8f3c6d4) <br/>
  <br/>

  The flag value obtained is : crypto/Base+64+Encoding+is+Web+Safe/ <br/>
  <br/>

  --------------------------------------------------------------

(4) BYTES AND BIG INTEGERS
<br/>

  The following python code was used to obtain the flag<br/> 
  <br/>

  ![image](https://github.com/user-attachments/assets/fde4417d-940f-498f-bc0a-1df7ef69ccbd)<br/>
  <br/>

  The flag value obtained is : crypto{3nc0d1n6_4ll_7h3_w4y_d0wn}<br/>
  <br/>

  --------------------------------------------------------------

(5) ENCODING CHALLENGE 
<br/>

  Made changes in the python code of 'pwntools...' provided with the help of YouTube videos and refering to different sites in Google.<br/>
  The required flag value was obtained after a series of changes made and it was displayed in the WSL interface as <br/>
  <br/>

  ![image](https://github.com/user-attachments/assets/d902109f-de12-4dee-9df0-b675b408e312)<br/>
  <br/>

  The flag value obtained is : crypto{3nc0d3_d3c0d3_3nc0d3}<br/>
  <br/>

  --------------------------------------------------------------

# 2. XOR

(1) XOR STARTER
<br/>

  The following python code was used to obtain the flag<br/>
  <br/>

  ![image](https://github.com/user-attachments/assets/5072e29a-bbae-4958-8d48-52b097983eb2)
  <br/>

  The variable ‘b’ is modified for each of the letters of the string ‘label’. Likewise each character for the FLAG is obtained.
  <br/>

  The flag value obtained is : crypto{aloha}
  <br/>

  --------------------------------------------------------------

(2) XOR PROPERTIES
<br/>

  The following python code was used to obtain the flag<br/>
  <br/>

  ![image](https://github.com/user-attachments/assets/40c55d0b-ab8e-468a-b3fe-018d18bd03fe)
  <br/>

  The flag value obtained is : crypto{x0r_i5_ass0c1at1v3}	
  <br/>

  --------------------------------------------------------------

(3) FAVOURITE BYTE
<br/>

  The following python code was used to obtain the flag<br/>
  <br/>

  ![image](https://github.com/user-attachments/assets/0d95d57a-20df-4f11-b530-a46f7c4d3234)
  <br/>

  First trying out with the possible numbers with a assumed limit. Since we obtain the FLAG from there itself, we are not trying out with the alphabets.
  <br/>

  ![image](https://github.com/user-attachments/assets/14c9dd9e-5121-4df4-af64-7d7cf5269e49)
  <br/>

  The flag value obtained is : crypto{0x10_15_my_f4v0ur173_by7e}
  <br/>

  --------------------------------------------------------------

(4) YOU EITHER KNOW, XOR YOU DON'T
<br/>

  The following python code was used to obtain the flag<br/>
  <br/>

  ![image](https://github.com/user-attachments/assets/739e138e-013c-4969-882e-219972c68a01)
  <br/>

  First I tried generating loops to check if the alphabets, numbers or the special characters satisfy and give the FLAG or not. Couldn’t obtain the FLAG this way. That is when I noticed about the ‘flag format’ mentioned in the task. I had no idea how to use it here. I then referred in sites to know the usage of it. I tried with a portion of the flag format from the idea got from some site I referred to. XORing that with the given text, for the ‘myXORke+y’ obtained, assumed that ‘myXORkey’ will be the secret key. By XORing this secret key with the text given, the FLAG was obtained.
  <br/>

  ![image](https://github.com/user-attachments/assets/21781e7d-7658-45ff-9181-be0e41ab5eb0)
  <br/>

  The flag value obtained is : crypto{1f_y0u_Kn0w_En0uGH_y0u_Kn0w_1t_4ll}
  <br/>

  --------------------------------------------------------------

(5) LEMUR XOR 
<br/>

  Since it was mentioned in the question to perform a visual XOR between the RGB bytes of the two images, the following command was executed in the WSL command-line interface :
  <br/>
		gmic a.png b.png -blend xor -o result.png
  <br/>

  ![image](https://github.com/user-attachments/assets/529f094d-14a5-4655-84c8-fae2be402894)
  <br/>

  The output image obtained is :
  <br/>

  ![image](https://github.com/user-attachments/assets/a9d51727-b459-4230-a382-16fc2c933ea8)
  <br/>

  The flag value obtained is : crypto{X0Rly_n0t!}
  <br/>

  --------------------------------------------------------------

# 3. MATHEMATICS

(1) GCD
<br/>

  The following python code was used to obtain the flag<br/>
  <br/>

  ![image](https://github.com/user-attachments/assets/29ac09f0-ff59-4125-b328-d3652b6d2c8b)
  <br/>

  Did using the algorithm of Euclid division algorithm for GCD.
  <br/>
   
Concept :
<br/>
 
Repeated division of 
<br/>
			  Largest = (smallest * p ) +  q
<br/>
     
For the next division, ‘smallest’ comes in place of ‘largest’ & ‘q’ comes in place of ‘smallest’. It is continued till the ‘q’ value becomes 0. In the program, ‘gcd = s’ is given because the ‘smallest’ value of the second last execution is the required GCD. If it is not given, the output will print as ‘0’.
<br/>

  ![image](https://github.com/user-attachments/assets/16e73c47-e835-4825-9d93-514c5e2a186f)
<br/>

  The flag value obtained is : 1512
  <br/>

  --------------------------------------------------------------

(2) EXTENDED GCD
<br/>

Did using the following concepts :

![image](https://github.com/user-attachments/assets/62e90f58-62ba-4e56-b315-a88a046b76b0)

![image](https://github.com/user-attachments/assets/b5fdae49-8f88-45d9-802e-246edc677d3c)

  The following python code was used to obtain the flag<br/>
  <br/>

  ![image](https://github.com/user-attachments/assets/c4836cca-478d-4da8-922d-410db0dcf591)

  ![image](https://github.com/user-attachments/assets/315f927c-72bd-4d10-99cc-8951ddcc3881)

  The flag value obtained is : -8404
  <br/>

  --------------------------------------------------------------

(3) MODULAR ARITHMETIC 1
<br/>

(x,y) = (5,4)
<br/>
	
The flag value is : 4
<br/>

--------------------------------------------------------------

(4) MODULAR ARITHMETIC 2
<br/>

  Solved using the following properties :

  ![image](https://github.com/user-attachments/assets/cdb2145d-f3f3-4c52-ba34-ba1534cac226)

  ![image](https://github.com/user-attachments/assets/c114ab31-bdc3-4ab5-bd97-ab4d1e3d5369)

The flag value is : 1
<br/>

--------------------------------------------------------------

(5) MODULAR INVERTING
<br/>

Solved using the concept given in question and from there itself was able to find out the flag value.
<br/>

The flag value is : 9
<br/>

--------------------------------------------------------------
