/******************************************************************************

Welcome to GDB Online.
GDB online is an online compiler and debugger tool for C, C++, Python, Java, PHP, Ruby, Perl,
C#, OCaml, VB, Swift, Pascal, Fortran, Haskell, Objective-C, Assembly, HTML, CSS, JS, SQLite, Prolog.
Code, Compile, Run and Debug online from anywhere in world.

*******************************************************************************/
#include <iostream>
#include <string>
using namespace std;

class Drone {
private:
	int hiz;
	int yuk;
	int yukseklik;
	int pil;
public:
	Drone( int yk, int h, int y, int p) {
		hiz=h;
		yuk=yk;
		yukseklik= y;
		pil=p;
	}
	string ucusGuvenligiKontrol() {
		pil -= (hiz / 10) * 5;

		if (yuk > 500) {
			return "Agir yuk, ucamaz!";
		} else if (pil < 30) {
			return "Pil seviyesi dusuk, ucus guvensiz!";
		} else if (yukseklik < 20) {
			return "Yukseklik guvensiz, ucus guvensiz!";
		} else if (yukseklik > 200) {
			return "Radar disi, ucus guvensiz!";
		} else {
			return "Ucus guvenli! Kalan pil: %" + to_string(pil);
		}
	}
	void setYuk(int yeniYuk) {
		yuk = yeniYuk;
	}
	~Drone() {
		cout<<endl <<"Yikici fonk. calisti";
	}
};

int main()
{
	Drone d1(350, 40, 50, 100);
	Drone d2(600, 30, 70, 100);
	Drone d3(100, 160, 180, 100);

	cout << "Drone 1: " << d1.ucusGuvenligiKontrol() << endl;
	cout << "Drone 2: " << d2.ucusGuvenligiKontrol() << endl;
	cout << "Drone 3: " << d3.ucusGuvenligiKontrol() << endl;
	return 0;
}
