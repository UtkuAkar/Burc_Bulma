# Burc
Burc

import java.util.Scanner;

public class Burc {
    public static void main(String[] args) {

        int mount,day;
        String burc="";
        boolean isError=false; //isError Kavramı birşeyin basında is varsa true yada false alcaktır

        Scanner input=new Scanner(System.in);
        System.out.println("Doğdugunuz Ay : ");
        mount=input.nextInt();

        System.out.println("Doğdugunuz Gun : ");
        day=input.nextInt();


        switch (mount){
            case 1:
                if (day>=1 && day <=31){
                    if(day<22 ){
                        burc = "Oğlak";
                    } else {
                        burc = "Kova";
                        }
                    } else {
                       isError=true;
                    }
                    break;

            case 2:
                if (day>=1 && day <=28){
                    if(day<20 ){
                        burc = "Kova";
                    } else {
                        burc = "Balık";
                    }
                } else {
                    isError=true;
                }
                break;

            case 3:
                if (day>=1 && day <=31){
                    if(day<21 ){
                        burc = "Balık";
                    } else {
                        burc = "Koç";
                    }
                } else {
                    isError=true;
                }
                break;

            case 4:
                if (day>=1 && day <=30){
                    if(day<22 ){
                        burc = "Koç";
                    } else {
                        burc = "Boğa";
                    }
                } else {
                    isError=true;
                }
                break;

            case 5:
                if (day>=1 && day <=31){
                    if(day<22 ){
                        burc = "Boğa";
                    } else {
                        burc = "İkizler";
                    }
                } else {
                    isError=true;
                }
                break;

            case 6:
                if (day>=1 && day <=30){
                    if(day<23 ){
                        burc = "İkizler";
                    } else {
                        burc = "Yengeç";
                    }
                } else {
                    isError=true;
                }
                break;

            case 7:
                if (day>=1 && day <=31){
                    if(day<23 ){
                        burc = "Yengeç";
                    } else {
                        burc = "Aslan";
                    }
                } else {
                    isError=true;
                }
                break;

            case 8:
                if (day>=1 && day <=31){
                    if(day<23 ){
                        burc = "Aslan";
                    } else {
                        burc = "Başak";
                    }
                } else {
                    isError=true;
                }
                break;

            case 9:
                if (day>=1 && day <=30){
                    if(day<23 ){
                        burc = "Başak";
                    } else {
                        burc = "Terazi";
                    }
                } else {
                    isError=true;
                }
                break;

            case 10:
                if (day>=1 && day <=31){
                    if(day<23 ){
                        burc = "Terazi";
                    } else {
                        burc = "Akrep";
                    }
                } else {
                    isError=true;
                }
                break;

            case 11:
                if (day>=1 && day <=30){
                    if(day<22 ){
                        burc = "Akrep";
                    } else {
                        burc = "Yay";
                    }
                } else {
                    isError=true;
                }
                break;

            case 12:
                if (day>=1 && day <=31){
                    if(day<22 ){
                        burc = "Yay";
                    } else {
                        burc = "Oğlak";
                    }
                } else {
                    isError=true;
                }
                break;
            default:
                System.out.println("Hatalı");

        }


            if (isError){
                System.out.println("Hatalı Giriş Tekrar Dene");
            }else {
                System.out.println("Burcunuz : " + burc);

        }

    }
}

