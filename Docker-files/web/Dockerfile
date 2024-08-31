#dockerfile nginx 
FROM nginx
LABEL "Project"="Vprofile"
LABEL "Author"="Brian"
RUN rm -rf /etc/nginx/conf.d/default.conf
copy nginxpro.conf /etc/nginx/conf.d/vprofile.conf
