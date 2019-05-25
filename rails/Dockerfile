FROM ruby:2.6.3

RUN groupadd -r rails && useradd --no-log-init -r -g rails rails \
    && mkdir /home/rails \
    && chown -R rails:rails /home/rails \
    && curl -sL https://deb.nodesource.com/setup_12.x | bash - \
    && apt-get install -y nodejs

USER rails

WORKDIR /home/rails

RUN gem install rails -v 5.2.3

EXPOSE 3000

CMD ["bash"]
