py_listComprehension
====================

Initial code:
>>> girls = ['alice', 'bernice', 'clarice']
>>> boys = ['chris', 'arnold', 'bob']
>>> [b + '+' + g for b in boys for g in girls if b[0] == g[0]]
['chris+clarice', 'arnold+alice', 'bob+bernice']


Better solution:
We build a dictionary: letterGirls. It using every single first letter as key, girl's name as value.
+		letterGirls	{'a': ['alice', 'alice'], 'b': ['bernice'], 'c': ['clarice', 'cici']}	dict
