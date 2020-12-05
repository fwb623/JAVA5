# Java5
### 第5次实验
## Student homework processing system
 #### 范文博 2020322103 G计202
## 1.实验目的： 
- 1.掌握字符串String及其方法的使用。
- 2.掌握文件的读取/写入方法。
- 3.掌握异常处理结构。
## 2.实验内容：
- 1.在某课上,学生要提交实验结果，该结果存储在一个文本文件A中。
- 2.在文件A中写学生的本信息。（学生姓名，年龄，性别，班级，学号）
- 3.在文件A中写学生处理后的作业信息。（长恨歌的古诗整齐写出）
- 4.统计学生作业中某个词或字出现的次数。
- 5.需要考虑学生可能写错，要设计异常处理。
## 3.实验要求：
- 1.设计学生类（包括学生姓名，年龄，性别，班级，学号）。
- 2.采用交互式方式实例化某学生。（Scanner）
- 3.写长恨歌时要求每7个汉字加入一个标点符号，奇数时加“，”，偶数时加“。”。
- 4.允许提供输入参数，统计古诗中某个字或词出现的次数。
- 5.输入的文本来源于文本文件B读取，把“古诗处理后的输出”结果存储到学生基本信息所在的文本文件A中。
 ## 4.实验过程：
 - 1.首先要创建学生类，填写学生信息。
 
        public class Student {
	         String Name;
         	String Sex;
	       public void setName(String Name) {
			    this.Name = Name;}
 - 2.然后实例化学生类。
 
        Student stu=new Student();
		      Scanner s=new Scanner(System.in);
		      System.out.println("姓名：");		
	      	String Name =s.next();
 - 3.创建A文件夹把A文件夹中的长恨歌按要求整理，在Txt类中整理。
 
       while ((fInputStream.read(ch)) !=-1) {
	                st.append(ch, 0,7);
	                st.append("，");
	                st.append(ch, 7, 7);
	                st.append("。"+"\n");
- 4.把A文件夹用B文件夹读取。
  
          FileReader fInputStream = new FileReader("F:////A.txt");//输入流文件
	         FileWriter fOutputStream  = new FileWriter("F:////B.txt")
- 5.做异常处理

	            try{              
                              }
           		catch (IOException e) {
		              	e.printStackTrace();
	                                 	}
-6.提取古诗中的字在文章中出现过几次。

              while ((len=fis.read(buffer))!=-1){
			             bos.write(buffer,0,len)；      	}
		              	data = bos.toByteArray();
			           String str1 = new String(data);
               int count=0;
		           	Scanner sc = new Scanner(System.in);
	          		 System.out.println("输入你要查找的字或词：");
			              char o = sc.next().charAt(0);
		              	char[] ch1 =str1.toCharArray();
			           for(int i=0;i<ch1.length;i++){
			              if(o==ch1[i]){
			                count++; }
## 5.流程图： 
https://github.com/fwb623/Java5/blob/main/%E6%B5%81%E7%A8%8B%E5%9B%BE.PNG
## 6.核心代码 ：

         public static void main(String args[]) throws FileNotFoundException, IOException {}//文件头
           try (FileReader fInputStream = new FileReader("F:////A.txt");     //写文件，输入输出
	             FileWriter fOutputStream  = new FileWriter("F:////B.txt")){
	            StringBuffer st=new StringBuffer();
	            while ()  {                    }//whiile语句
	                 }
            try{         }；   catch(Exception e) {    }；//异常处理
               Scanner s=new Scanner(System.in);   //运行输入语句
                  if( ){                }//if语句

## 7.系统运行结果：
## 8.实验感想：
