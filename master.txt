import requests
from bs4 import BeautifulSoup
f=open(r"C:/Users/5288/Downloads/output12 (1).html", encoding="utf-8")
#print(f.read())
soup=BeautifulSoup(f.read(),'html.parser')
#a=soup.td['class']
#print(a)
s=soup.find(class_="c0")
print(s)
#print(s.contents)
for lm in s:
    print(lm)
#print(s.next_sibling)
for c in s.next_sibling:
    print(c)
#print(s.next_sibling.next_sibling)
for d in s.next_sibling.next_sibling:
    print(d)
for f in s.next_sibling.next_sibling.next_sibling:
    print(f)
list1=[]
for lm in s:
    list1.append(lm)
    print(lm)
for c in s.next_sibling:
    list1.append(c)
    print(c)
for d in s.next_sibling.next_sibling:
    list1.append(d)
    print(d)
for e in  s.next_sibling.next_sibling.next_sibling:
    list1.append(e)
    print(list1)
    