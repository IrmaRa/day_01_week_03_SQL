## Questions

1. Return ALL the data in the 'movies' table.


select * from movies;

2. Return ONLY the name column from the 'people' table


select name from people;

3. Oops! Someone at CodeClan spelled Johnny's name wrong! Change it to reflect the proper spelling (change 'Jnny Watson' to 'Johnny Watson').


update people set name = 'Johnny Watson' where name = 'Jnny Watson';

4. Return ONLY your name from the 'people' table.


select * from people;
select name from people where id = 11;

5. The cinema is showing 'Batman Begins', but Batman is DC, not Marvel! Delete the entry from the 'movies' table.


delete from movies where id = 9;

6. Create a new entry in the 'people' table with the name of one of the instructors.


insert into people (name) values ('Simon Douglas');

7. Craig Morton, has decided to hijack our movie evening, Remove him from the table of people.


delete from people where name = 'Craig Morton';

8. Somehow the list of people includes two people named 'Simon'. Change these entries to the proper names ('Jack Jarvis' and 'Victor McDade')


select * from people;
update people set name = 'Jack Jarvis' where id = 8;
update people set name = 'Victor McDade' where id = 9;

9. The cinema has just heard that they will be holding an exclusive midnight showing of 'Guardians of the Galaxy 2'!! Create a new entry in the 'movies' table to reflect this.


insert into movies (title, year) values ('Guardians of the Galaxy 2', 2017, '12:10');

10. The cinema would also like to make the Guardian movies a back to back feature. Update the 'Guardians of the Galaxy' show time from 12:10 to 21:30


update movies set show_time = '21:30' where title = 'Guardians of the Galaxy 2';

## Extension

1. Research how to delete multiple entries from your table in a single command.


delete from movies where id >= 1 and id <= 7;
