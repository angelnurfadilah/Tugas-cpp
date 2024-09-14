#include <iostream>
using namespace std;

int main() {
	
    char tipeRumah;
	char jenisPembayaran;
	
    int hargaTunai;
	int hargaPerbulan;
	int totalHargaRumah;

    cout << "Masukkan Tipe Rumah (A/B/C/D): ";
    cin >> tipeRumah;
    
    cout << "Masukkan Jenis Pembayaran (T untuk Tunai, K untuk Kredit): ";
    cin >> jenisPembayaran;
	
	if( tipeRumah == 'A' || tipeRumah == 'a')
	{
		hargaTunai = 50000000;
		hargaPerbulan = 500000;
	}
	
	else if( tipeRumah == 'B' || tipeRumah == 'b')
	{
		hargaTunai = 75000000;
		hargaPerbulan = 750000;
	}
		
	else if( tipeRumah == 'C' || tipeRumah == 'c')
	{
		hargaTunai = 85000000;
		hargaPerbulan = 850000;
	}
		
	else if( tipeRumah == 'd' || tipeRumah == 'D')
	{
		hargaTunai = 100000000;
		hargaPerbulan = 1000000;
	}	
	else
	{
		cout << "Tipe Rumah tidak ada" << endl;
	}

    if (jenisPembayaran == 't' || jenisPembayaran == 'T')
	{
        totalHargaRumah = hargaTunai;
    }
    
	else if (jenisPembayaran == 'K'|| jenisPembayaran == 'k') 
	{
        totalHargaRumah = 12 * hargaPerbulan * 10;
   		cout << "Angsuran Perbulan: Rp " << hargaPerbulan << endl;
    }
    
	else
	{
        cout << "Jenis Pembayaran tidak ada!" << endl;
        return 1;
    }

    cout << "Total Harga Rumah: Rp " << totalHargaRumah << endl;

    return 0;
}
