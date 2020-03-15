# pyxing
이베스트투자증권 xing API python wrapper 

## 로그인

```python
from pyxing.session import *

xasession = XASession()
xasession.login("아이디", "비밀번호", "공인인증비밀번호", block=True)

print("서버이름: ", xasession.get_server_name())
print("연결상태: ", xasession.is_connected())
print("계좌수  : ", xasession.get_account_list_count())
print("계좌    : ", xasession.get_account_list(0))
```
