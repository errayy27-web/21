# S17 kontrol raporu

TAMAM (kaynak kod): uygulama açılınca ve her 3 saniyede bir /shared senkronizasyonu, /snapshot ürün-stok-fiyat, /sales, /daily-sales ve /kasa otomatik okuma. Yerel PC adresi önce denenir, sonra varsa genel Bulut API adresi denenir. Ekranlara ve Kasa hesaplama fonksiyonuna dokunulmadı.

EKSİK: Supabase URL + anon key tek başına bir /snapshot, /shared API sağlamaz; bulut için güvenli PC köprüsü ve Supabase veri şeması kurulmalıdır. Sipariş/barkod hatası/fotoğraf/KOM-PAK merkezi senkronizasyonu eksiktir. /shared yalnızca desteklenen alanları taşır.

UYARI: 3 saniyelik zamanlayıcı, istekler ağ gecikmesi nedeniyle sürerken yeni bir tur başlatmaz. Tüm cihazlarda 3 saniye içinde sonuç garantisi değildir. APK derlenmedi, gerçek PC/telefon testi yapılmadı.
