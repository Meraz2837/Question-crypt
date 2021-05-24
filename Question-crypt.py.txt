class Node:
    def __init__(self, dataval=None):

        self.dataval = dataval

        self.nextval = None



class SLinkedList:

    def __init__(self):

        self.headval = None



    def listprint(self):

        printval = self.headval

        while printval is not None:

            print (printval.dataval)

            printval = printval.nextval



def List():

    list = SLinkedList()

    list.headval = Node("1. Dhaka")

    e2 = Node("2. Chattogram")

    e3 = Node("3. Rajshahi")

    e4 = Node("4. Dinajpur")

    e5 = Node("5. Jashor")

    e6 = Node("6. Cumilla")

    e7 = Node("7. Sylhet")

    e8 = Node("8. Mymensingh")

    e9 = Node("9. Barishal")

    

    list.headval.nextval = e2



    e2.nextval = e3

    e3.nextval = e4

    e4.nextval = e5

    e5.nextval = e6

    e6.nextval = e7

    e7.nextval = e8

    e8.nextval = e9



    list.listprint()





def Dhaka():

    qdhaka = Encrypt()

    print("Question after encription: ",qdhaka)

    return qdhaka

    

def Chattogram():

    qchattogram = Encrypt()

    print("Question after encription: ",qchattogram)

    return qchattogram



def Rajshahi():

    qrajshahi = Encrypt()

    print("Question after encription: ",qrajshahi)

    return qrajshahi



def Dinajpur():

    qdinajpur = Encrypt()

    print("Question after encription: ",qdinajpur)

    return qdinajpur



def Jashor():

    qjashor = Encrypt()

    print("Question after encription: ",qjashor)

    return qjashor



def Cumilla():

    qcumilla = Encrypt()

    print("Question after encription: ",qcumilla)

    return qcumilla



def Sylhet():

    qsylhet = Encrypt()

    print("Question after encription: ",qsylhet)

    return qsylhet



def Mymensingh():

    qmymensingh = Encrypt()

    print("Question after encription: ",qmymensingh)

    return qmymensingh



def Barishal():

    qbarishal = Encrypt()

    print("Question after encription: ",qbarishal)

    return qbarishal





def bod():

    global count2

    global count3

    print("-------------------------------------------------")

    print("\t\tBoard of Director")

    print("-------------------------------------------------")

    

    print("Log in first")

    print("================")

    username = str(input("UserName: "))

    password = str(input("PassWord: "))

    print("================")

    if username == "dhaka" and password == "2854":

        

        print("\n\nSelect Board")

        print("----------------")

        List()

        print("----------------")

        select = int(input("Select by number: "))

        if select == 1:

            print("------------------------------------------")

            print("\tWelcome to Dhaka board")

            print("------------------------------------------")

            Dhaka()

            print("\n\n1. Previous page\n2. Home\n3. Exit")

            sel = int(input("Select by number: "))

            if sel == 1:

                bod()

            elif sel == 2:

                main()

            else:

                exit()

        elif select == 2:

            print("------------------------------------------")

            print("\tWelcome to Chattogram board")

            print("------------------------------------------")

            Chattogram()

            print("\n\n1. Previous page\n2. Home\n3. Exit")

            sel = int(input("Select by number: "))

            if sel == 1:

                bod()

            elif sel == 2:

                main()

            else:

                exit()

        elif select == 3:

            print("------------------------------------------")

            print("\tWelcome to Rajshahi board")

            print("------------------------------------------")

            Rajshahi()

            print("\n\n1. Previous page\n2. Exit")

            sel = int(input("Select by number: "))

            if sel == 1:

                bod()

            else:

                exit()

        elif select == 4:

            print("------------------------------------------")

            print("\tWelcome to Dinajpur board")

            print("------------------------------------------")

            Dinajpur()

            print("\n\n1. Previous page\n2. Home\n3. Exit")

            sel = int(input("Select by number: "))

            if sel == 1:

                bod()

            elif sel == 2:

                main()

            else:

                exit()

        elif select == 5:

            print("------------------------------------------")

            print("\tWelcome to Jashor board")

            print("------------------------------------------")

            Jashor()

            print("\n\n1. Previous page\n2. Exit")

            sel = int(input("Select by number: "))

            if sel == 1:

                bod()

            else:

                exit()

        elif select == 6:

            print("------------------------------------------")

            print("\tWelcome to Cumilla board")

            print("------------------------------------------")

            Cumilla()

            print("\n\n1. Previous page\n2. Home\n3. Exit")

            sel = int(input("Select by number: "))

            if sel == 1:

                bod()

            elif sel == 2:

                main()

            else:

                exit()

        elif select == 7:

            print("------------------------------------------")

            print("\tWelcome to Sylhet board")

            print("------------------------------------------")

            Sylhet()

            print("\n\n1. Previous page\n2. Exit")

            sel = int(input("Select by number: "))

            if sel == 1:

                bod()

            else:

                exit()

        elif select == 8:

            print("------------------------------------------")

            print("\tWelcome to Mymensingh board")

            print("------------------------------------------")

            Mymensingh()

            print("\n\n1. Previous page\n2. Home\n3. Exit")

            sel = int(input("Select by number: "))

            if sel == 1:

                bod()

            elif sel == 2:

                main()

            else:

                exit()

        elif select == 9:

            print("------------------------------------------")

            print("\tWelcome to Barishal board")

            print("------------------------------------------")

            Barishal()

            print("\n\n1. Previous page\n2. Home\n3. Exit")

            sel = int(input("Select by number: "))

            if sel == 1:

                bod()

            elif sel == 2:

                main()

            else:

                exit()

    else:

        print("***Wrong Password***")

        print(count3,"Times left")

        count2+=1

        count3-=1

        if count2 == 4:

            print("\nAccess terminated for too many wrong information\n3")

            exit()

        else:

            bod()

    

