# ��Ŀ�������
* ����Ŀ����[Selenium](https://github.com/SeleniumHQ/selenium)��Դ���߷�װ���ɵ��Զ�����web���Թ���

# ����
* ���ǻ���python3
* ���ǻ���webdriver���󲿷ִ��붼����ͨ�ã�ֻ�������ļ���һ��
* ����ά���õ�YMAL
* �ʼ�����excel�Ĳ��Ա���


# �÷�

**������Ŀ:**

```
git clone git@github.com:Louis-me/selenium_auto.git
```

**����openurl.yaml**

```
openurl: http://www....com/login
```

**��������yaml**


```
testinfo: 
    - id: 001
      moudle: mokģ��
      intr: ����
testcase:
    - element_info: //*[@id="login"]/div[1]/div[2]/form/div[1]/input
      find_type: by_xpath
      operate_type: send_keys
      text: test
    - element_info: //*[@id="login"]/div[1]/div[2]/form/div[2]/input
      find_type: by_xpath
      operate_type: send_keys
      text: 123456
    - element_info: //*[@id="login"]/div[1]/div[2]/form/button[1]
      find_type: by_xpath
      operate_type: click
check:
    - element_info: //*[@id="home"]/a
      find_type: by_xpath

```



**����������:**

```
pyhton testRunner/runner.py
```







