def data():
    phone_number= (input('Enter phone_num\n\t>>> '))
    if len(phone_number) == 11 and phone_number.isnumeric():
        dailyplan_others(phone_number)
    else:
        print(
            'Invalid phone number\n'
            'Try again\n'
        )
        data()
def data1():
    phone_number= (input('Enter phone_num\n\t>>> '))
    if len(phone_number) == 11 and phone_number.isnumeric():
        weeklyplan1(phone_number)
    else:
        print(
            'Invalid phone number\n'
            'Try again\n'
        )
        data1()

def data2():
    phone_number= (input('Enter phone_num\n\t>>> '))
    if len(phone_number) == 11 and phone_number.isnumeric():
        monthlyplan1(phone_number)
    else:
        print(
            'Invalid phone number\n'
            'Try again\n'
        )
        data2()
def data3():
    phone_number= (input('Enter phone_num\n\t>>> '))
    if len(phone_number) == 11 and phone_number.isnumeric():
        monthsplan1(phone_number)
    else:
        print(
            'Invalid phone number\n'
            'Try again\n'
        )
        data3()

def data4():
    phone_number= (input('Enter phone_num\n\t>>> '))
    if len(phone_number) == 11 and phone_number.isnumeric():
      yearplan1(phone_number)
    else:
        print(
            'Invalid phone number\n'
            'Try again\n'
        )
        data4()

def yearplan1(x):
    PLAN = input('SELECT OPTIONS\n\n'
                 '1> 400GB (90 DAYS) FOR N50000.00\n'
                 '2> 500GB (120 DAYS) FOR N600000.00\n'

                 '>>>'
                 )

    if PLAN == '1':
        print(f'confirm purchase of 400GB (90 DAYS) FOR N50000.00 to {x}')
        confam_data()
    elif PLAN == '2':
        print(f'confirm purchase of 500GB (120 DAYS) FOR N600000.00 to {x} ')
        confam_data()
    else:
        print('error unsupported')
        select_data_plans()

def monthsplan1(x):
    plan = input('SELECT OPTION\n'
                 '1> 400GB (90 DAYS) FOR N50000\n'

                 '>>>'

                 )
    if plan == '1':
        print(f'confirm purchase of 400GB (90 DAYS) FOR N50000.00 to {x}')
        confam_data()
    else:
        monthsplan1(x)


def moreplan3a(x):
    PLAN = input('SELECT OPTIONS\n\n'
                 '1> 240GB (30 DAYS) FOR N30000.00\n'
                 '2> 280GB (30 DAYS) FOR N360000.00\n'
                 '3> Back\n'

                 '>>>'
                 )
    if PLAN == '1':
        print(f'confirm purchase of 240GB (30 DAYS) FOR N30000.00 to {x} ')
        confam_data()
    elif PLAN == '2':
        print(f'confirm purchase of 280GB (30 DAYS) FOR N360000.00 to {x}')
        confam_data()
    elif PLAN == '3':
        moreplan2a(x)


    else:
        print('wrong input')
        moreplan3a(x)


def moreplan2a(x):
    PLAN = input('SELECT OPTIONS\n\n'
                 '1> 30GB (30 DAYS) FOR N8000.00\n'
                 '2> 40GB (30 DAYS) FOR N10000.00\n'
                 '3> 75GB (30 DAYS) FOR N15000.00\n'
                 '4> 120GB (30 DAYS) FOR N20000.00\n'
                 '5> next page\n'
                 '6> back\n'

                 '>>>'
                 )
    if PLAN == '1':
        print(f'confirm purchase of 30GB (30 DAYS) FOR N8000.00 to {x} ')
        confam_data()
    elif PLAN == '2':
        print(f'confirm purchase of 40GB (30 DAYS) FOR N10000.00  to {x}')
        confam_data()
    elif PLAN == '3':
        print(f'confirm purchase of 75GB (30 DAYS) FOR N15000.00 to {x} ')
        confam_data()
    elif PLAN == '4':
        print(f'confirm purchase of 120GB (30 DAYS) FOR N20000.00 to {x}')
        confam_data()
    elif PLAN == '5':
        moreplan3a(x)
    elif PLAN == '6':
        moreplan1a(x)

    else:
        print('wrong input')
        moreplan2a(x)