def moe():

    global count4

    global count5

    print("-------------------------------------------------")

    print("\t\tMinistry of Education")

    print("-------------------------------------------------")

    print("Log in first")

    print("================")

    username = str(input("UserName: "))

    password = str(input("PassWord: "))

    print("================")

    if username == "moe" and password == "2847":

        print("----------------")

        List()

        print("----------------")

        select = int(input("Select by number: "))

        if select == 1:

            print("------------------------------------------")

            print("\tWelcome to Dhaka board")

            print("------------------------------------------")

            print("********For more security you will have to login again********")

            Decrypt()

            print("\n\n1. Previous page\n2. Home\n3. Exit")

            sel = int(input("Select by number: "))

            if sel == 1:

                moe()

            elif sel == 2:

                main()

            else:

                exit()

            

        elif select == 2:

            print("------------------------------------------")

            print("\tWelcome to Chattogram board")

            print("------------------------------------------")

            

            print("********For more security you will have to login again********")

            Decrypt()

            print("\n\n1. Previous page\n2. Home\n3. Exit")

            sel = int(input("Select by number: "))

            if sel == 1:

                moe()

            elif sel == 2:

                main()

            else:

                exit()

        elif select == 3:

            print("------------------------------------------")

            print("\tWelcome to Rajshahi board")

            print("------------------------------------------")

            print("********For more security you will have to login again********")

            Decrypt()

            print("\n\n1. Previous page\n2. Home\n3. Exit")

            sel = int(input("Select by number: "))

            if sel == 1:

                moe()

            elif sel == 2:

                main()

            else:

                exit()

        elif select == 4:

            print("------------------------------------------")

            print("\tWelcome to Dinajpur board")

            print("------------------------------------------")

            print("********For more security you will have to login again********")

            Decrypt()

            print("\n\n1. Previous page\n2. Home\n3. Exit")

            sel = int(input("Select by number: "))

            if sel == 1:

                moe()

            elif sel == 2:

                main()

            else:

                exit()

        elif select == 5:

            print("------------------------------------------")

            print("\tWelcome to Jashor board")

            print("------------------------------------------")

            print("********For more security you will have to login again********")

            Decrypt()

            print("\n\n1. Previous page\n2. Home\n3. Exit")

            sel = int(input("Select by number: "))

            if sel == 1:

                moe()

            elif sel == 2:

                main()

            else:

                exit()

        elif select == 6:

            print("------------------------------------------")

            print("\tWelcome to Cumilla board")

            print("------------------------------------------")

            print("********For more security you will have to login again********")

            Decrypt()

            print("\n\n1. Previous page\n2. Home\n3. Exit")

            sel = int(input("Select by number: "))

            if sel == 1:

                moe()

            elif sel == 2:

                main()

            else:

                exit()

        elif select == 7:

            print("------------------------------------------")

            print("\tWelcome to Sylhet board")

            print("------------------------------------------")

            print("********For more security you will have to login again********")

            Decrypt()

            print("\n\n1. Previous page\n2. Home\n3. Exit")

            sel = int(input("Select by number: "))

            if sel == 1:

                moe()

            elif sel == 2:

                main()

            else:

                exit()

        elif select == 8:

            print("------------------------------------------")

            print("\tWelcome to Mymensingh board")

            print("------------------------------------------")

            print("********For more security you will have to login again********")

            Decrypt()

            print("\n\n1. Previous page\n2. Home\n3. Exit")

            sel = int(input("Select by number: "))

            if sel == 1:

                moe()

            elif sel == 2:

                main()

            else:

                exit()

        elif select == 9:

            print("------------------------------------------")

            print("\tWelcome to Barishal board")

            print("------------------------------------------")

            print("********For more security you will have to login again********")

            Decrypt()

            print("\n\n1. Previous page\n2. Home\n3. Exit")

            sel = int(input("Select by number: "))

            if sel == 1:

                moe()

            elif sel == 2:

                main()

            else:

                exit()

    else:

        print("***Wrong Password***")

        print(count5,"Times left")

        count4+=1

        count5-=1

        if count4 == 4:

            print("\nAccess terminated for too many wrong information\n3")

            exit()

        else:

            moe()



