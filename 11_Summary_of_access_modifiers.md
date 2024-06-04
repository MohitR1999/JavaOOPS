
| Visibility                              | public | protected                                 | default | private |
| --------------------------------------- | ------ | ----------------------------------------- | ------- | ------- |
| within the same class                   | Yes    | Yes                                       | Yes     | Yes     |
| From child class of same package        | Yes    | Yes                                       | Yes     | No      |
| From non child class of same package    | Yes    | Yes                                       | Yes     | No      |
| From child class of outside package     | Yes    | Yes (We need to use child reference only) | No      | No      |
| From non child class of outside package | Yes    | No                                        | No      | No      |
