# Escrevendo-as-Classes-de-Um-Jogo
class Heroi:
    def __init__(self, nome, idade, tipo):
        self.nome = nome  
        self.idade = idade  
        self.tipo = tipo 

    def atacar(self):
        if self.tipo == 'mago':
            ataque = 'usou magia'
        elif self.tipo == 'guerreiro':
            ataque = 'usou espada'
        elif self.tipo == 'monge':
            ataque = 'usou artes marciais'
        elif self.tipo == 'ninja':
            ataque = 'usou shuriken'
        else:
            ataque = 'ataque desconhecido'
        print(f"o {self.tipo} atacou usando {ataque}")

# Criando um objeto da classe Heroi
heroi = Heroi('Junior', 35, 'ninja')

# Usando o método atacar
heroi.atacar()
