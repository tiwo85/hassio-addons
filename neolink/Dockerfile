FROM quantumentangledandy/neolink:v0.5.13

RUN apt-get update && \
    apt-get install -y \
        jq && \
    apt-get clean -y && rm -rf /var/lib/apt/lists/*

# Copy data for add-on
COPY run.sh /
RUN chmod a+x /run.sh

CMD [ "/run.sh" ]
