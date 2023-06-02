# Hostel-Management-System

The Main agenda in this project is to build a fully-flexible Hostel Management System, in such a way that it contains all the relevant and important data concerned with a Hostel. This System keeps track of all the details, starting from hostel block, to each furniture in the room of each of the hostel blocks. It doesn’t contain any ambiguous entities, which makes it a flexible one.I have included several foreign key constraints, which binds together the relations. Here, in this project,I have included 10 relations, all related and applicable to hostel or other similar institutions. Here,I have managed to complete this project using only SQL Plus.
These entities along with certain relationships between them form the Hostel Management System. Here, I have first created all the relations using ‘create’ command. After that, Ifeeded the respective values to the relations and finally declare foreign key attributes, which binds together the relations together.


Foreign keys:
1. Student Relation derives BHOSTEL_ID from Boys_Hostel’s BHOSTEL_ID 
2. Mess_Employee derives BHOSTEL_ID from Boys_Hostel’s BHOSTEL_ID 
3. Room derives BHOSTEL_ID from Boys_Hostel’s BHOSTEL_ID
4. Student derives ROOM_ID from Room’s ROOM_ID
5. Fee derives FSID from Student’s STUDENT_ID

NOTE:The above relational schema includes all the possible foreign key relationships. However, I chose 5 among them in the project.

Five Foreign Keys additional:

ALTER TABLE STUDENT ADD CONSTRAINT BID FOREIGN KEY(BHOSTEL_ID) REFERENCES BOYS_HOSTEL(BHOSTEL_ID);
ALTER TABLE MESS_EMPLOYEE ADD CONSTRAINT MID FOREIGN KEY(BHOSTEL_ID) REFERENCES BOYS_HOSTEL(BHOSTEL_ID);
ALTER TABLE ROOM ADD CONSTRAINT BID2 FOREIGN KEY(BHOSTEL_ID) REFERENCES BOYS_HOSTEL(BHOSTEL_ID);
ALTER TABLE STUDENT ADD CONSTRAINT RID FOREIGN KEY(ROOM_ID) REFERENCES ROOM(ROOM_ID);
ALTER TABLE FEE ADD CONSTRAINT SID FOREIGN KEY(FSID) REFERENCES STUDENT(STUDENT_ID);

Conclusion:

In any scenario, whatever may the case be,I often require database management systems. Therefore, the deep study of database management systems are an important factor in today’s moving world. Here, as I have seen, the Hostel Management System keeps a record of all the required data, concerned with a very little entity such as a furniture, thus revealing its true power. Take a quick look at the world around you, a bank has a database; a school has a database; a library has a database; and the list goes on. 
