import basis.*;
import java.math.BigInteger; 
import java.math.BigDecimal;
import java.util.Scanner;

/**
 * Von Tuhin Thodeme Q1
 * Version 2
 * 
 * Datum:27.02.2020
 * 
 * Das ganze Programm und die Verschlüsselung und Entschlüsselung 
 * wurde selbständig von mir programmiert
 * 
 */
public class cclient extends Client
{
    private String send,rt, entschlusseltText,zwischenSpeicher1;
    private long berechne;
    private char zwischenSpeicher;
    private int zwischenSpeicher2,y;
    private Fenster win;
    private TextFeld text;
    private Knopf senden, schließen;
    private BeschriftungsFeld feld,feld2;
    private BigInteger big,bigexponent,bigmodulo;
    private int oSchlusselExpo, oSchlusselMod;
    public cclient(String sip, int sport)
    {
        super(sip,sport);

        win = new Fenster(400,400);
        feld = new BeschriftungsFeld("User 1 Chatmodul",30,30,300,40);
        feld2 = new BeschriftungsFeld("Nachricht eingeben und senden:", 30, 55,300,40);
        text = new TextFeld(30,100,300,40);
        text.setzeText(" ");
        senden = new Knopf("Senden", 30, 145, 85,40);
        schließen = new Knopf("Schließen", 150, 145,85,40);
        System.out.println("-Neue Sitzug--> ");
        System.out.println("---User 1 erstellt---");
        
        //Öffentlicher Schlüssel von User 2 bzw Server 
        oSchlusselExpo = 7;
        oSchlusselMod = 253;
        
        // Privater Schlüssel von User 1 bzw Client
        bigexponent = new BigInteger("77");
        bigmodulo = new BigInteger("221");
        rt = "";
        while(isConnected()== false){
            Hilfe.kurzePause();
        }
        System.out.println("---Verbunden---");
        this.handling();
    }

    public void handling(){
        while(!schließen.wurdeGedrueckt()){
            
            if(senden.wurdeGedrueckt()){ 
               if(text.text()==null){
                }
               
               else{
                //Senden von der Nachricht und Aufrufen der Verschlüsselung
                super.send(this.verschlusselung(text.text()));
               System.out.println("User 1 (Du): "+text.text());
                text.setzeText(" ");
            }
            }
            Hilfe.kurzePause();
        }
        win.gibFrei();
    }

