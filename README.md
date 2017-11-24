import java.io.*;
class book
{
	int bid;
	String bname;
	boolean status;
	BufferedReader br=new BufferedReader(new InputStreamReader(System.in));
	
	
	void add()throws Exception
	{
		System.out.println("enter the book id");
		bid =Integer.parseInt(br.readLine());
		System.out.println("enter the book name ");
		bname=br.readLine();
		status=true;
	}
	
	void issue()
	{
		if(status==true)
		{
		System.out.println("book issued succesfully");
		status=false;
		}
		else
		{
		System.out.println("book already issued");
		}
	}
	
	void submit()