def hoc():

    global count6

    global count7

    print("-------------------------------------------------")

    print("\t\tHead of Center")

    print("-------------------------------------------------")

    print("Log in first")

    print("================")

    username = str(input("UserName: "))

    password = str(input("PassWord: "))

    print("================")

    if username == "hoc" and password == "2861":

        print("----------------")

        List()

        print("----------------")

        select = int(input("Select by number: "))

        if select == 1:

            print("------------------------------------------")

            print("\tWelcome to Dhaka board")

            print("------------------------------------------")

            print("********For more security you will have to login again********")

            Decrypt()

            print("Dhaka board's question deccrypted")

            print("\n\n1. Previous page\n2. Home\n3. Exit")

            sel = int(input("Select by number: "))

            if sel == 1:

                hoc()

            elif sel == 2:

                main()

            else:



                exit()

        elif select == 2:

            print("------------------------------------------")

            print("\tWelcome to Chattogram board")

            print("------------------------------------------")

            print("********For more security you will have to login again********")

            Decrypt()

            print("Chattogram's board's question deccrypted")

            print("\n\n1. Previous page\n2. Home\n3. Exit")

            sel = int(input("Select by number: "))

            if sel == 1:

                hoc()

            elif sel == 2:

                main()

            else:

                exit()

        elif select == 3:

            print("------------------------------------------")

            print("\tWelcome to Rajshahi board")

            print("------------------------------------------")

            print("********For more security you will have to login again********")

            Decrypt()

            print("Rajshahi board's question deccrypted")

            print("\n\n1. Previous page\n2. Home\n3. Exit")

            sel = int(input("Select by number: "))

            if sel == 1:

                hoc()

            elif sel == 2:

                main()

            else:

                exit()

        elif select == 4:

            print("------------------------------------------")

            print("\tWelcome to Dinajpur board")

            print("------------------------------------------")

            print("********For more security you will have to login again********")

            Decrypt()

            print("Dinajpur board's question deccrypted")

            print("\n\n1. Previous page\n2. Home\n3. Exit")

            sel = int(input("Select by number: "))

            if sel == 1:

                hoc()

            elif sel == 2:

                main()

            else:

                exit()

        elif select == 5:

            print("------------------------------------------")

            print("\tWelcome to Jashor board")

            print("------------------------------------------")

            print("********For more security you will have to login again********")

            Decrypt()

            print("Jashor board's question deccrypted")

            print("\n\n1. Previous page\n2. Home\n3. Exit")

            sel = int(input("Select by number: "))

            if sel == 1:

                hoc()

            elif sel == 2:

                main()

            else:

                exit()

        elif select == 6:

            print("------------------------------------------")

            print("\tWelcome to Cumilla board")

            print("------------------------------------------")

            print("********For more security you will have to login again********")

            Decrypt()

            print("Cumilla board's question deccrypted")

            print("\n\n1. Previous page\n2. Home\n3. Exit")

            sel = int(input("Select by number: "))

            if sel == 1:

                hoc()

            elif sel == 2:

                main()

            else:

                exit()

        elif select == 7:

            print("------------------------------------------")

            print("\tWelcome to Sylhet board")

            print("------------------------------------------")

            print("********For more security you will have to login again********")

            Decrypt()

            print("Sylhet board's question deccrypted")

            print("\n\n1. Previous page\n2. Home\n3. Exit")

            sel = int(input("Select by number: "))

            if sel == 1:

                hoc()

            elif sel == 2:

                main()

            else:

                exit()

        elif select == 8:

            print("------------------------------------------")

            print("\tWelcome to Mymensingh board")

            print("------------------------------------------")

            print("********For more security you will have to login again********")

            Decrypt()

            print("Mymensingh board's question deccrypted")

            print("\n\n1. Previous page\n2. Home\n3. Exit")

            sel = int(input("Select by number: "))

            if sel == 1:

                hoc()

            elif sel == 2:

                main()

            else:

                exit()

        elif select == 9:

            print("------------------------------------------")

            print("\tWelcome to Barishal board")

            print("------------------------------------------")

            print("********For more security you will have to login again********")

            Decrypt()

            print("Barishal board's question deccrypted")

            print("\n\n1. Previous page\n2. Home\n3. Exit")

            sel = int(input("Select by number: "))

            if sel == 1:

                hoc()

            elif sel == 2:

                main()

            else:

                exit()



    else:

        print("***Wrong Password***")

        print(count7,"Times left")

        count6+=1

        count7-=1

        if count6 == 4:

            print("\nAccess terminated for too many wrong information\n3")

            exit()

        else:

            hoc()

        



