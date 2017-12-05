zip -r comp2402a5{.zip,}


curl -sb -X POST \
                -F "code=[secret key]" \
                -F "upfile=@comp2402a5.zip" \
                -F "submit=Submit assignment" \
                [submission link] > result
                sed -n '/<pre>/,/<\/pre>/p' result | sed -e '1s/.*<pre>//' -e '$s/<\/pre>.*//'


curl -sb -X POST \
                -F "STUDENT=[secret key]" \
                -F "ASSIGNMENT=a5" \
                -F "submit=Email detailed results" \
                [email submission link] > email_confirmation
                sed -n '/.css">/,/<br>/p' email_confirmation | sed -e '1s/.*.css">//' -e '$s/<br>.*//'