    public String verschlusselung(String nachricht){
        rt = "";
        //Verschlüsselung der Nachricht durch RSA
        //Buchstaben werden umgewandelt in eine Zahl, angelehnt an das UTF-8 System
        //Die Schlüssel wurden schon voher berechnet, siehe Facharbeit
        for(int l = 0 ; l<nachricht.length();l++){
            zwischenSpeicher = nachricht.charAt(l);
            if(zwischenSpeicher == 'A'){
                berechne = (long) (Math.pow(41,oSchlusselExpo))%oSchlusselMod;
                rt = rt+berechne+",";
            }
            if(zwischenSpeicher == 'B'){
                berechne = (long) (Math.pow(42,oSchlusselExpo))%oSchlusselMod; 
                rt = rt+berechne+",";
            }  
            if(zwischenSpeicher == 'C'){
                berechne = (long) (Math.pow(43,oSchlusselExpo))%oSchlusselMod; 
                rt = rt+berechne+",";
            }
            if(zwischenSpeicher == 'D'){
                berechne = (long) (Math.pow(44,oSchlusselExpo))%oSchlusselMod; 
                rt = rt+berechne+",";
            }
            if(zwischenSpeicher == 'E'){
                berechne = (long) (Math.pow(45,oSchlusselExpo))%oSchlusselMod; 
                rt = rt+berechne+",";
            }
            if(zwischenSpeicher == 'F'){
                berechne = (long) (Math.pow(46,oSchlusselExpo))%oSchlusselMod; 
                rt = rt+berechne+",";
            }
            if(zwischenSpeicher == 'G'){
                berechne = (long) (Math.pow(47,oSchlusselExpo))%oSchlusselMod; 
                rt = rt+berechne+",";
            }
            if(zwischenSpeicher == 'H'){
                berechne = (long) (Math.pow(48,oSchlusselExpo))%oSchlusselMod; 
                rt = rt+berechne+",";
            }
            if(zwischenSpeicher == 'I'){
                berechne = (long) (Math.pow(49,oSchlusselExpo))%oSchlusselMod; 
                rt = rt+berechne+",";
            }
            if(zwischenSpeicher == 'J'){
                berechne = (long) (Math.pow(50,oSchlusselExpo))%oSchlusselMod; 
                rt = rt+berechne+",";
            }
            if(zwischenSpeicher == 'K'){
                berechne = (long) (Math.pow(51,oSchlusselExpo))%oSchlusselMod; 
                rt = rt+berechne+",";
            }
            if(zwischenSpeicher == 'L'){
                berechne = (long) (Math.pow(52,oSchlusselExpo))%oSchlusselMod; 
                rt = rt+berechne+",";
            }
            if(zwischenSpeicher == 'M'){
                berechne = (long) (Math.pow(53,oSchlusselExpo))%oSchlusselMod; 
                rt = rt+berechne+",";
            }
            if(zwischenSpeicher == 'N'){
                berechne = (long) (Math.pow(54,oSchlusselExpo))%oSchlusselMod; 
                rt = rt+berechne+",";
            }
            if(zwischenSpeicher == 'O'){
                berechne = (long) (Math.pow(55,oSchlusselExpo))%oSchlusselMod; 
                rt = rt+berechne+",";
            }
            if(zwischenSpeicher == 'P'){
                berechne = (long) (Math.pow(56,oSchlusselExpo))%oSchlusselMod; 
                rt = rt+berechne+",";
            }
            if(zwischenSpeicher == 'Q'){
                berechne = (long) (Math.pow(57,oSchlusselExpo))%oSchlusselMod; 
                rt = rt+berechne+",";
            }
            if(zwischenSpeicher == 'R'){
                berechne = (long) (Math.pow(58,oSchlusselExpo))%oSchlusselMod; 
                rt = rt+berechne+",";
            }
            if(zwischenSpeicher == 'S'){
                berechne = (long) (Math.pow(59,oSchlusselExpo))%oSchlusselMod; 
                rt = rt+berechne+",";
            }
            if(zwischenSpeicher == 'T'){
                berechne = (long) (Math.pow(60,oSchlusselExpo))%oSchlusselMod; 
                rt = rt+berechne+",";
            }
            if(zwischenSpeicher == 'U'){
                berechne = (long) (Math.pow(61,oSchlusselExpo))%oSchlusselMod; 
                rt = rt+berechne+",";
            }
            if(zwischenSpeicher == 'V'){
                berechne = (long) (Math.pow(62,oSchlusselExpo))%oSchlusselMod; 
                rt = rt+berechne+",";
            }
            if(zwischenSpeicher == 'W'){
                berechne = (long) (Math.pow(63,oSchlusselExpo))%oSchlusselMod; 
                rt = rt+berechne+",";
            }
            if(zwischenSpeicher == 'X'){
                berechne = (long) (Math.pow(64,oSchlusselExpo))%oSchlusselMod; 
                rt = rt+berechne+",";
            }
            if(zwischenSpeicher == 'Y'){
                berechne = (long) (Math.pow(65,oSchlusselExpo))%oSchlusselMod; 
                rt = rt+berechne+",";
            }
            if(zwischenSpeicher == 'Z'){
                berechne = (long) (Math.pow(66,oSchlusselExpo))%oSchlusselMod; 
                rt = rt+berechne+",";
            }
            if(zwischenSpeicher == ' '){
                berechne = (long) (Math.pow(67,oSchlusselExpo))%oSchlusselMod; 
                rt = rt+berechne+",";
            }
            if(zwischenSpeicher == '!'){
                berechne = (long) (Math.pow(68,oSchlusselExpo))%oSchlusselMod; 
                rt = rt+berechne+",";
            
            }
            if(zwischenSpeicher == '?'){
            berechne = (long) (Math.pow(69,oSchlusselExpo))%oSchlusselMod; 
                rt = rt+berechne+",";
            
            }
            if(zwischenSpeicher == '.'){
                berechne = (long) (Math.pow(96,oSchlusselExpo))%oSchlusselMod; 
                rt = rt+berechne+",";
            
            }
            if(zwischenSpeicher == 'a'){
                berechne = (long) (Math.pow(70,oSchlusselExpo))%oSchlusselMod; 
                rt = rt+berechne+",";
            }
            if(zwischenSpeicher == 'b'){
                berechne = (long) (Math.pow(71,oSchlusselExpo))%oSchlusselMod; 
                rt = rt+berechne+",";
            }  
            if(zwischenSpeicher == 'c'){
                berechne = (long) (Math.pow(72,oSchlusselExpo))%oSchlusselMod; 
                rt = rt+berechne+",";
            }
            if(zwischenSpeicher == 'd'){
                berechne = (long) (Math.pow(73,oSchlusselExpo))%oSchlusselMod; 
                rt = rt+berechne+",";
            }
            if(zwischenSpeicher == 'e'){
                berechne = (long) (Math.pow(74,oSchlusselExpo))%oSchlusselMod; 
                rt = rt+berechne+",";
            }
            if(zwischenSpeicher == 'f'){
                berechne = (long) (Math.pow(75,oSchlusselExpo))%oSchlusselMod; 
                rt = rt+berechne+",";
            }
            if(zwischenSpeicher == 'g'){
                berechne = (long) (Math.pow(76,oSchlusselExpo))%oSchlusselMod; 
                rt = rt+berechne+",";
            }
            if(zwischenSpeicher == 'h'){
                berechne = (long) (Math.pow(77,oSchlusselExpo))%oSchlusselMod; 
                rt = rt+berechne+",";
            }
            if(zwischenSpeicher == 'i'){
                berechne = (long) (Math.pow(78,oSchlusselExpo))%oSchlusselMod; 
                rt = rt+berechne+",";
            }
            if(zwischenSpeicher == 'j'){
                berechne = (long) (Math.pow(79,oSchlusselExpo))%oSchlusselMod; 
                rt = rt+berechne+",";
            }
            if(zwischenSpeicher == 'k'){
                berechne = (long) (Math.pow(80,oSchlusselExpo))%oSchlusselMod; 
                rt = rt+berechne+",";
            }
            if(zwischenSpeicher == 'l'){
                berechne = (long) (Math.pow(81,oSchlusselExpo))%oSchlusselMod; 
                rt = rt+berechne+",";
            }
            if(zwischenSpeicher == 'm'){
                berechne = (long) (Math.pow(82,oSchlusselExpo))%oSchlusselMod; 
                rt = rt+berechne+",";
            }
            if(zwischenSpeicher == 'n'){
                berechne = (long) (Math.pow(83,oSchlusselExpo))%oSchlusselMod; 
                rt = rt+berechne+",";
            }
            if(zwischenSpeicher == 'o'){
                berechne = (long) (Math.pow(84,oSchlusselExpo))%oSchlusselMod; 
                rt = rt+berechne+",";
            }
            if(zwischenSpeicher == 'p'){
                berechne = (long) (Math.pow(85,oSchlusselExpo))%oSchlusselMod; 
                rt = rt+berechne+",";
            }
            if(zwischenSpeicher == 'q'){
                berechne = (long) (Math.pow(86,oSchlusselExpo))%oSchlusselMod; 
                rt = rt+berechne+",";
            }
            if(zwischenSpeicher == 'r'){
                berechne = (long) (Math.pow(87,oSchlusselExpo))%oSchlusselMod; 
                rt = rt+berechne+",";
            }
            if(zwischenSpeicher == 's'){
                berechne = (long) (Math.pow(88,oSchlusselExpo))%oSchlusselMod; 
                rt = rt+berechne+",";
            }
            if(zwischenSpeicher == 't'){
                berechne = (long) (Math.pow(89,oSchlusselExpo))%oSchlusselMod; 
                rt = rt+berechne+",";
            }
            if(zwischenSpeicher == 'u'){
                berechne = (long) (Math.pow(90,oSchlusselExpo))%oSchlusselMod; 
                rt = rt+berechne+",";
            }
            if(zwischenSpeicher == 'v'){
                berechne = (long) (Math.pow(91,oSchlusselExpo))%oSchlusselMod; 
                rt = rt+berechne+",";
            }
            if(zwischenSpeicher == 'w'){
                berechne = (long) (Math.pow(92,oSchlusselExpo))%oSchlusselMod; 
                rt = rt+berechne+",";
            }
            if(zwischenSpeicher == 'x'){
                berechne = (long) (Math.pow(93,oSchlusselExpo))%oSchlusselMod; 
                rt = rt+berechne+",";
            }
            if(zwischenSpeicher == 'y'){
                berechne = (long) (Math.pow(94,oSchlusselExpo))%oSchlusselMod; 
                rt = rt+berechne+",";
            }
            if(zwischenSpeicher == 'z'){
                berechne = (long) (Math.pow(95,oSchlusselExpo))%oSchlusselMod; 
                rt = rt+berechne+",";
            }
            if(zwischenSpeicher == '('){
                berechne = (long) (Math.pow(97,oSchlusselExpo))%oSchlusselMod; 
                rt = rt+berechne+",";
            }
            if(zwischenSpeicher == ')'){
                berechne = (long) (Math.pow(98,oSchlusselExpo))%oSchlusselMod; 
                rt = rt+berechne+",";
            }
            if(zwischenSpeicher == ':'){
                berechne = (long) (Math.pow(99,oSchlusselExpo))%oSchlusselMod; 
                rt = rt+berechne+",";
            }
            if(zwischenSpeicher == ';'){
                berechne = (long) (Math.pow(100,oSchlusselExpo))%oSchlusselMod; 
                rt = rt+berechne+",";
            }
            if(zwischenSpeicher == '-'){
                berechne = (long) (Math.pow(101,oSchlusselExpo))%oSchlusselMod; 
                rt = rt+berechne+",";
            }
            if(zwischenSpeicher == '+'){
                berechne = (long) (Math.pow(102,oSchlusselExpo))%oSchlusselMod; 
                rt = rt+berechne+",";
            }
            if(zwischenSpeicher == '*'){
                berechne = (long) (Math.pow(103,oSchlusselExpo))%oSchlusselMod; 
                rt = rt+berechne+",";
            }
            if(zwischenSpeicher == '#'){
                berechne = (long) (Math.pow(105,oSchlusselExpo))%oSchlusselMod; 
                rt = rt+berechne+",";
            }
            nachricht = nachricht.substring(0,nachricht.length());
        }
        
        return rt;
    }

