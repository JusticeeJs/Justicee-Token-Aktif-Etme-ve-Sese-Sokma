Bu projenin amacı nedir?
Projenin amacı birden fazla hesabı tek bir proje ile aktif edip sese sokmaktır.
Şöyle örnek vereyim x1,x2,x3,x4 ve x5 adın da hesaplarınız var.
Ve sunucunuzda sese sokmak istiyorsun.
Öncelikle justicee.js kanalından login kısmına hesap tokenlerinizi girmeniz gerekiyor.
1 den fazla token girmek için const,login ve voice kısmını çoğaltın.
Çoğaltmanın örneği de şu şekilde 

const justicee1= new Discord.Client();
const justicee2= new Discord.Client();

justicee1.login("token")
justicee2.login("token")

justicee1.on("ready", () => {justicee1.channels.cache.get(process.env.ses).join()})
justicee2.on("ready", () => {justicee2.channels.cache.get(process.env.ses).join()})

Bu şekilde ne kadar hesabınız varsa aktif edip sese sokabilirsiniz
