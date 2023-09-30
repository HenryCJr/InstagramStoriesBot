from selenium import webdriver

from selenium.webdriver.edge.service import Service as EdgeService

import PySimpleGUI as psg
from webdriver_manager.microsoft import EdgeChromiumDriverManager
import pyautogui
import time

#Layout begin

psg.theme('topanga')

l1 = psg.Text('E-mail or nickname:', key='-OUT-', font=('Arial Bold', 20), expand_x=True, justification='center')
t1 = psg.Input('', enable_events=True, key='-EMAIL-', font=('Arial Bold', 20), expand_x=True, justification='left')

l2 = psg.Text('Password:', key='-OUT-', font=('Arial Bold', 20), expand_x=True, justification='center')
t2 = psg.Input('', enable_events=True, key='-PASSWORD-', font=('Arial Bold', 20), expand_x=True, justification='left')

b1 = psg.Button('Run', font=('Arial Bold', 20))
b2 = psg.Button('Exit', font=('Arial Bold', 20))
layout = [[l1], [t1],[l2], [t2], [b1, b2]]
window = psg.Window('Busca Automatizada', layout, size=(750, 350))


while True:             # Event Loop
        event, values = window.Read()
        # print(event, values)
        if event in (None, 'Exit'):
            break
        elif event == 'Run':

           a = str(values['-EMAIL-'])
           b = str(values['-PASSWORD-'])


           window.close()




#Layout end



driver = webdriver.Edge(service=EdgeService(EdgeChromiumDriverManager().install()))

link = 'https://www.instagram.com/'


driver.get(link)
driver.maximize_window()

# soup = BeautifulSoup(r, 'html.parser')
time.sleep(10)

log = driver.find_element('xpath', '//*[@id="loginForm"]/div/div[1]/div/label/input')
log.send_keys(a)
password = driver.find_element('xpath', '//*[@id="loginForm"]/div/div[2]/div/label/input')
password.send_keys(b)
driver.find_element('xpath', '//*[@id="loginForm"]/div/div[3]/button').click()


x = 1
i = 0
cont = 0

# roll = 200

time.sleep(5)
driver.get(link)
time.sleep(10)
driver.find_element('xpath','/html/body/div[3]/div[1]/div/div[2]/div/div/div/div/div[2]/div/div/div[3]/button[2]').click()
time.sleep(3)
driver.find_element('xpath','/html/body/div[2]/div/div/div[2]/div/div/div/div[1]/div[1]/div[2]/section/main/div[1]/div[1]/div/div[1]/div/div/div/div/div/div/ul/li[3]/div/button').click()


time.sleep(3)
pause = driver.find_element('xpath','/html/body/div[2]/div/div/div[2]/div/div/div/div[1]/div[1]/section/div[1]/div/div[5]/section/div/header/div[2]/div[2]/div[1]/div')
driver.find_element('xpath','/html/body/div[2]/div/div/div[2]/div/div/div/div[1]/div[1]/section/div[1]/div/div[5]/section/div/header/div[2]/div[2]/div[1]/div').click()
driver.find_element('xpath','/html/body/div[2]/div/div/div[2]/div/div/div/div[1]/div[1]/section/div[1]/div/div[5]/section/div/div[3]/div/div/div[2]/span/div/div/span').click()
like = driver.find_element('xpath','/html/body/div[2]/div/div/div[2]/div/div/div/div[1]/div[1]/section/div[1]/div/div[5]/section/div/div[3]/div/div/div[2]/span/div/div/span')
driver.find_element('xpath','/html/body/div[2]/div/div/div[2]/div/div/div/div[1]/div[1]/section/div[1]/div/div[5]/section/div/button').click()

while(i<=100):





    try:


        time.sleep(2)

        pyautogui.moveTo(746,715)
        pyautogui.moveTo(600, 715)

        driver.find_element('xpath','/html/body/div[2]/div/div/div[2]/div/div/div/div[1]/div[1]/section/div[1]/div/div[5]/section/div/div[3]/div/div/div[2]/span/div/div/span').click()


        time.sleep(0.5)
        driver.find_element('xpath','/html/body/div[2]/div/div/div[2]/div/div/div/div[1]/div[1]/section/div[1]/div/div[5]/section/div/button[2]').click()



    except:




        pass

    x = x + 1



time.sleep(10)
driver.close()
