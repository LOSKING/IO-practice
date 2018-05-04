package com.bjpowernode.demo02;

import java.io.File;
import java.io.FileInputStream;
import java.io.FileNotFoundException;
import java.io.IOException;

public class Test02 {
/**
 * FileInputStream读取文件的内容
 * @param args
 * @throws IOException 
 */
	public static void main(String[] args) throws IOException {
		// 1)建立流通道
		FileInputStream fis = new FileInputStream("e:/abc.txt");
		//2)读取流中的内容
		int x = fis.read();
		System.out.println(x);
		//继续从流中读取字节
		x = fis.read();
		x = fis.read();
		x = fis.read();
		x = fis.read();
		x = fis.read();
		x = fis.read();
		System.out.println(x);
		x = fis.read();
		System.out.println(x);
		x = fis.read();
		System.out.println(x);
		x = fis.read();
		x = fis.read();
		System.out.println(x);
		x = fis.read();
		System.out.println(x);
		x = fis.read();
		System.out.println(x);
		
		
		//3)关闭流通道
		fis.close();
		
	}

}
