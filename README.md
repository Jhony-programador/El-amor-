import time 

Dicionario = {
    "Melisa": {
      "Edad": "20",
      "Pais": "Nicaragua",
      "Ciudad": "Esteli",
      "Amiga": "Anyi"   
      },
      "Solanyi": {
      "Edad2": "17",
      "pais": "Nicaragua ",
      "Ciudad": "Matagalpa",
      "Amigo": "Elder"
        },
       "Katherine": {
       "Edad3": "15",
       "Ciudad": "Chinandega",
       "Amiga": "Esther"
       }
       	
}
while True:
    Data = input("\n\033[043mInicia tu búsqueda👀:\033[0m ").capitalize()
    if Data == "Salir":
        print("----------------🔥-------------------")
        print("! \033[041mSaliendo con estilo 🔥.       🧠!\033[0m")
        print("-----------------🧠-----------------")
        break
    if Data in Dicionario:
        print(f"\033[041m]Informacion sobre {Data}\n\033[0m")
        time.sleep(1)
        for clave, valor in  Dicionario[Data].items():
            for letra in f"{clave}: {valor}\n":
                print(letra,end=" ", flush=True)
                time.sleep(0.05)   
        print(f"\n \033[045m]Desearia guardar la informacion de {Data}\033[0m]")
    else:
        print(f"\033[031m]El nombre de {Data} no se encontro\033[0m]")
        
    
