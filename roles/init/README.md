Revboot/Cloudflare.Init Role
============================

Initialization role (gets and creates zones).

Requirements
------------

Does not require root privileges by default. This is set on `defaults/main.yml`.

Role Variables
--------------

See `defaults/main.yml` for more information.

Dependencies
------------

The following dependencies are needed:

- Python: 3.0+.
  - Python Packages: See `requirements.python.txt` for more information.
- Ansible: 2.12, enforced in `meta/main.yml` and `requirements.python.txt`.
  - Ansible Collections: See `requirements.galaxy.yml` for more information.
  - Ansible Roles: See `requirements.galaxy.yml` and `meta/main.yml` for
more information.

Example Playbook
----------------

Initialization:
```
    - name: "Initialize Cloudflare playbook"
      hosts: all
      tasks:
        - name: "Initialize Cloudflare with role revboot/cloudflare.init"
          include_role:
            name: revboot/cloudflare.init
          vars:
```

License
-------

This program is free software: you can redistribute it and/or modify  
it under the terms of the GNU General Public License as published by  
the Free Software Foundation, either version 3 of the License, or  
(at your option) any later version.

This program is distributed in the hope that it will be useful,  
but WITHOUT ANY WARRANTY; without even the implied warranty of  
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the  
GNU General Public License for more details.  

You should have received a copy of the GNU General Public License  
along with this program.  If not, see <http://www.gnu.org/licenses/>.

Author Information
------------------

Maintainer: Luís Algarvio <luis.algarvio@revboot.com> https://lp.algarvio.org/

Copyright Revboot - Tecnologias de Informação e Comunicação, Lda.
