# MAQUINA-DE-REFRI-
print("MAQUINA REFRI DRINK")
quantidadeCoca=10
quantidadePepsi=10
quantidadeKaut=10
quantidadeGuarana=10
quantidadeFanta=10

refriCoca=3.00
refriPepsi=3.00
refriKaut=3.00
refriGuarana=3.00
refriFanta=3.00
sairSair=3
while sairSair!=1:
    print("MAQUINA REFRI DRINK")
    print("(1) COCA COLA R$3.00 ")
    print("(2) PEPSI R$3.00")
    print("(3) KAUT R$3.00")
    print("(4) GUARANÁ R$3.00")
    print("(5)FANTA UVA R$3.00")
    escolhaProduto=int(input("ESCOLHA O NÚMERO DO PRODUTO DESEJADO ="))
    if escolhaProduto == 4321:
        print("OLÁ ADMINISTRADOR")
        print(" (1) COCA COLA",quantidadeCoca,"UNIDADES")
        print(" (2) PEPSI",quantidadePepsi,"UNIDADES")
        print("(3) KAUT",quantidadeKaut,"UNIDADES")
        print("(4) GUARANÁ ",quantidadeGuarana,"UNIDADES")
        print("(5) FANTA UVA",quantidadeFanta,"UNIDADES")
        cocaCola=1
        pepsiPepsi=2
        kautKaut=3
        guaranaGuarana=4
        fantaFanta=5
        quantidadeSomarproduto=int(input("Qual produto deseja acrescentar? =  "))
        if quantidadeSomarproduto == 1:
            acrescentarCoca=int(input("Quantos produtos deseja acrescentar para Coca Cola?  ="))
            quantidadeCoca=quantidadeCoca+acrescentarCoca
            print("TOTAL DE COCA COLA",quantidadeCoca,"UNIDADES")
        if quantidadeSomarproduto == 2:
            acrescentarPepsi=int(input("Quantos produtos deseja acrescentar para PEPSI?  ="))
            quantidadePepsi=quantidadePepsi+acrescentarPepsi
            print("TOTAL DE PEPSI",quantidadePepsi,"UNIDADES")
        if quantidadeSomarproduto == 3:
            acrescentarKaut=int(input("Quantos produtos deseja acrescentar para KAUT?  ="))
            quantidadeKaut=quantidadeKaut+acrescentarKaut
            print("TOTAL DE KAUT",quantidadeKaut,"UNIDADES")
        if quantidadeSomarproduto == 4:
            acrescentarGuarana=int(input("Quantos produtos deseja acrescentar para GUARANÁ?  ="))
            quantidadeGuarana=quantidadeGuarana+acrescentarGuarana
            print("TOTAL DE GUARANÁ",quantidadeGuarana,"UNIDADES")
        if quantidadeSomarproduto == 5:
            acrescentarFanta=int(input("Quantos produtos deseja acrescentar para FANTA UVA?  ="))
            quantidadeFanta=quantidadeFanta+acrescentarFanta
            print("TOTAL DE FANTA",quantidadeFanta,"UNIDADES")
        
    if escolhaProduto == 1:
        print("Coloque o valor a pagar ")
        valorPagarcoca=float(input("R$ "))
        if valorPagarcoca<refriCoca:
            print("Saldo insuficiente")
            faltamValor1=(refriCoca-valorPagarcoca)
            print("Falta R$",faltamValor1)
            dinheiroFalta=int(input("Deseja inserir Mais dinheiro? (1)SIM 2(NÃO)"))
            if dinheiroFalta==1:
                dinherioRestante=float(input("R$ "))
                if dinherioRestante==faltamValor1:
                    print("Pagamento com Sucesso")
                    print("REFRI COCA COLA SENDO ENTREGUE")
                    quantidadeCoca = quantidadeCoca - 1
                    print("Restam", quantidadeCoca, "Unidades")
            else:
                print("CANCELANDO COMPRA")
                print("DEVOLVENDO DINHEIRO")
                
        if valorPagarcoca==refriCoca:
            print("REFRI COCA COLA SENDO ENTREGUE")
            quantidadeCoca=quantidadeCoca-1
            print("Restam",quantidadeCoca,"Unidades")
        elif valorPagarcoca>refriCoca:
            valorTroco=(valorPagarcoca-refriCoca)
            print("TROCO =",valorTroco)
            print("REFRI COCA COLA SENDO ENTREGUE")
            quantidadeCoca = quantidadeCoca - 1
            print("Restam", quantidadeCoca, "Unidades")
    if escolhaProduto == 2:
        print("Coloque o valor a pagar ")
        valorPagarcoca=float(input("R$ "))
        if valorPagarcoca<refriPepsi:
            print("Saldo insuficiente")
            faltamValor1=(refriPepsi-valorPagarcoca)
            print("Falta R$",faltamValor1)
            dinheiroFalta=int(input("Deseja inserir Mais dinheiro? (1)SIM 2(NÃO)"))
            if dinheiroFalta==1:
                dinherioRestante=float(input("R$ "))
                if dinherioRestante==faltamValor1:
                    print("Pagamento com Sucesso")
                    print("REFRI PEPSI SENDO ENTREGUE")
                    quantidadePepsi = quantidadePepsi - 1
                    print("Restam", quantidadePepsi, "Unidades")
            else:
                print("CANCELANDO COMPRA")
                print("DEVOLVENDO DINHEIRO")
                
        if valorPagarcoca==refriPepsi:
            print("REFRI PEPSI SENDO ENTREGUE")
            quantidadePepsi = quantidadePepsi - 1
            print("Restam", quantidadePepsi, "Unidades")
        elif valorPagarcoca>refriPepsi:
            valorTroco=(valorPagarcoca-refriPepsi)
            print("TROCO =",valorTroco)
            print("REFRI PEPSI SENDO ENTREGUE")
            quantidadePepsi = quantidadePepsi - 1
            print("Restam", quantidadePepsi, "Unidades")   
            
        