def moreplan1a(x):
    PLAN = input('SELECT OPTIONS\n\n'
                 '1> 6GB (30 DAYS) FOR N2500.00\n'
                 '2> 10GB (30 DAYS) FOR N3000.00\n'
                 '3> 15GB (30 DAYS) FOR N4000.00\n'
                 '4> 18GB (30 DAYS) FOR N5000.00\n'
                 '5> next page\n'
                 '6> back\n'

                 '>>>'
                 )
    if PLAN == '1':
        print(f'confirm purchase of 6GB (30 DAYS) FOR N2500.00 to {x} ')
        confam_data()
    elif PLAN == '2':
        print(f'confirm purchase of 10GB (30 DAYS) FOR N3000.00 to {x} ')
        confam_data()
    elif PLAN == '3':
        print(f'confirm purchase of 15GB (30 DAYS) FOR N4000.00 to {x} ')
        confam_data()
    elif PLAN == '4':
        print(f'confirm purchase of 18GB (30 DAYS) FOR N5000.00 to {x} ')
        confam_data()
    elif PLAN == '5':
        moreplan2a(x)
    elif PLAN == '6':
        monthlyplan1(x)

    else:
        print('wrong input')
        moreplan1a(x)


def monthlyplan1(x):
    PLAN = input('SELECT OPTIONS\n\n'
                 '1> 1.2GB (30 DAYS) FOR N1000.00\n'
                 '2> 1.5GB (30 DAYS) FOR N1200.00\n'
                 '3> 3GB (30 DAYS) FOR N1500.00\n'
                 '4> 4.5GB (30 DAYS) FOR N2000.00\n'
                 '5> next page\n'
                 '>>>'
                 )
    if PLAN == '1':
        print(f'confirm purchase of 1.2GB (30 DAYS) FOR N1000.00 to {x} ')
        confam_data()
    elif PLAN == '2':
        print(f'confirm purchase of 1.5GB (30 DAYS) FOR N1200.00 to {x} ')
        confam_data()
    elif PLAN == '3':
        print(f'confirm purchase of 3GB (30 DAYS) FOR N1500.00 to {x} ')
        confam_data()
    elif PLAN == '4':
        print(f'confirm purchase of 4.5GB (30 DAYS) FOR N2000.00 to {x} ')
        confam_data()
    elif PLAN == '5':
        moreplan1a(x)
    else:
        print('wrong input')
        monthlyplan1(x)


def weeklyplan1(x):
    PLAN = input('SELECT OPTIONS\n\n'
                 '1> 350MB (7 DAYS) FOR N350.00\n'
                 '2> 750MB (7 DAYS) FOR N500.00\n'
                 '3> 5GB (7 DAYS) FOR N1500.00\n'

                 '>>>'
                 )
    if PLAN == '1':
        print(f'confirm purchase of 350MB (7 DAYS) FOR N350.00 to {x} ')
        confam_data()
    elif PLAN == '2':
        print(f'confirm purchase of 750MB (7 DAYS) FOR N500.00 to {x} ')
        confam_data()
    elif PLAN == '3':
        print(f'confirm purchase of 5GB (7 DAYS) FOR N1500.00 to {x}')
        confam_data()

    else:
        print('wrong input')
        weeklyplan1(x)


def moreplans(x):
    more=input( '1> 500MB (1 DAY) FOR N350.00\n'
                '2> 350MB (1 DAY) FOR N300.00\n'
                '3> 2.5GB (3 DAY) FOR N800.00\n'
                '4> 2.5MB (1 DAY) FOR N500.00\n'
                '5> Back\n'
                '>>>'
                )
    if more == '1':
        print(f'confirm purchase of 500MB (1 DAY) FOR N350.00 to {x}')
        confam_data()
    elif more == '2':
        print(f'confirm purchase of 350MB (1 DAY) FOR N300.00 to {x}')
        confam_data()
    elif more == '3':
        print(f'confirm purchase of 2.5GB (3 DAY) FOR N800.00 to {x}')
        confam_data()
    elif more== '4':
        print(f'confirm purchase of 2.5GB (1 DAY) FOR N500.00 to {x} ')
        confam_data()
    elif more == '5':
        dailyplan_others(x)
    else:
        print('wrong input')
        moreplans(x)

