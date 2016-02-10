# python-code
code created by me during my online course
fline = "blah blah"

if len(fline) > 1 :
    print "More than one"
    if fline[0] == "h" : 
        print "Has an h"
print "All done"

def comp_pay(h,r):
     if h<=40:
        pay=r*h
        return pay
     else:
         pay=r*40+((r*1.5)*(h-40))
         return pay
print comp_pay(45,10)

#p2
astr='hello'
try:
    print 'hello' 
    istr=int(astr) 
    print 'there'
except:istr=-1
print 'done',istr

n=[4,56,7,3,45,2]
n[2]=90
print n,len(n),range(len(n))

#to count a loop
z=0
for n in [5,7,8,9,6,4,34,78,56]:
      z=z+1
      print z,'.',n
print 'total loops: ',z

name='poornima'
i=0
while i<len(name):
      print name[i]
      i=i+1

#name = raw_input("Enter file:")
handle = open('mbox-short.txt')
for l in handle:
     if l.startswith('From:'):
         p=l[5:]
c=dict()
for w in p:
    c[w]=c.get(w,0)+1
maxv=None
maxk=None
for k,v in c.items():
    if maxv==None or maxv<v:
         maxv=v
         maxk=k 
print maxk,maxv

#mbox-short.txt
From stephen.marquard@uct.ac.za Sat Jan  5 09:14:16 2008
Return-Path: <postmaster@collab.sakaiproject.org>
Received: from murder (mail.umich.edu [141.211.14.90])
	 by frankenstein.mail.umich.edu (Cyrus v2.3.8) with LMTPA;
	 Sat, 05 Jan 2008 09:14:16 -0500
X-Sieve: CMU Sieve 2.3
Received: from murder ([unix socket])
	 by mail.umich.edu (Cyrus v2.2.12) with LMTPA;
	 Sat, 05 Jan 2008 09:14:16 -0500
Received: from holes.mr.itd.umich.edu (holes.mr.itd.umich.edu [141.211.14.79])
	by flawless.mail.umich.edu () with ESMTP id m05EEFR1013674;
	Sat, 5 Jan 2008 09:14:15 -0500
Received: FROM paploo.uhi.ac.uk (app1.prod.collab.uhi.ac.uk [194.35.219.184])
	BY holes.mr.itd.umich.edu ID 477F90B0.2DB2F.12494 ; 
	 5 Jan 2008 09:14:10 -0500
Received: from paploo.uhi.ac.uk (localhost [127.0.0.1])
	by paploo.uhi.ac.uk (Postfix) with ESMTP id 5F919BC2F2;
	Sat,  5 Jan 2008 14:10:05 +0000 (GMT)
Message-ID: <200801051412.m05ECIaH010327@nakamura.uits.iupui.edu>
Mime-Version: 1.0
Content-Transfer-Encoding: 7bit
Received: from prod.collab.uhi.ac.uk ([194.35.219.182])
          by paploo.uhi.ac.uk (JAMES SMTP Server 2.1.3) with SMTP ID 899
          for <source@collab.sakaiproject.org>;
          Sat, 5 Jan 2008 14:09:50 +0000 (GMT)
Received: from nakamura.uits.iupui.edu (nakamura.uits.iupui.edu [134.68.220.122])
	by shmi.uhi.ac.uk (Postfix) with ESMTP id A215243002
	for <source@collab.sakaiproject.org>; Sat,  5 Jan 2008 14:13:33 +0000 (GMT)
Received: from nakamura.uits.iupui.edu (localhost [127.0.0.1])
	by nakamura.uits.iupui.edu (8.12.11.20060308/8.12.11) with ESMTP id m05ECJVp010329
	for <source@collab.sakaiproject.org>; Sat, 5 Jan 2008 09:12:19 -0500
Received: (from apache@localhost)

#search using boolean
find=False
for n in [9,41,12,3,74,15]:
     if n==3:
         find=True
         break
print find

while True:
          line=raw_input('>')
          if line[0]=='#':
              continue
          if line == 'done':
               break
          print line
print 'done'

purse=dict()
purse ['pen']=5            # different type of constant definition
purse= {'tissue':50,'candy':7}
print purse
purse ['candy']= purse ['candy'] + 3
print purse

#add numbers in a loop:
z=0
for t in [9,41,12,3,74,15]:
      z=z+t 
print 'after',z 

data = 'From stephen.marquard@uct.ac.za Sat Jan  5 09:14:16 2008'
pos = data.find('.')
print data[pos:pos+3]

fn=raw_input('enter file:')
fh=open(fn)
count=0
for line in fh:
    if line.startswith('Subject:'):
        count=count+1
print 'there are',count,'subject lines in',fn 

try:istr=int(astr)
except:istr=-1 
print 'first',istr
astr='123'
try:istr=int(astr)
except:istr=-1
print 'second',istr
