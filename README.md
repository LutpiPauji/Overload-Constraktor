# Overload-Constraktor

class kotak {
    double panjang;
    double lebar;
    double tinggi;
    //mendefinisikan contruktor tanpa parameter
    
    kotak (){
        panjang=0;
        lebar=0;
        tinggi=0;
    }
    //mendefinisikan contruktor dengan satu parameter
    kotak (double sisi){
    panjang=lebar=tinggi=sisi;
    }
    
    //mendefinisikan contruktor dengan tiga parameter 
    kotak (double p, double l, double t){
    panjang=p;
    lebar=l;
    tinggi=t;
            
    }
    
    double hitungvolume (){
        return (panjang*lebar*tinggi);
    }
}
public class OverloadConstraktor {
    public static void main (String []args){
    kotak k1,k2,k3;
    k1=new kotak ();
    k2=new kotak (10);
    k3=new kotak (4,3,2);
    
    //menampilkan volume
    System.out.println ("Volume k1= "+k1.hitungvolume());
    System.out.println ("Volume k2= "+k2.hitungvolume());
    System.out.println ("Volume k3= "+k3.hitungvolume());
    }
    
}