def dailyplan_others(x):
    PLAN=input('SELECT OPTIONS\n\n'
                    '1> 40MB (1 DAY) FOR N50.00\n'
                    '2> 100MB (1 DAY) FOR N100.00\n'
                    '3> 200MB (3 DAY) FOR N200.00\n'
                    '4> 100MB (1 DAY) FOR N200.00\n'
                    '5> next page\n'
                    '>>>'
                    )
    if PLAN == '1':
        print(f'confirm purchase of 40MB (1 DAY) FOR N50.00 to {x} ')
        confam_data()
    elif PLAN == '2':
        print(f'confirm purchase of 100MB (1 DAY) FOR N100.00 to {x} ')
        confam_data()
    elif PLAN == '3':
        print(f'confirm purchase of 200MB (1 DAY) FOR N200.00 to {x} ')
        confam_data()
    elif PLAN== '4':
        print(f'confirm purchase of 100MB (1 DAY) FOR N200.00 to {x} ')
        confam_data()
    elif PLAN == '5':
        moreplans(x)
    else:
        print('wrong input')
        dailyplan_others()








################all for self
def monthsplan():
    plan=input('SELECT OPTION\n'
        '1> 400GB (90 DAYS) FOR N50000\n'
               
             '>>>'

    )
    if plan=='1':
        print('confirm purchase of 400GB (90 DAYS) FOR N50000.00 ')
        confam_data()
    else:
        monthsplan()



def yearplan():
    PLAN = input('SELECT OPTIONS\n\n'
                 '1> 400GB (90 DAYS) FOR N50000.00\n'
                 '2> 500GB (120 DAYS) FOR N600000.00\n'
                 
                 '>>>'
                 )


    if PLAN == '1':
      print('confirm purchase of 400GB (90 DAYS) FOR N50000.00 ')
      confam_data()
    elif PLAN == '2':
         print('confirm purchase of 500GB (120 DAYS) FOR N600000.00 ')
         confam_data()
    else:
        print('error unsupported')
        select_data_plan()


def moreplan3():
    PLAN = input('SELECT OPTIONS\n\n'
                 '1> 240GB (30 DAYS) FOR N30000.00\n'
                 '2> 280GB (30 DAYS) FOR N360000.00\n'
                 '3> Back\n'

                 '>>>'
                 )
    if PLAN == '1':
        print('confirm purchase of 240GB (30 DAYS) FOR N30000.00 ')
        confam_data()
    elif PLAN == '2':
        print('confirm purchase of 280GB (30 DAYS) FOR N360000.00 ')
        confam_data()
    elif PLAN == '3':
        moreplan2()


    else:
        print('wrong input')
        moreplan3()


def moreplan2():
    PLAN = input('SELECT OPTIONS\n\n'
                 '1> 30GB (30 DAYS) FOR N8000.00\n'
                 '2> 40GB (30 DAYS) FOR N10000.00\n'
                 '3> 75GB (30 DAYS) FOR N15000.00\n'
                 '4> 120GB (30 DAYS) FOR N20000.00\n'
                 '5> next page\n'
                 '6> back\n'

                 '>>>'
                 )
    if PLAN == '1':
        print('confirm purchase of 30GB (30 DAYS) FOR N8000.00 ')
        confam_data()
    elif PLAN == '2':
        print('confirm purchase of 40GB (30 DAYS) FOR N10000.00 ')
        confam_data()
    elif PLAN == '3':
        print('confirm purchase of 75GB (30 DAYS) FOR N15000.00 ')
        confam_data()
    elif PLAN == '4':
        print('confirm purchase of 120GB (30 DAYS) FOR N20000.00 ')
        confam_data()
    elif PLAN == '5':
        moreplan3()
    elif PLAN == '6':
        moreplan1()

    else:
        print('wrong input')
        moreplan2()


