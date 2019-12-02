
#include<bits/stdc++.h> 
using namespace std; 
  

int value(char r) 
{ 
    if (r == 'I') 
        return 1; 
    if (r == 'V') 
        return 5; 
    if (r == 'X') 
        return 10; 
    if (r == 'L') 
        return 50; 
    if (r == 'C') 
        return 100; 
    if (r == 'D') 
        return 500; 
    if (r == 'M') 
        return 1000; 
  
    return -1; 
} 
  

int romanToDecimal(string &str) 
{ 
   
    int res = 0; 
  
   
    for (int i=0; i<str.length(); i++) 
    { 
        int s1 = value(str[i]); 
  
        if (i+1 < str.length()) 
        { 
            
            int s2 = value(str[i+1]); 
  
           
            if (s1 >= s2) 
            { 
               
                res = res + s1; 
            } 
            else
            { 
                res = res + s2 - s1; 
                i++; 
            } 
        } 
        else
        { 
            res = res + s1; 
             
        } 
    } 
    return res; 
} 
  
 
int main() 
{ 
    
    string str ="MCMIV"; 
    cout << "ROMAN RAKAMININ SAYI OLARAK KARÞILIÐI "
         << romanToDecimal(str) << endl; 
  
    return 0; 
} 

#include <bits/stdc++.h> 
using namespace std; 
  

string intToRoman(int num)  
{    
    
     string m[] = {"", "M", "MM", "MMM"}; 
     string c[] = {"", "C", "CC", "CCC", "CD", "D",  
                        "DC", "DCC", "DCCC", "CM"}; 
     string x[] = {"", "X", "XX", "XXX", "XL", "L",  
                        "LX", "LXX", "LXXX", "XC"}; 
     string i[] = {"", "I", "II", "III", "IV", "V",  
                        "VI", "VII", "VIII", "IX"}; 
          
     string binler = m[num/1000]; 
     string yüzler = c[(num%1000)/100]; 
     string onlar =  x[(num%100)/10]; 
     string birler = i[num%10]; 
          
     string ans = binler + yüzler + onlar + birler;
          
     return ans; 
} 
  

int main() 
{ 
      int number = 3549; 
      cout << intToRoman(number); 
      return 0; 


} 

//kaynaklar:
//https://yazilimsihirbazi.wordpress.com/2013/05/07/c-programlama-dili-roma-rakamlari-islemleri/
//https://www.geeksforgeeks.org
