print("MAQUINA REFRI DRINK")
quantidadeCoca=0
quantidadePepsi=10
quantidadeKaut=10
quantidadeGuarana=10
quantidadeFanta=10
lucroRefricoca=0
lucroRefripepsi=0
lucroRefrikaut=0
lucroRefriguarana=0
lucroRefriFanta=0
refriCoca=3.00
refriPepsi=7.00
refriKaut=3.00
refriGuarana=5.00
refriFanta=3.00
sairSair=3
while sairSair!=1:
    print("MAQUINA REFRI DRINK")
    print("(1) COCA COLA 350 ml ---------- R$3.00")
    print("(2) PEPSI 1l ------------------ R$7.00")
    print("(3) KAUT 350 ml --------------- R$3.00")
    print("(4) GUARANÁ 500 ml ------------ R$5.00")
    print("(5)FANTA UVA 350 ml ------------R$3.00")
    escolhaProduto=int(input("ESCOLHA O NÚMERO DO PRODUTO DESEJADO ="))
    if escolhaProduto == 4321:
        print("OLÁ ADMINISTRADOR")
        print(" (1) COCA COLA",quantidadeCoca,"UNIDADES")
        print(" (2) PEPSI",quantidadePepsi,"UNIDADES")
        print(" (3) KAUT",quantidadeKaut,"UNIDADES")
        print(" (4) GUARANÁ ",quantidadeGuarana,"UNIDADES")
        print(" (5) FANTA UVA",quantidadeFanta,"UNIDADES")
        print("--------------------------------------------")
        totalProdutos=(quantidadeCoca+quantidadePepsi+quantidadeKaut+quantidadeGuarana+quantidadeFanta)
        totalVendidoscoca=(lucroRefricoca/3)
        totalVendidospepsi=(lucroRefripepsi/7)
        totalVendidoskaut=(lucroRefrikaut/3)
        totalVendidosguarana=(lucroRefriguarana/5)
        totalVendidosfanta=(lucroRefriFanta/3)
        print("TOTAL DE PRODUTOS = ",totalProdutos,"UNIDADES")
        print("---------------------------------------------")
        print("VALOR VENDIDO DE COCA COLA ", lucroRefricoca,"REAIS ------- FORAM VENDIDOS --- ",totalVendidoscoca,"UNIDADES")
        print("VALOR VENDIDO DE PEPSI ", lucroRefripepsi,"REAIS ---------- FORAM VENDIDOS --- ",totalVendidospepsi,"UNIDADES")
        print("VALOR VENDIDO DE KAUT ", lucroRefrikaut,"REAIS -------------FORAM VENDIDOS --- ",totalVendidoskaut,"UNIDADES")
        print("VALOR VENDIDO DE GUARANÁ ", lucroRefriguarana,"REAIS -------FORAM VENDIDOS --- ",totalVendidosguarana,"UNIDADES")
        print("VALOR VENDIDO DE FANTA UVA ", lucroRefriFanta,"REAIS -------FORAM VENDIDOS --- ",totalVendidosfanta,"UNIDADES")
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
                    lucroRefricoca=lucroRefricoca+refriCoca
                    
            else:
                print("CANCELANDO COMPRA")
                print("DEVOLVENDO DINHEIRO")
                
        if valorPagarcoca==refriCoca:
            print("REFRI COCA COLA SENDO ENTREGUE")
            quantidadeCoca=quantidadeCoca-1
            print("Restam",quantidadeCoca,"Unidades")
            lucroRefricoca=lucroRefricoca+refriCoca
        elif valorPagarcoca>refriCoca:
            valorTroco=(valorPagarcoca-refriCoca)
            print("TROCO =",valorTroco)
            print("REFRI COCA COLA SENDO ENTREGUE")
            quantidadeCoca = quantidadeCoca - 1
            print("Restam", quantidadeCoca, "Unidades")
            lucroRefricoca=lucroRefricoca+refriCoca
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
                    lucroRefripepsi=lucroRefripepsi+refriPepsi
            else:
                print("CANCELANDO COMPRA")
                print("DEVOLVENDO DINHEIRO")
                
        if valorPagarcoca==refriPepsi:
            print("REFRI PEPSI SENDO ENTREGUE")
            quantidadePepsi = quantidadePepsi - 1
            print("Restam", quantidadePepsi, "Unidades")
            lucroRefripepsi=lucroRefripepsi+refriPepsi
        elif valorPagarcoca>refriPepsi:
            valorTroco=(valorPagarcoca-refriPepsi)
            print("TROCO =",valorTroco)
            print("REFRI PEPSI SENDO ENTREGUE")
            quantidadePepsi = quantidadePepsi - 1
            print("Restam", quantidadePepsi, "Unidades")
            lucroRefripepsi=lucroRefripepsi+refriPepsi
    if escolhaProduto == 3 :
        print("Coloque o valor a pagar ")
        valorPagarcoca=float(input("R$ "))
        if valorPagarcoca<refriKaut:
            print("Saldo insuficiente")
            faltamValor1=(refriKaut-valorPagarcoca)
            print("Falta R$",faltamValor1)
            dinheiroFalta=int(input("Deseja inserir Mais dinheiro? (1)SIM 2(NÃO)"))
            if dinheiroFalta==1:
                dinherioRestante=float(input("R$ "))
                if dinherioRestante==faltamValor1:
                    print("Pagamento com Sucesso")
                    print("REFRI KAUT SENDO ENTREGUE")
                    quantidadeKaut = quantidadeKaut - 1
                    print("Restam", quantidadeKaut, "Unidades")
                    lucroRefrikaut=lucroRefrikaut+refriKaut
            else:
                print("CANCELANDO COMPRA")
                print("DEVOLVENDO DINHEIRO")
                
        if valorPagarcoca==refriKaut:
            print("REFRI KAUT SENDO ENTREGUE")
            quantidadeKaut = quantidadeKaut - 1
            print("Restam", quantidadeKaut, "Unidades")
            lucroRefrikaut=lucroRefrikaut+refriKaut
        elif valorPagarcoca>refriKaut:
            valorTroco=(valorPagarcoca-refriKaut)
            print("TROCO =",valorTroco)
            print("REFRI KAUT SENDO ENTREGUE")
            quantidadeKaut = quantidadeKaut - 1
            print("Restam", quantidadeKaut, "Unidades") 
            lucroRefrikaut=lucroRefrikaut+refriKaut
    if escolhaProduto==4:
        print("Coloque o valor a pagar ")
        valorPagarcoca=float(input("R$ "))
        if valorPagarcoca<refriGuarana:
            print("Saldo insuficiente")
            faltamValor1=(refriGuarana-valorPagarcoca)
            print("Falta R$",faltamValor1)
            dinheiroFalta=int(input("Deseja inserir Mais dinheiro? (1)SIM 2(NÃO)"))
            if dinheiroFalta==1:
                dinherioRestante=float(input("R$ "))
                if dinherioRestante==faltamValor1:
                    print("Pagamento com Sucesso")
                    print("REFRI GUARANÁ SENDO ENTREGUE")
                    quantidadeGuarana = quantidadeGuarana - 1
                    print("Restam", quantidadeGuarana, "Unidades")
                    lucroRefriguarana=lucroRefriguarana+refriGuarana
            else:
                print("CANCELANDO COMPRA")
                print("DEVOLVENDO DINHEIRO")
                
        if valorPagarcoca==refriPepsi:
            print("REFRI GUARANÁ SENDO ENTREGUE")
            quantidadeGuarana = quantidadeGuarana - 1
            print("Restam", quantidadeGuarana, "Unidades")
            lucroRefriguarana=lucroRefriguarana+refriGuarana
        elif valorPagarcoca>refriGuarana:
            valorTroco=(valorPagarcoca-refriGuarana)
            print("TROCO =",valorTroco)
            print("REFRI GUARANÁ SENDO ENTREGUE")
            quantidadeGuarana = quantidadeGuarana - 1
            print("Restam", quantidadeGuarana, "Unidades")
            lucroRefriguarana=lucroRefriguarana+refriGuarana
    if escolhaProduto==5:
        print("Coloque o valor a pagar ")
        valorPagarcoca=float(input("R$ "))
        if valorPagarcoca<refriFanta:
            print("Saldo insuficiente")
            faltamValor1=(refriFanta-valorPagarcoca)
            print("Falta R$",faltamValor1)
            dinheiroFalta=int(input("Deseja inserir Mais dinheiro? (1)SIM 2(NÃO)"))
            if dinheiroFalta==1:
                dinherioRestante=float(input("R$ "))
                if dinherioRestante==faltamValor1:
                    print("Pagamento com Sucesso")
                    print("REFRI FANTA UVA SENDO ENTREGUE")
                    quantidadeFanta = quantidadeFanta - 1
                    print("Restam", quantidadeFanta, "Unidades")
                    lucroRefriFanta=lucroRefriFanta+refriFanta
            else:
                print("CANCELANDO COMPRA")
                print("DEVOLVENDO DINHEIRO")
                
        if valorPagarcoca==refriFanta:
            print("REFRI FANTA UVA SENDO ENTREGUE")
            quantidadeFanta = quantidadeFanta - 1
            print("Restam", quantidadeFanta, "Unidades")
            lucroRefriFanta=lucroRefriFanta+refriFanta
        elif valorPagarcoca>refriFanta:
            valorTroco=(valorPagarcoca-refriFanta)
            print("TROCO =",valorTroco)
            print("REFRI FANTA UVA SENDO ENTREGUE")
            quantidadeFanta = quantidadeFanta - 1
            print("Restam", quantidadeFanta, "Unidades")
            lucroRefriFanta=lucroRefriFanta+refriFanta
            
        
