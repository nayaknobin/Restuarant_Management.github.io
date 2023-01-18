# Restuarant_Management.github.io
package Project;

import java.util.*;
class Restaurant_management {
    public static void main(String[] args) {
        Scanner in=new Scanner(System.in);
        int vstr,tvstr=0,nvstr,tnvstr=0,vfd,tvfd=0,nvfd,tnvfd=0,fd=0,tfd=0,amt=0,tamt=0,totalamt=0,totald=0,d,damt=0,ch;
        double gst=0;
        String str="",ans,choice="Y";
        System.out.println("************Welcome to the Multi-Cuisine Restaurant!!!*********");
        System.out.println(".............Starter Corner.........: 1");
        System.out.println(".............Main Course............: 2");
        System.out.println(".............Deserts ...............: 3");
        System.out.println();
        System.out.println("Press 1 for Starter");
        System.out.println("Press 2 for Main Course");
        System.out.println("Press 3 for Cool with Deserts");
        System.out.println();
        System.out.println("Enter Your Choice ");
        ch=in.nextInt();
        switch(ch){
            case 1:
            System.out.println("***********Welcome to Starter Menu!!!********");
            System.out.println("Enter 'VS' for Veg Starter and 'NVS' for Non-Veg Starter");
            str=in.next();
            if(str.equalsIgnoreCase("VS")){
                System.out.println("Starter\t\t\t\t\tPrice (in Rs.)");
                System.out.println("1.  Paneer Tikka\t\t\t110");
                System.out.println("2.  Paneer Pakoda\t\t\t100");
                System.out.println("3.  Veg Seekh Kebab\t\t\t160");
                System.out.println("4.  Paneer Masala \t\t\t200");
                System.out.println("5.  American Corn Ballr\t\t\t 90");
                System.out.println("6.  Cripsy Baby Cornt\t\t\t160");
                System.out.println("7.  Veg Briyani\t\t\t\t240");
                System.out.println("8.  Chilli Paneer\t\t\t120");
                System.out.println("9.  Cripsy Mushroom\t\t\t150");
                System.out.println("10. Dal Tadka\t\t\t\t140");
                System.out.println();
                while(choice.equalsIgnoreCase("Y"))
                {
                    System.out.println("Choose your starter from the above list by entering number.");
                    vstr=in.nextInt();
                    System.out.println("Enter the total number of starters you want.");
                    tvstr=in.nextInt();
                    if(vstr==1)
                    amt=tvstr*110;
                    if(vstr==2)
                    amt=tvstr*100;
                    if(vstr==3)
                    amt=tvstr*160;
                    if(vstr==4)
                    amt=tvstr*200;
                    if(vstr==5)
                    amt=tvstr*90;
                    if(vstr==6)
                    amt=tvstr*160;
                    if(vstr==7)
                    amt=tvstr*240;
                    if(vstr==8)
                    amt=tvstr*120;
                    if(vstr==9)
                    amt=tvstr*150;
                    if(vstr==10)
                    amt=tvstr*140;
                    tamt=tamt+amt;
                    System.out.println("Do you want to place more order ? Enter Y/N");
                    choice=in.next();
                }
            }
            if(str.equalsIgnoreCase("NVS")){
                System.out.println("..........Non-Vegetarian Starter..........");
                System.out.println();
                System.out.println("Non-Veg Starters\t\t\tPrice (in Rs.)");
                System.out.println("1.  Chicken Tikka\t\t\t130");
                System.out.println("2.  Chicken Pakoda\t\t\t100");
                System.out.println("3.  Chicken Seekh Kebabt\t\t160");
                System.out.println("4.  Chicken Tandori\t\t\t220");
                System.out.println("5.  Omlette\t\t\t\t 50");
                System.out.println("6.  Hydrebad Dum Briyani\t\t260");
                System.out.println("7.  Egg Briyani\t\t\t\t200");
                System.out.println("8.  Chilli Chicken\t\t\t130");
                System.out.println("9.  Fish Ajwani Tikka\t\t\t150");
                System.out.println("10. Double Mix Non-Veg Roll\t\t140");
                System.out.println();
                while(choice.equalsIgnoreCase("Y"))
                {
                    System.out.println("Choose your starter from the above list by entering number.");
                    nvstr=in.nextInt();
                    System.out.println("Enter the total number of starters you want.");
                    tnvstr=in.nextInt();
                    if(nvstr==1)
                    amt=tnvstr*130;
                    if(nvstr==2)
                    amt=tnvstr*100;
                    if(nvstr==3)
                    amt=tnvstr*160;
                    if(nvstr==4)
                    amt=tnvstr*220;
                    if(nvstr==5)
                    amt=tnvstr*50;
                    if(nvstr==6)
                    amt=tnvstr*260;
                    if(nvstr==7)
                    amt=tnvstr*200;
                    if(nvstr==8)
                    amt=tnvstr*130;
                    if(nvstr==9)
                    amt=tnvstr*150;
                    if(nvstr==10)
                    amt=tnvstr*140;
                    tamt=tamt+amt;
                    System.out.println("Do you want to place more order ? Enter Y/N");
                    choice=in.next();
            }
        }
        System.out.println("******** Multi Cuisine Restaurant ********");
        System.out.println("********** Bill **********");
        System.out.println("Total Cost =Rs."+tamt);
        gst=Math.round(18.0/100.0*tamt);
        System.out.println("GST = 18.0%");
        System.out.println("Total GST = Rs."+gst);
        System.out.println("Amount to be paid = Rs."+(tamt+gst));
        System.out.println();
        break;
        case 2:
        System.out.println("..............Main Course: Indian and Chinese Dishes!..........");
        System.out.println("Enter 'V' for Indian Veg Dishes and 'NV' for Indian Non-Veg Dishes and 'C' for Chineses Dishes.");
        str=in.next();
        if(str.equalsIgnoreCase("V")){
            System.out.println("..........Welcome to Indian Veg Dishes......");
            System.out.println();
            System.out.println("Indian Veg Dishes\t\t\tPrice (in Rs.)");
            System.out.println("1.  Shahi Paneer\t\t\t180");
            System.out.println("2.  Navrantan Korna\t\t\t180");
            System.out.println("3.  Paneer Seekh Kebabt\t\t\t160");
            System.out.println("4.  Malai Kofta\t\t\t\t160");
            System.out.println("5.  Mixed Vegetables\t\t\t120");
            System.out.println("6.  Makai Corn Palak\t\t\t 90");
            System.out.println("7.  Butter Naan\t\t\t\t 50");
            System.out.println("8.  Stuffed Kulcha\t\t\t 40");
            System.out.println("9.  Kashmiri Palao\t\t\t150");
            System.out.println("10. Shabnam Curry\t\t\t170");
            System.out.println();
            while(choice.equalsIgnoreCase("Y"))
            {
                System.out.println("Choose your Main Veg Course from the above list by entering number.");
                vfd=in.nextInt();
                System.out.println("How many plates do you want to place from the above list ?");
                tvfd=in.nextInt();
                if(vfd==1)
                amt=tvfd*180;
                if(vfd==2)
                amt=tvfd*180;
                if(vfd==3)
                amt=tvfd*160;
                if(vfd==4)
                amt=tvfd*160;
                if(vfd==5)
                amt=tvfd*120;
                if(vfd==6)
                amt=tvfd*90;
                if(vfd==7)
                amt=tvfd*50;
                if(vfd==8)
                amt=tvfd*40;
                if(vfd==9)
                amt=tvfd*150;
                if(vfd==10)
                amt=tvfd*170;
                totalamt=totalamt+amt;
                System.out.println("Do you want to place more order ? Enter Y/N");
                choice=in.next();
            }
        }
        if(str.equalsIgnoreCase("NV")){
            System.out.println(".........Welcome to Indian Non-Veg Dishes.........");
            System.out.println();
            System.out.println("Indian Non-Veg Dishes\t\t\tPrice (in Rs.)");
            System.out.println("1.  Chicken Tikka Masala\t\t180");
            System.out.println("2.  Chicken Tikka Labadar\t\t200");
            System.out.println("3.  Chicken Bharta\t\t\t160");
            System.out.println("4.  Muglai Chicken\t\t\t190");
            System.out.println("5.  Chicken Do Pyaza\t\t\t170");
            System.out.println("6.  Mutton Togan Josh\t\t\t290");
            System.out.println("7.  Prawn Malai Curry\t\t\t150");
            System.out.println("8.  Fish Sarsowala\t\t\t140");
            System.out.println("9.  Chicken Butter Masala\t\t150");
            System.out.println("10. Fish Dhaniwala\t\t\t170");
            System.out.println();
            while(choice.equalsIgnoreCase("Y"))
            {
                System.out.println("Choose your Main Non-Veg Course from the above list by entering number.");
                nvfd=in.nextInt();
                System.out.println("How many plates do you want to place from the above list ?");
                tnvfd=in.nextInt();
                if(nvfd==1)
                amt=tnvfd*180;
                if(nvfd==2)
                amt=tnvfd*200;
                if(nvfd==3)
                amt=tnvfd*160;
                if(nvfd==4)
                amt=tnvfd*190;
                if(nvfd==5)
                amt=tnvfd*170;
                if(nvfd==6)
                amt=tnvfd*290;
                if(nvfd==7)
                amt=tnvfd*150;
                if(nvfd==8)
                amt=tnvfd*140;
                if(nvfd==9)
                amt=tnvfd*150;
                if(nvfd==10)
                amt=tnvfd*170;
                totalamt=totalamt+amt;
                System.out.println("Do you want to place more order ? Enter Y/N");
                choice=in.next();
            }
        }
        if(str.equalsIgnoreCase("C")){
            System.out.println("..........Welcome to Chinese Dishes.........");
            System.out.println();
            System.out.println("Chinese Dishes\t\t\tPrice in Rs.");
            System.out.println("1.  ScheZwan Fried Rice\t\t\t240");
            System.out.println("2.  Schezwan Chicken\t\t\t290");
            System.out.println("3.  Chilli Chicken\t\t\t160");
            System.out.println("4.  Chicken Manchurian\t\t\t220");
            System.out.println("5.  Veg. Hakka Noodles\t\t\t170");
            System.out.println("6.  Paneer Manchurian\t\t\t160");
            System.out.println("7.  Chilly Paneet\t\t\t150");
            System.out.println("8.  Fish Fried\t\t\t\t140");
            System.out.println("9.  Chicken Fried Rice\t\t\t190");
            System.out.println("10. Kimchi Rice Veg\t\t\t220");
            System.out.println();
            while(choice.equalsIgnoreCase("Y"))
            {
                System.out.println("Choose your Main  Course from the above list by entering number.");
                fd=in.nextInt();
                System.out.println("How many plates do you want to place from the above list ?");
                tfd=in.nextInt();
                if(fd==1)
                amt=tfd*240;
                if(fd==2)
                amt=tfd*290;
                if(fd==3)
                amt=tfd*160;
                if(fd==4)
                amt=tfd*220;
                if(fd==5)
                amt=tfd*170;
                if(fd==6)
                amt=tfd*160;
                if(fd==7)
                amt=tfd*150;
                if(fd==8)
                amt=tfd*140;
                if(fd==9)
                amt=tfd*190;
                if(fd==10)
                amt=tfd*220;
                totalamt=totalamt+amt;
                System.out.println("Do you want to place more order ? Enter Y/N");
                choice=in.next();
            }
        }
        System.out.println("********** Multi Cuisine Restaurant **********");
        System.out.println("************* Bill ************");
        System.out.println("Total Cost =Rs."+totalamt);
        gst=Math.round(18.0/100.0*totalamt);
        System.out.println("GST = 18.0%");
        System.out.println("Total GST = Rs."+gst);
        System.out.println("Amount to be paid = Rs."+(totalamt+gst));
        System.out.println();
        break;
        case 3:
                System.out.println("..................Cool With Deserts..................");
                System.out.println();
                System.out.println("  Deserts\t\t\t\t Price (in Rs.)");
                System.out.println("1.  Softy Pineapple\t\t\t110");
                System.out.println("2.  Softy Cruncy Chocolate\t\t100");
                System.out.println("3.  Chocolate Walnut Brownie\t\t120");
                System.out.println("4.  Chocolate Doughtnut\t\t\t100");
                System.out.println("5.  Black Forest Gateaux\t\t90");
                System.out.println("6.  Chocolate shake\t\t\t160");
                System.out.println("7.  Pineapple Shake\t\t\t110");
                System.out.println("8.  Tooty Fruity\t\t\t120");
                System.out.println("9.  Mocha Magic\t\t\t\t80");
                System.out.println("10. Tooty Fruity\t\t\t130");
                System.out.println();
                while(choice.equalsIgnoreCase("Y"))
                {
                    System.out.println("Choose your desert from the above list by entering number.");
                    d=in.nextInt();
                    System.out.println("Enter the total number of items you want to buy!!");
                    totald=in.nextInt();
                    if(d==1)
                    damt=totald*110;
                    if(d==2)
                    damt=totald*100;
                    if(d==3)
                    damt=totald*120;
                    if(d==4)
                    damt=totald*100;
                    if(d==5)
                    damt=totald*90;
                    if(d==6)
                    damt=totald*160;
                    if(d==7)
                    damt=totald*110;
                    if(d==8)
                    damt=totald*120;
                    if(d==9)
                    damt=totald*80;
                    if(d==10)
                    damt=totald*130;
                    totalamt=totalamt+damt;
                    System.out.println("Do you want to place more order ? Enter Y/N");
                    choice=in.next();
                }
                System.out.println("************ Multi Cuisine Restaurant **********");
                System.out.println("************** Bill ************");
                System.out.println("Total Cost =Rs."+damt);
                gst=Math.round(18.0/100.0*damt);
                System.out.println("GST = 18.0%");
                System.out.println("Total GST = Rs."+gst);
                System.out.println("Amount to be paid = Rs."+(totalamt+gst));
                System.out.println();
                break;
                default:
                System.out.println("You have entered wrong choice!!!");
                System.out.println("You can enter in the Multi-Cuisine Restaurant by executing the program again with corrent choice!!!");
                System.out.println("Now, 'Quit' the program");
        }
            System.out.println("To exit the Multi Cuisine Restaurant World, enter the word 'QUIT'!!!");
            ans=in.next();
            if(ans.equals("quit")||ans.equals("Quit")||ans.equals("QUIT")){
                System.out.println("......Thanks For coming to Multi-Cuisine Restuarant!!!........");
                System.out.println("..........Your Pleasure Come Comfort!!!...........");
                System.out.println(".............Visit Again!!!...........");
                System.out.println();
            }
    }  
}
