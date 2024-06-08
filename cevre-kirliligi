import discord
from discord.ext import commands
import os

intents = discord.Intents.default()
intents.message_content = True
bot = commands.Bot(command_prefix="!", intents=intents)

@bot.event
async def on_ready():
    print(f"{bot.user} discord'a giriş yaptı!")

@bot.command()
async def merhaba(ctx):
    await ctx.send("Merhaba, Çevre kirliliği hakkında bilgi almak ister misin?")

@bot.command()
async def evet(ctx):
    await ctx.send("Çevrenin canlı ögelerinin hayat aktivitelerini olumsuz yönde etkileyen, cansız ögelerin üzerinde ise yapısal zararlar meydana getiren ve niteliklerini bozan yabancı maddelerin hava, su ve toprağa yoğun bir şekilde karışması olayına çevre kirliliği denir. Hızla artan insan nüfusu ihtiyaçları arttırmakta, insan eliyle yaratılan kirliliğin tabiata ve çevreye verdiği zararın boyutu her geçen gün artmaktadır. Yaşamı daha mükemmel bir hale getirmek, daha sağlıklı ve uzun bir ömür sağlayabilmek amacına dönük bazı gelişmelerin, kırsal ve kentsel alanlarda doğal kaynaklarını bozduğu, su, hava, toprak kirlenmesine yol açtığı, bitki ve hayvan varlığına ve sağlığına zarar verdiği açıkça görülebilen bir gerçek haline gelmiştir. Hangi çeşitten bilgi almak istersin? (su/hava/toprak/ses/ışık)")

@bot.command()
async def hayır(ctx):
    await ctx.send("NE DEMEK HAYIR! TEKRAR DÜŞÜN!")

@bot.command()
async def su(ctx):
    await ctx.send("Su kirliliği, istenmeyen zararlı maddelerin, suyun niteliğini ölçülebilecek oranda bozmalarını sağlayacak miktar ve yoğunlukta suya karışma olayıdır. Konutlar, endüstri kuruluşları, termik santraller, gübreler, kimyasal mücadele ilaçları (pestisitler), tarımsal sanayi atık suları, nükleer santrallerden çıkan sıcak sular ve toprak erozyonu gibi süreçler ve maddeler su kirliliğini meydana getiren başlıca kaynaklardır. Bunların hepsi doğrudan doğruya veya dolaylı olarak canlı ve cansız varlıklara zarar vermektedir.")

    with open('images/su.jpg', 'rb') as f:
        picture = discord.File(f)
    await ctx.send(file = picture)

@bot.command()
async def hava(ctx):
    await ctx.send("Atmosferde duman, toz ve saf olmayan su buharı şeklinde bulunabilecek kirleticilerin, insanlar ve diğer canlılar ile eşyaya zarar verebilecek miktarlara yükselmesi Hava kirliliği olarak nitelenmektedir. Havayı kirleten maddelerin sınır değerleri (havada zararlı olmayacak derecedeki en yüksek değerleri), her ülkenin ilgili kuruluşları tarafından yönetmeliklerle belirlenir. Kirletici maddelerin niteliğine göre, canlılara vereceği zarar şekil ve dereceleri de değişir. Hava kirliliğine karşı alınabilecek önlemler, kirlilik kaynağına göre (fabrika, termik santral, konutlar, taşıt araçları) çok çeşitlidir. Bu önlemler başta eğitim alınmak üzere teknik, hukuksal önlemler olmak üzere başlıca 3 grupta toplanabilir. Birçok ülkenin hava kirliliğinin sınırı vardır fakat gelişmiş ülkeler bu sınırı aşmakta ve aşmaya devam ediyor.")

    with open('images/hava.jpg', 'rb') as f:
        picture = discord.File(f)
    await ctx.send(file = picture)

@bot.command()
async def toprak(ctx):
    await ctx.send("Toprağın kimyasal maddelerle veya atıklarla kirlenmesidir. Toprak kirlenmesi, hava ve suları kirleten maddeler tarafından meydana getirilebilir. Örneğin, kükürt dioksit oranı yüksek olan bir atmosfer tabakasından geçen yağmur damlacıkları asit yağmuru hâlinde toprağa geçer. Toprak içine giren bu asitli sular ağaç köklerini, bitkisel ve hayvansal toprak canlılarını zarara uğratır. Toprağın reaksiyonunu etkileyerek besin maddesi dengesini bozar, yeraltı sularını içilmez hâle getirir. Aynı şekilde çöp yığınlarından toprağa sızan sular, kirli sulama suları, gübre çözeltileri, radyoaktif maddeler, uçucu küller, ağır metaller, kükürt dioksit sanayi atıkları toprağı kirleten madde ve kaynaklardır.")

    with open('images/toprak.jpg', 'rb') as f:
        picture = discord.File(f)
    await ctx.send(file = picture)

@bot.command()
async def ses(ctx):
    await ctx.send("Yoğun şehir yaşamında özellikle insanların istirahat vakitlerinde yayılan motorlu araç, makina sesleri, inşaat, eğlence, bazı dinî-sosyal aktiviteler, maçlar ses kirliliğini oluşturan bazı gürültü kaynaklarına örnek olarak verilebilir. Ses kirliliğinden dolayı insanlar ve hayvanlar rahatsız olur. Bu nedenle fabrikalar, hava alanları vb. mekanları şehirden uzak yerlere yapılmalıdır.")

    with open('images/ses.jpg', 'rb') as f:
        picture = discord.File(f)
    await ctx.send(file = picture)

@bot.command()
async def ışık(ctx):
    await ctx.send("Işık kirliliğinin sebepleri lazerler ve gereksiz aydınlatmalardır. Işık kirliliği gece havada aşırı aydınlık oluşmasıdır. Aşırı aydınlık canlılara zarar vermektedir. Örneğin;Deniz kaplumbağaları yumurtadan çıktıklarında denizin üzerindeki Ay yansımasını ararlar ama aşırı aydınlatmalardan dolayı bir kısmı ayın yansımasını ayırt edemez sonuç olarak açlıktan veya avlanmaktan dolayı ölürler.Kuşlar uçarken aya göre yön bulurlar. Ama aşırı aydınlatmalardan dolayı hangisinin ay olduğunu bilemezler ve göç edemeyip ölürler.Gereksiz aydınlatmanın diğer etkileri:Yeryüzündeki teleskoplar gök cisimlerini gözlemleyemez.")

    with open('images/ışık.jpg', 'rb') as f:
        picture = discord.File(f)
    await ctx.send(file = picture)

bot.run("BOT TOKEN")
