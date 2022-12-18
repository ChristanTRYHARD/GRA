# GRA

import random
HP = 150
name = input('podaj ksywe:')
umięśnienie = int(input('oceń swoje umięśnienie od 0 do 100:'))
if umięśnienie < 25:
    print('HA, słabeusz')
elif 25 < umięśnienie < 50:
    print('nie jest najgorzej')
else:
    print('wow')
while 150 >= HP > 0:
    a = 2
    print('atakuje cię', a, "goblinów po 50HP")
    print('1 - lewy prosty(30dm), 2 - lewy podbródkowy(200dm)')
    odp1 = int(input('>'))
    
    if odp1 == 1:
        HP = HP - a*12
        if HP <= 0:
            break
        print("Jeden z", a, 'goblinów ma zaledwie 20hp, niefortunnie zostałeś również draśnięty')
        
        

        print('zostało Ci', HP,'hp')
        print('Trzeba ich dokończyć')
        print('1 - unik, lewy prosty(35dm)      3 - prężysz muskuły licząc na to że się przestraszą')
        odp2 = int(input('>'))
        
        if odp2 == 1:
            HP = HP - a*4
            if HP <= 0:
                break
            print('Udał ci się unik, rozwalileś goblinka jeszcze', a - 1)
            print('dzięki unikowi straciłeś tylko', a*4, 'HP')
            
            
            print('twoje HP =', HP )
            a = a - 1
        if odp2 == 3:
            HP = HP - a*35
            if HP <= 0:
                break
            print("dostajesz srogi wperwdol")
            
            
            print('twoje HP = ',HP,'HP')
            print('gobliny myślaly że jesteś martwy i uciekły, jeden z nich został żeby się upewnić')
            a = 1
            
            
        if a == 1:
            print('Ostatni lamus do bicia')
            print('1 - Uduszenie (999dm)    2 - kopniak w jaja(120dm)')
            odp3 = int(input('>'))
            if odp3 == 1:
                HP = HP - a*18
                if HP <= 0:
                    break
                print('goblinek dusząc cię poważnie podrapał ci twarz')
                
                
                print('zostało ci', HP, 'hp')
                print('idziesz przez las')
                HP = HP + 200
            elif odp3 == 2:
                print('Nawet cie nie drasnoł')
                print('essa win')
                HP = HP + 200
                    
        if a == 2:
            print("pora na kombinacje")
            print('1 - dwa szybkie sierpy(2*80dm)   2 - zwód, potęzny prawy prosty(120dm) i lewy hak na dół(100dm)')
            odp4 = int(input('>'))
                
            if odp4 == 1:
                HP = HP - a*12
                if HP <= 0:
                    break
                print('Dobra robota')
                
                
                print('twoje HP = ',HP,'HP')
                print('idziesz dalej')
                HP = HP + 200
            elif odp4 == 2:
                HP = HP - a*6
                if HP <= 0:
                    break
                print('jesteś niesamowity dzięki twojemu zwodowi uniknołeś 2 poważne ciosy')
                
                
                print('twoje HP = ',HP,'HP')
                print('idziesz dalej')
                HP = HP + 200
                    
        if a == 3:
            print('Zostało ci', a,'zawodników')
            print(' 1 - ojcowski liść(200dm),    2 - prędki lewy w zemby (50dm)')
            odp5 = int(input('>'))
                   
            if odp5 == 1:
                HP = HP - a*20
                if HP <= 0:
                    break
                print('Cios nie doszedł, dostałeś w zęby')
                
                
                print('twoje HP = ',HP,'HP')
                print('1 - ostateczne zniszczenie    2 - cios w pysk z całej siły')
                odp6 = int(input(">"))
                if odp6 == 1:
                    HP = HP - a*20
                    if HP <= 0:
                        break
                    print('bierzesz jednego za noge, przy okazji poważnie dostajesz w ryja, machasz nim i zabijasz pozostałych')
                    
                    print('twoje HP = ',HP,'HP')
                    print('dumnym krokiem idziesz dalej')
                    HP = HP + 200
                           
                if odp6 == 2:
                    HP = HP - a*10
                    if HP <= 0:
                        break
                    print("Uśpiłeś chama")
                    
                    
                    print('Lekko cie drasnoł, jak zwykle :)')
                    print('twoje HP = ',HP,'HP')
                    print("pora na kombinacje")
                    print('1 - dwa szybkie sierpy(2*80dm)   2 - zwód, potęzny prawy prosty(120dm) i lewy hak na dół(100dm)')
                    odp7 = int(input(">"))
                    if odp7 == 1:
                        HP = HP - a*12
                        if HP <= 0:
                            break
                        print('Dobra robota')
                        
                        
                        print('twoje HP = ',HP,'HP')
                        print('idziesz dalej')
                        HP = HP + 200
                    elif odp7 == 2:
                        HP = HP - a*16
                        if HP <= 0:
                            break
                        print('jesteś niesamowity dzięki twojemu zwodowi uniknołeś 2 poważne ciosy')
                        
                        print('twoje HP = ',HP,'HP')
                        print('idziesz dalej')
                        HP = HP + 200
            if odp5 == 2:
                print('dzięki potwornej sile wybuchasz mu czache')
                print('robota nie skończona')
                print('1 - ostateczne zniszczenie    2 - cios w pysk z całej siły')
                odp6 = int(input(">"))
                       
                if odp6 == 1:
                    HP = HP - a*20
                    if HP <= 0:
                            break
                    print('bierzesz jednego za noge, przy okazji poważnie dostajesz w ryja, machasz nim i zabijasz pozostałych')
                    
                    
                    print('twoje HP = ',HP,'HP')
                    print('dumnym krokiem idziesz dalej')
                    HP = HP + 200
                           
                if odp6 == 2:
                    HP = HP - a*10
                    if HP <= 0:
                        break
                    print("Uśpiłeś chama")
                    
                    print('Lekko cie drasnoł, jak zwykle :)')
                    print('twoje HP = ',HP,'HP')
                    print("pora na kombinacje")
                    print('1 - dwa szybkie sierpy(2*80dm)   2 - zwód, potęzny prawy prosty(120dm) i lewy hak na dół(100dm)')
                    odp7 = int(input(">"))
                    if odp7 == 1:
                        HP = HP - a*12
                        if HP <= 0:
                            break
                        print('Dobra robota')
                        
                        
                        print('twoje HP = ',HP,'HP')
                        print('idziesz dalej')
                        HP = HP + 200
                    elif odp7 == 2:
                        HP = HP - a*10
                        if HP <= 0:
                            break
                        print('jesteś niesamowity dzięki twojemu zwodowi uniknołeś 2 poważne ciosy')
                        
                        
                        print('twoje HP = ',HP,'HP')
                        print('idziesz dalej')
                        HP = HP + 200
    elif odp1 == 2:
        print('Znokałtowałeś jednego z', a, 'goblinów, jeszcze tylko',a -1)
        print("Nie wyszedłeś bez szfanku, twoje HP =",HP - a*3)
        a = a - 1
        
        if a == 1:
            print('Ostatni lamus do bicia')
            print('1 - Uduszenie (999dm)    2 - kopniak w jaja(120dm)')
            odp3 = int(input('>'))
            if odp3 == 1:
                HP = HP - a*18
                if HP <= 0:
                    break
                print('goblinek dusząc cię poważnie podrapał ci twarz')
                
                
                
                print('zostało ci', HP, 'hp')
                print('idziesz przez las')
            elif odp3 == 2:
                print('Nawet cie nie drasnoł')
                print('essa win, spacerujesz')
                HP = HP + 200
                
        if a == 2:
            print("pora na kombinacje")
            print('1 - dwa szybkie sierpy(2*80dm)   2 - zwód, potęzny prawy prosty(120dm) i lewy hak na dół(100dm)')
            odp4 = int(input('>'))
                
            if odp4 == 1:
                HP = HP - a*12
                if HP <= 0:
                    break
                print('Dobra robota')
                
                
                
                print('twoje HP = ',HP,'HP')
                print('idziesz dalej')
                HP = HP + 200
            elif odp4 == 2:
                HP = HP - a*9
                if HP <= 0:
                    break
                print('jesteś niesamowity dzięki twojemu zwodowi uniknołeś 2 poważne ciosy')
                
               
                print('twoje HP = ',HP,'HP')
                print('idziesz dalej')
                HP = HP + 200
                    
        if a == 3:
            print('Zostało ci', a,'zawodników')
            print(' 1 - ojcowski liść(200dm),    2 - prędki lewy w zemby (50dm)')
            odp5 = int(input('>'))
                   
            if odp5 == 1:
                HP = HP - a*20
                if HP <= 0:
                    break
                print('Cios nie doszedł, dostałeś w zęby')
                
                
                print('twoje HP = ',HP,'HP')
                print('1 - ostateczne zniszczenie    2 - cios w pysk z całej siły')
                odp6 = int(input(">"))
                if odp6 == 1:
                    HP = HP - a*20
                    if HP <= 0:
                        break
                    print('bierzesz jednego za noge, przy okazji poważnie dostajesz w ryja, machasz nim i zabijasz pozostałych')
                    
                    
                    print('twoje HP = ',HP,'HP')
                    print('dumnym krokiem idziesz dalej')
                    HP = HP + 200
                           
                if odp6 == 2:
                    HP = HP - a*13
                    if HP <= 0:
                        break
                    print("Uśpiłeś chama")
                    
                    
                    print('Lekko cie drasnoł, jak zwykle :)')
                    print('twoje HP = ',HP,'HP')
                    print("pora na kombinacje")
                    print('1 - dwa szybkie sierpy(2*80dm)   2 - zwód, potęzny prawy prosty(120dm) i lewy hak na dół(100dm)')
                    odp7 = int(input(">"))
                    if odp7 == 1:
                        HP = HP - a*15
                        if HP <= 0:
                            break
                        print('Dobra robota')
                        
                        
                        print('twoje HP = ',HP,'HP')
                        print('idziesz dalej')
                        HP = HP + 200
                    elif odp7 == 2:
                        HP = HP - a*9
                        if HP <= 0:
                            break
                        print('jesteś niesamowity dzięki twojemu zwodowi uniknołeś 2 poważne ciosy')
                        
                        
                       
                        print('twoje HP = ',HP,'HP')
                        print('idziesz dalej')
                        HP = HP + 200
                        break
print(50*'-')
if HP <= 0:
    print("hi hi hi hA!")
    print("umarłeś")
    print('koniec')
else:
    print('wygrałeś')
