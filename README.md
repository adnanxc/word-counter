# word-counter

#include <iostream>
using namespace std;

int wordcounter (string a){
    int ctr = 1 , length = a.length();
    for(int i=0; i<length; i++){
        if(a[i]==' '){
            ctr++;
        }
    }
    return ctr;
}




int main(){
    string s;
    cout << "Enter your string: ";
    getline(cin,s);

    cout << "Number of words: " << wordcounter(s);
}
