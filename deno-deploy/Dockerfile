FROM hayd/alpine-deno
EXPOSE 8000
WORKDIR /app
ADD . /app
# RUN ping -c 4 8.8.8.8
# RUN ping deno.land
# RUN wget https://deno.land/std@0.55.0/http/server.ts
# RUN cat /etc/resovl.conf
# RUN echo "nameserver 8.8.8.8" >> /etc/resolv.conf
RUN deno cache server.ts
CMD ["run", "--allow-net", "server.ts"]

