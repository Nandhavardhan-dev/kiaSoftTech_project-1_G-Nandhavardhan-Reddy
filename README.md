# kiaSoftTech_project-1_G-Nandhavardhan-Reddy

package kiasoft.pack;

import java.util.SplittableRandom;

public class OTPGenerator {
	
	public static void main(String[] args)
	{
		int length = 6;
		OTP(length);
	}
	static void OTP(int len)
	{
		//creating SplittableRandom class obj
		SplittableRandom sr=new SplittableRandom();
		//creating StringBuilder class obj
		StringBuilder sb=new StringBuilder();
		for (int i = 0; i < len; i++) {
			//nextInt(0,10) is to get a number b/w 0 to 9
			sb.append(sr.nextInt(0, 10));
		}
		//printing the sb(otp)
		System.out.println(sb);
	}
	
}
