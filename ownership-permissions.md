### Permissions and Ownership

We have 3 types of ownership.

**User:** He is the one created the file/folder. Denotes by u
**Group:** a group of users the file belongs to. Denotes by g
**Other:** Any one other than the user and group. Denotes by o

3 types of Permissions

**Read:** denotes by number 4
**Write:** Denotes by number 2
**Execute:** Denotes by number 1
```
-rw-rw-r-- 1 ec2-user ec2-user  1483 May 24 13:58 eks-client.sh
```
Above line has total 10 characters. First character  shows it is file(-)
Next 3 characters denotes permission of user.
Next 3 characters denotes permission of group
Next 3 characters denotes permission of other

So user has read and write access.
Group has read and write access.
others have only write access.

If we want to add execute permission to everyone.

```
chmod ugo+x [file-name]
```

If we want to add write permission only to user and group.

```
chmod ug+w [file-name]
```

If we want to remove execute access to all.

```
chmod ugo-x [file-name]
```

We can use letters also.
R+W = 4+2 =6
R+W+X = 4+2+1 = 7

Below line denotes read access to user and no access to group and others.
```
chmod 400 [file-name]
```