def Encrypt():

    question1 = str(input("Please Type Question: "))

    alphabets = 'A!B@C#D$E%F^G&H*I(J)K_L+M-N~O`P/Q1RSTUVWXYZa2b3c4d?5.,><|:;{}[]e6f7g8h9 ijklmnopqrstuvwxyz'



    encrypt = ''

    for i in question1:

        position = alphabets.find(i)

        newposition = (position + 5)%90

        encrypt+=alphabets[newposition]

    return encrypt

    

    



def Decrypt():



    global count

    global count1

    print("Login first to access question")

    print("\nEnter the UserName and Password given from board")

    print("================")



    username = str(input("UserName: "))

    password = str(input("PassWord: "))

    print("================")

    if username == "DECRYPT" and password == "2837":

        question1 = str(input("Please paste the Encrypted Question: "))

        alphabets = 'A!B@C#D$E%F^G&H*I(J)K_L+M-N~O`P/Q1RSTUVWXYZa2b3c4d?5.,><|:;{}[]e6f7g8h9 ijklmnopqrstuvwxyz3'



        encrypt = ''

        for i in question1:

            position = alphabets.find(i)

            newposition = (position - 5) % 90

            encrypt += alphabets[newposition]

        print("Encrypted Question: ", encrypt)

    else:

        print("***Wrong Password***")

        print(count1,"Times left")

        count+=1

        count1-=1

        if count == 4:

            print("\nAccess terminated for too many wrong information\n3")

            exit()

        else:

            Decrypt()





def main():

    print("\t\t------------------------------------")

    print("\t\t Welcome to digital question system ")

    print("\t\t------------------------------------")

    option = int(input("Log in as\n1. Board of Director\n2. Ministry of education\n3. Head of center\n4. About us\nEnter Number: "))

    if option == 1:

        

        bod()

    elif option == 2:

        

        moe()

        

    elif option == 3:

        

        hoc()

    elif option == 4:

        about_us()

    else:

        exit()





def about_us():

    print("\n\nMd. Mazbaur Rashid")

    print("CEO & Founder")

    print("Facebook: facebook.com/mezbah.meraz\n\n")

    print("Tawhid Ahmed Komol")

    print("Co-Developer")

    print("Facebook: facebook.com/towhid.komol\n\n")

    print("Shariar Kabir Nayeem")

    print("Idea Developer")

    print("Facebook: facebook.com/profile.php?id=100006494299107\n\n")

    print("Sabbir Hossain")

    print("Co-Designer")

    print("Facebook: facebook.com/sabbirto13\n\n")

    print("Md. Sabbir Alam")

    print("Editor")

    print("Facebook: facebook.com/profile.php?id=100010042142996\n\n")

    print("Nazmus Sakib Tanim")

    print("Designer")

    print("Facebook: facebook.com/tanim.khan.395017\n")

    print("\n\nMore details available on Google Site")





count2 = 0

count3 = 3

count4 = 0

count5 = 3

count6 = 0

count7 = 3

count = 0

count1 = 3

main()

