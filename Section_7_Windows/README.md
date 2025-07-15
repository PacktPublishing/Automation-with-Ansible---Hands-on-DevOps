# Few Windows Adhoc commands

- ansible "windows" -m ansible.windows.win_ping
- ansible "windows" -m ansible.windows.win_ping -o

- ansible "windows" -m ansible.windows.win_command -a "hostname"
- ansible "windows" -m ansible.windows.win_command -a "netstat"

- ansible "windows" -m ansible.windows.win_file -a "path=C:\Users\demoansible\Desktop\demofile.txt stste=touch"
- ansible "windows" -m ansible.windows.win_file -a 'path="C:\\Users\\demoansible\\Desktop\\demoonefile.txt" state=touch'

- ansible "windows" -m ansible.windows.win_file -a 'path="C:\\Users\\demoansible\\Desktop\\demodir" state=directory'

- ansible "windows" -m ansible.windows.win_copy -a 'dest="C:\\Users\\demoansible\\Desktop\\demodir\\fileone" content="Hello how are you!"'

- ansible "windows" -m ansible.windows.win_copy -a 'dest="C:\\Users\\demoansible\\Desktop\\demodir\\filetwo.txt" content="Hello how are you!"'
