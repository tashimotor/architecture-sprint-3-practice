FROM squidfunk/mkdocs-material

RUN pip install mkdocs_puml
RUN pip install mkdocs-render-swagger-plugin
RUN pip install mkdocs-drawio

WORKDIR /docs

ENTRYPOINT ["/sbin/tini", "--", "mkdocs"]
CMD ["serve", "--dev-addr=0.0.0.0:8000"]