def moreplan1():
    PLAN=input('SELECT OPTIONS\n\n'
                    '1> 6GB (30 DAYS) FOR N2500.00\n'
                    '2> 10GB (30 DAYS) FOR N3000.00\n'
                    '3> 15GB (30 DAYS) FOR N4000.00\n'
                    '4> 18GB (30 DAYS) FOR N5000.00\n'
                    '5> next page\n'
                    '6> back\n'
               
                    '>>>'
                    )
    if PLAN == '1':
        print('confirm purchase of 6GB (30 DAYS) FOR N2500.00 ')
        confam_data()
    elif PLAN == '2':
        print('confirm purchase of 10GB (30 DAYS) FOR N3000.00 ')
        confam_data()
    elif PLAN == '3':
        print('confirm purchase of 15GB (30 DAYS) FOR N4000.00 ')
        confam_data()
    elif PLAN== '4':
        print('confirm purchase of 18GB (30 DAYS) FOR N5000.00 ')
        confam_data()
    elif PLAN == '5':
        moreplan2()
    elif PLAN=='6':
        monthlyplan()

    else:
        print('wrong input')
        moreplan1()



def monthlyplan():
    PLAN=input('SELECT OPTIONS\n\n'
                    '1> 1.2GB (30 DAYS) FOR N1000.00\n'
                    '2> 1.5GB (30 DAYS) FOR N1200.00\n'
                    '3> 3GB (30 DAYS) FOR N1500.00\n'
                    '4> 4.5GB (30 DAYS) FOR N2000.00\n'
                    '5> next page\n'
                    '>>>'
                    )
    if PLAN == '1':
        print('confirm purchase of 1.2GB (30 DAYS) FOR N1000.00 ')
        confam_data()
    elif PLAN == '2':
        print('confirm purchase of 1.5GB (30 DAYS) FOR N1200.00 ')
        confam_data()
    elif PLAN == '3':
        print('confirm purchase of 3GB (30 DAYS) FOR N1500.00 ')
        confam_data()
    elif PLAN== '4':
        print('confirm purchase of 4.5GB (30 DAYS) FOR N2000.00 ')
        confam_data()
    elif PLAN == '5':
        moreplan1()
    else:
        print('wrong input')
        monthlyplan()




def weeklyplan():
    PLAN=input('SELECT OPTIONS\n\n'
                    '1> 350MB (7 DAYS) FOR N350.00\n'
                    '2> 750MB (7 DAYS) FOR N500.00\n'
                    '3> 5GB (7 DAYS) FOR N1500.00\n'
        
                    '>>>'
                    )
    if PLAN == '1':
        print('confirm purchase of 350MB (7 DAYS) FOR N350.00 ')
        confam_data()
    elif PLAN == '2':
        print('confirm purchase of 750MB (7 DAYS) FOR N500.00 ')
        confam_data()
    elif PLAN == '3':
        print('confirm purchase of 5GB (7 DAYS) FOR N1500.00 ')
        confam_data()

    else:
        print('wrong input')
        weeklyplan()


def all_work_pin():
    pin = input('\n>>>')
    if pin=='1234':
        print(f'You transaction was succesful.'
              f'\nThank you for using our USSD service.')
    else:
        print('Invalid pin\nTry again')
        all_work_pin()


def confam_data():
    confirm = input('1.Confirm\n2.Cancel\n\t>>> ')
    if confirm == '1' and confirm.isnumeric():
        print('Enter 4-digit ussd pin to complete transfer ')
        all_work_pin()

    elif confirm == '2' and confirm.isnumeric():
        print('Transfer cancel.\nThank you for using our ussd service')

    else:
        print('Invalid entry\nTry again')
        confam_data()

def moreplan():
    more=input( '1> 500MB (1 DAY) FOR N350.00\n'
                '2> 350MB (1 DAY) FOR N300.00\n'
                '3> 2.5GB (3 DAY) FOR N800.00\n'
                '4> 2.5MB (1 DAY) FOR N500.00\n'
                '5> Back\n'
                '>>>'
                )
    if more == '1':
        print('confirm purchase of 500MB (1 DAY) FOR N350.00 ')
        confam_data()
    elif more == '2':
        print('confirm purchase of 350MB (1 DAY) FOR N300.00 ')
        confam_data()
    elif more == '3':
        print('confirm purchase of 2.5GB (3 DAY) FOR N800.00 ')
        confam_data()
    elif more== '4':
        print('confirm purchase of 2.5GB (1 DAY) FOR N500.00 ')
        confam_data()
    elif more == '5':
        dailyplan()
    else:
        print('wrong input')
        dailyplan()


