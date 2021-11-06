# publicnote.com
Public Encrypted Notes

Publicnote is a database of notes that is accessible to the public. No account is required. Simply enter a title to access any note.

Every note is encrypted with AES256, using the title as the encryption key. An SHA256 hash of the title is used to index the encrypted note. The title is never exposed, thus neither the website owner nor the web host can view the plaintext contents of any note (unless the title is easily guessed).

            title → SHA256 → index
              ⇣
             🔑
    note → AES256 → encrypted note

By design, there is no way to recover a note if you forget the title.

Notes stored on publicnote can be public or private, depending on the complexity of the title. Simple titles lead to highly visible notes that can be edited by anyone who stumbles upon it, while complex titles lead to private, anonymous notes that are securely encrypted. The more complex the title is, the stronger the encryption is.

There are various uses for publicnote:
personal notetaking
copy-pasting text from one device to another
sending messages privately and anonymously
chatting with strangers
posting jokes and ASCII art
puzzles and scavenger hunts
announcements and advertisements
Using common words like "hello" as your title is for entertainment purposes only. You will find a variety of messages left by others. If you find something you find offensive, delete it. More complex titles that can't be easily guessed can be used for personal use, but never use it to store sensitive information.

Publicnote is open source and offered as a free service, running thanks to your cryptocurrency donations.

daniel@ncrypt.org

BTC: 1HrQfojcRt4gGEZntEwp24KVrSch8mtqMk  
LTC: Lc5Mw23SWYJjX3Fx4Nw7J5PG4eyyG3Pow2  
