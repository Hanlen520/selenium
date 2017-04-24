# ��Ŀ�������
* ����Ŀ����[Selenium](https://github.com/SeleniumHQ/selenium)��Դ���߷�װ���ɵ��Զ�����web���Թ���

# ����
* ����python3
* ����ά���õ�YMAL


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
    - element_info: //*[@id="setting111"]/a
      find_type: by_xpath

```

**��д��������**

��������ֱ�Ӹ���

```
PATH = lambda p: os.path.abspath(
    os.path.join(os.path.dirname(__file__), p)
)
from testRunner.runnerBase import TestInterfaceCase
class testSetting(TestInterfaceCase):
    def setUp(self, methodName=''):
        super(testSetting, self).setUp()
        self.bc = webCase.WebCaseBase(driver=self.driver, casename="testSetting")
    def tearDown(self):
        self.driver.quit()
        pass
    def test_setting(self):
        self.bc.execCase(PATH("../yaml/setting.yaml"))
```



**����������:**

```
pyhton testRunner/runner.py
```

**���Ա���**
![](log/comment.PNG "comment.PNG")

![](log/detail.PNG "detail.PNG")