def dailyplan():
    PLAN=input('SELECT OPTIONS\n\n'
                    '1> 40MB (1 DAY) FOR N50.00\n'
                    '2> 100MB (1 DAY) FOR N100.00\n'
                    '3> 200MB (3 DAY) FOR N200.00\n'
                    '4> 100MB (1 DAY) FOR N200.00\n'
                    '5> next page\n'
                    '>>>'
                    )
    if PLAN == '1':
        print('confirm purchase of 40MB (1 DAY) FOR N50.00 ')
        confam_data()
    elif PLAN == '2':
        print('confirm purchase of 100MB (1 DAY) FOR N100.00 ')
        confam_data()
    elif PLAN == '3':
        print('confirm purchase of 200MB (1 DAY) FOR N200.00 ')
        confam_data()
    elif PLAN== '4':
        print('confirm purchase of 100MB (1 DAY) FOR N200.00 ')
        confam_data()
    elif PLAN == '5':
        moreplan()
    else:
        print('wrong input')
        dailyplan()


def select_data_plans():
    dataplan = input('SELECT DATA PLAN\n\n'
                     '1> DAILY_PLAN\n'
                     '2> WEEKLY_PLAN\n'
                     '3> MONTHLY_PLAN\n'
                     '4> 2-3 MONTHS_PLANS\n'
                     '5> YEARLY_PLAN\n\t'

                     '>>>'
                     )

    if dataplan == '1':
        data()
    elif dataplan == '2':
        data1()
    elif dataplan == '3':
        data2()
    elif dataplan == '4':
        data3()
    elif dataplan == '5':
        data4()
    else:
        print('value unsupported')
        select_data_plans()

def select_data_plan():
    dataplan=input('SELECT DATA PLAN\n\n'
                   '1> DAILY_PLAN\n'
                   '2> WEEKLY_PLAN\n'
                   '3> MONTHLY_PLAN\n'
                   '4> 2-3 MONTHS_PLANS\n'
                   '5> YEARLY_PLAN\n\t'
                    
                    '>>>'
                   )

    if dataplan=='1':
        dailyplan()
    elif dataplan == '2':
        weeklyplan()
    elif dataplan == '3':
        monthlyplan()
    elif dataplan == '4':
        monthsplan()
    elif dataplan == '5':
        yearplan()
    else:
        print('value unsupported')
        select_data_plan()


def select_provider():
    data_provider=input('SELECT_PROVIDER\n\n'
                        '1>MTN\n'
                        '2>AIRTEL\n'
                        '3>GLO\n'
                        '4>ETISALAT\n\t'
                        '>>>'
                   )
    select_data_plans()

def buy_data():
    bu_data=input('1>self\n'
              '2>third party\n'
              
              '>>>')
    if bu_data=='1':
        select_data_plan()
    elif bu_data=='2':
        select_provider()
    else:
         print('Invalid Entry\nTry again\n')
         buy_data()

def main_menu():
    menu = input(" USSD Banking Service.\n"
                         '1. Check Account Balance\n'
                         '2. Transfer Funds\n'
                         '3. Buy Airtime\n'
                         '4. Buy Data\n'
                         '5. Account Statements\n'
                         '6. More Services\n\t'

                         '>>> '
                         )
    if menu == '1':
                print('Your acct.bal is $300,000')

    elif menu == '2':
                funds_trans()

    elif menu == '3':
                airtime()
    elif menu == '4':
                buy_data()

    elif menu == '5':
                print('account statement')

    else:
                print('Invalid Entry\nTry again\n')
                main_menu()

## ussd function
def ussd_code():
    ussd = input('Enter ussd\n\t>>> ')
    if ussd == '*965#':
     main_menu()

    else:
        print('Invalid ussd\nTry again\n')


ussd_code()
