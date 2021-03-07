package test;

public class class1 {
	public static void main(String[] args) {
		java.util.Scanner s = new java.util.Scanner(System.in);
		
		System.out.print("请输入歌曲名称:");
		String SongName = s.nextLine();
		System.out.print("请输入歌曲单价:");
		double SongPrice = s.nextFloat();
		System.out.print("请输入歌曲数量:");
		int SongNumber = s.nextInt();
		
		double TotalRevence;
		double ManageRevence;
		double SiteRevence;
		double ManageRate = 0.12;
		double SiteRate = 0.03;
		
		TotalRevence = SongPrice * SongNumber;
		ManageRevence = TotalRevence * ManageRate;
		SiteRevence = TotalRevence * SiteRate;
		
		System.out.println("歌曲总利润为" + TotalRevence);
		System.out.println("经理总利润为" + ManageRevence);
		System.out.println("网站总利润为" + SiteRevence);
	}

}
