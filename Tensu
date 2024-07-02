#include <iostream>
#include <fstream>
#include <algorithm>
//#include <vector>
using namespace std;

int main(){
    ifstream file("sample.txt");
    if(!file){
        cerr<<"!CAN NOT OPEN THE FILE!"<<endl;
        return 0;
    }
    int F[30]={0}; //ファイルの初期化
    int num;
    
    //ファイルから数字を読み込み
    while(file >> num){
        if(num >= 1 && num <= 30){
            F[num - 1] = 1; //提出された番号を1にする
        }
    }
    file.close();
    
    bool shuseki = true;
    for(int i=1; i<28; ++i){
        if(F[i]==0){
            cout<<(i+1)<<endl;
        }
    }
    return 0;
}
