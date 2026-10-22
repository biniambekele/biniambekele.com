# biniambekele.com

[biniambekele.com website](https://biniambekele.com)

## Getting Started

1.  Install `node>=10.0.0` and `npm>=6.0.0`
1.  Run `npm install` to install project dependencies
1.  Run `npm run server`, which serves `public/`
1.  Navigate to `http://localhost:8080` in a web browser

## Production

Only `public/` is served. Everything else in the repository, such as `resources/` and the npm files, stays off the web.

Ansible
[variables](https://docs.ansible.com/ansible/latest/user_guide/playbooks_variables.html) definition for use with
[ansible-workstation](https://github.com/andornaut/ansible-workstation) and
[ansible-role-nginx](https://github.com/andornaut/ansible-role-nginx):

```
websites:
  - domain: biniambekele.com
    repo: https://github.com/biniambekele/biniambekele.com.git
    path: public
```
