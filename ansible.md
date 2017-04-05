### Patterns

http://docs.ansible.com/ansible/intro_patterns.html#patterns

- OR
```
webservers:dbservers
```

- AND
```
webservers:&dbservers
```

- NOT
```
webservers:&dbservers:!phoenix
```

- subscript
```
websesrvers[0]
websesrvers[-1]
websesrvers[0:1]
websesrvers[1:]
```
