# 110-database-concept-
Pip install pysqlite3
import salite3
conn = sglite3.connect("school.db")
cur = conn.cursor()
cur.execute("""
CREATE TABLE IF NOT EXISTS Students(
ID INTEGER PRIMARY KEY AUTOINCREMENT
Name TEXT
Age INTEGER, 
Grade TEXT
พ"")
data = [("Alice", 20, "A"), ("Bob", 21, "B")
cur.executemany("INSERT INTO Students (Name, Age, Grade) VALuEs (.?, ?y', data)
conn.commit)
print("Students:")
for row in cur.execute("SELECT * FROM Students"”):
print(row)
8/15
cur.execute("DELETE FROM Students WHERE ID =1")
conn.commit()
print("InAfter Deletion:")
for row in cur.execute("SELECT * FROM Students"):
print(row)
conn.close()
Output:
Students
(1, 'Alice', 20, 'A')
(2, 'Bob', 21, 'B')
After Deletion:
(2, 'Bob', 21, 'B)
