import qrcode
print ('''  _______    _______    _          _______               _______ 
 (       )  (  ___  )  ( (    /|  (  ____ \  |\     /|  (  ____ )
 | () () |  | (   ) |  |  \  ( |  | (    \/  | )   ( |  | (    )|
 | || || |  | (___) |  |   \ | |  | (_____   | |   | |  | (____)|
 | |(_)| |  |  ___  |  | (\ \) |  (_____  )  | |   | |  |     __)
 | |   | |  | (   ) |  | | \   |        ) |  | |   | |  | (\ (   
 | )   ( |  | )   ( |  | )  \  |  /\____) |  | (___) |  | ) \ \__
 |/     \|  |/     \|  |/    )_)  \_______)  (_______)  |/   \__/
                                                                 

''')
text = input("ссылка = ")
img  = qrcode.make(text)
name = input("название вашего файла =  ")
img.save(name)
print("QR-код сгенерирован успешно\n" + "ссылка : " + text +  "\n названия : " + "name"
