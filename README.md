# Use a bashrc.d directory to split .bashrc into separate files

Clone this in ~ and include the following into your .bashrc;

```shell
for path in $(run-parts --list ~/.bashrc.d)
do
    source $path
done
```