    public void processMessage(String pMessage){
        //Ausgabe der Nachricht und Aufruf von Decodieren
        System.out.println("User 2 Verschlüsselt: "+pMessage);
        System.out.println("User 2: "+this.decode(pMessage));
        
    }

        public String decode(String nachricht){
        entschlusseltText = "";
        
        while(!nachricht.isEmpty()){
            y = nachricht.indexOf(",");
            
            //Entschlüsseln der Nachricht mit dem Privaten Schlüssel
            
            zwischenSpeicher1 = nachricht.substring(0,y);
            nachricht = nachricht.substring(y+1,nachricht.length());
            big = new BigInteger(zwischenSpeicher1);
            big = big.modPow(bigexponent,bigmodulo);
            zwischenSpeicher2 = big.intValue();
               
            //Zuordung der Zahl zu Buchstaben
            
            if(zwischenSpeicher2 == 41){
                entschlusseltText = entschlusseltText+"A";
            }
            if(zwischenSpeicher2 == 42){
                entschlusseltText = entschlusseltText+"B";
            }  
            if(zwischenSpeicher2 == 43){
                entschlusseltText = entschlusseltText+"C";
            }
            if(zwischenSpeicher2 == 44){
                entschlusseltText = entschlusseltText+"D";
            }
            if(zwischenSpeicher2 == 45){
                entschlusseltText = entschlusseltText+"E";
            }
            if(zwischenSpeicher2 == 46){
                entschlusseltText = entschlusseltText+"F";
            }
            if(zwischenSpeicher2 == 47){
                entschlusseltText = entschlusseltText+"G";
            }
            if(zwischenSpeicher2 == 48){
                entschlusseltText = entschlusseltText+"H";
            }
            if(zwischenSpeicher2 == 49){
                entschlusseltText = entschlusseltText+"I";
            }
            if(zwischenSpeicher2 == 50){
                entschlusseltText = entschlusseltText+"J";
            }
            if(zwischenSpeicher2 == 51){
                entschlusseltText = entschlusseltText+"K";
            }
            if(zwischenSpeicher2 == 52){
                entschlusseltText = entschlusseltText+"L";
            }
            if(zwischenSpeicher2 == 53){
                entschlusseltText = entschlusseltText+"M";
            }
            if(zwischenSpeicher2 == 54){
                entschlusseltText = entschlusseltText+"N";
            }
            if(zwischenSpeicher2 == 55){
                entschlusseltText = entschlusseltText+"O";
            }
            if(zwischenSpeicher2 == 56){
                entschlusseltText = entschlusseltText+"P";
            }
            if(zwischenSpeicher2 == 57){
                entschlusseltText = entschlusseltText+"Q";
            }
            if(zwischenSpeicher2 == 58){
                entschlusseltText = entschlusseltText+"R";
            }
            if(zwischenSpeicher2 == 59){
                entschlusseltText = entschlusseltText+"S";
            }
            if(zwischenSpeicher2 == 60){
                entschlusseltText = entschlusseltText+"T";
            }
            if(zwischenSpeicher2 == 61){
                entschlusseltText = entschlusseltText+"U";
            }
            if(zwischenSpeicher2 == 62){
                entschlusseltText = entschlusseltText+"V";
            }
            if(zwischenSpeicher2 == 63){
                entschlusseltText = entschlusseltText+"W";
            }
            if(zwischenSpeicher2 == 64){
                entschlusseltText = entschlusseltText+"X";
            }
            if(zwischenSpeicher2 == 65){
                entschlusseltText = entschlusseltText+"Y";
            }
            if(zwischenSpeicher2 == 66){
                entschlusseltText = entschlusseltText+"Z";
            }
            if(zwischenSpeicher2 == 67){
                entschlusseltText = entschlusseltText+" ";
            }
            if(zwischenSpeicher2 == 68){
                entschlusseltText = entschlusseltText+"!";
            }
            if(zwischenSpeicher2 == 69){
                entschlusseltText = entschlusseltText+"?";
            }
            if(zwischenSpeicher2 == 96){
                entschlusseltText = entschlusseltText+".";
            }
            if(zwischenSpeicher2 == 70){
                entschlusseltText = entschlusseltText+"a";
            }
            if(zwischenSpeicher2 == 71){
                entschlusseltText = entschlusseltText+"b";
            }  
            if(zwischenSpeicher2 == 72){
                entschlusseltText = entschlusseltText+"c";
            }
            if(zwischenSpeicher2 == 73){
                entschlusseltText = entschlusseltText+"d";
            }
            if(zwischenSpeicher2 == 74){
                entschlusseltText = entschlusseltText+"e";
            }
            if(zwischenSpeicher2 == 75){
                entschlusseltText = entschlusseltText+"f";
            }
            if(zwischenSpeicher2 == 76){
                entschlusseltText = entschlusseltText+"g";
            }
            if(zwischenSpeicher2 == 77){
                entschlusseltText = entschlusseltText+"h";
            }
            if(zwischenSpeicher2 == 78){
                entschlusseltText = entschlusseltText+"i";
            }
            if(zwischenSpeicher2 == 79){
                entschlusseltText = entschlusseltText+"j";
            }
            if(zwischenSpeicher2 == 80){
                entschlusseltText = entschlusseltText+"k";
            }
            if(zwischenSpeicher2 == 81){
                entschlusseltText = entschlusseltText+"l";
            }
            if(zwischenSpeicher2 == 82){
                entschlusseltText = entschlusseltText+"m";
            }
            if(zwischenSpeicher2 == 83){
                entschlusseltText = entschlusseltText+"n";
            }
            if(zwischenSpeicher2 == 84){
                entschlusseltText = entschlusseltText+"o";
            }
            if(zwischenSpeicher2 == 85){
                entschlusseltText = entschlusseltText+"p";
            }
            if(zwischenSpeicher2 == 86){
                entschlusseltText = entschlusseltText+"q";
            }
            if(zwischenSpeicher2 == 87){
                entschlusseltText = entschlusseltText+"r";
            }
            if(zwischenSpeicher2 == 88){
                entschlusseltText = entschlusseltText+"s";
            }
            if(zwischenSpeicher2 == 89){
                entschlusseltText = entschlusseltText+"t";
            }
            if(zwischenSpeicher2 == 90){
                entschlusseltText = entschlusseltText+"u";
            }
            if(zwischenSpeicher2 == 91){
                entschlusseltText = entschlusseltText+"v";
            }
            if(zwischenSpeicher2 == 92){
                entschlusseltText = entschlusseltText+"w";
            }
            if(zwischenSpeicher2 == 93){
                entschlusseltText = entschlusseltText+"x";
            }
            if(zwischenSpeicher2 == 94){
                entschlusseltText = entschlusseltText+"y";
            }
            if(zwischenSpeicher2 == 95){
                entschlusseltText = entschlusseltText+"z";
            }
            if(zwischenSpeicher2 == 97){
                entschlusseltText = entschlusseltText+"(";
            }
            if(zwischenSpeicher2 == 98){
                entschlusseltText = entschlusseltText+")";
            }
            if(zwischenSpeicher2 == 99){
                entschlusseltText = entschlusseltText+":";
            }
            if(zwischenSpeicher2 == 100){
                entschlusseltText = entschlusseltText+";";
            }
            if(zwischenSpeicher2 == 101){
                entschlusseltText = entschlusseltText+"-";
            }
            if(zwischenSpeicher2 == 102){
                entschlusseltText = entschlusseltText+"+";
            }
            if(zwischenSpeicher2 == 103){
                entschlusseltText = entschlusseltText+"*";
            }
            if(zwischenSpeicher2 == 105){
                entschlusseltText = entschlusseltText+"#";
            }
        }
        
        return entschlusseltText;
    }
    
}
