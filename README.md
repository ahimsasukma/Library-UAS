# Library-UAS
Untuk tugas UAS mata kuliah Pemrograman
#include<iostream> // menampilkan perintah cout, cin, endl
#include<conio.h> // menampilkan perintah getch, clrscr
#include<string> // untuk atribut-atribut class

using namespace std;

class buku{ //sebagai sebuah class
	public:
		//atribut-atribut yang ada
		string jurusan;
		string kelas;
		string mapel;
		string semester;
};

int main(){
	cout<<"==========================================="<<endl;  
	cout<<"		LIBRARY	"<<endl;  //judul
	cout<<"==========================================="<<endl;  
		
	int Search; //untuk berapa kali input data (berupa angka)
	
	buku buku; //sebagai sebuah object
	
	cout<<"Search: ";
	cin>>Search;
	
	for(int i=0;i<Search;i++){ //input bisa satu kali atau lebih
		cin.ignore(); //mengabaikan enter
		cout<<"Jurusan		: ";getline(cin,buku.jurusan);
		cout<<"Kelas		: ";getline(cin,buku.kelas);
		//getline untuk membaca input dalan 1 baris
		cout<<"Mapel		: ";cin>>buku.mapel;
		cout<<"Semester		: ";cin>>buku.semester;
		
		//menmpilkan hasil
		cout<<buku.jurusan<<endl;
		cout<<buku.kelas<<endl;
		cout<<buku.mapel<<endl;
		cout<<buku.semester<<endl;
		cout<<""<<endl;  
	}

	getche();
}

// Nama : Ahimsa Sukma Pamungkas
// Nim : 17.11.1536
// Prodi : S1 – Informatika
