# Create a multiline variable

Pretty simple but I always forget how to do it...

Put the second EOF at the beginning of the line or you will have a warning "here-document" ...


```bash
#!/bin/bash

read -d '' My_variable <<EOF
	SELECT * FROM my_table
	WHERE user_id=3
	AND group_id=5
EOF
echo "Multiline"
echo "$My_variable"

echo "On one line"
echo $My_variable
```
