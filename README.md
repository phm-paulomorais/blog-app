# README

This README would normally document whatever steps are necessary to get the
application up and running.

Things you may want to cover:

* Rails version: 5.2.8.1

* Ruby version: 2.7.0 (x86_64-linux)

* System dependencies

* Configuration

* Database creation

* Database initialization

* How to run the test suite

* Services (job queues, cache servers, search engines, etc.)

* Deployment instructions

* ...
# blog-app

Vídeo da Aplicação: https://www.loom.com/share/1a305f33345c4433917d43d8043aa1e5

Link de referência: 

https://reinteractive.com/posts/32-ruby-on-rails-3-2-blog-in-15-minutes-step-by-step

Erros encontrados:

<img alt="Erro" title="Erro" src="erro-app-blog.png" width="800px" />

Solução:

 - Fazer o ajuste no arquivo comments_controller.rb:

	@comment = @post.comments.create!(params[:comment].permit!)
	
	Referência da solução: https://stackoverflow.com/questions/19861067/activemodelforbiddenattributeserror-in-commentscontrollercreate

Problema: Não suportado mais o div_for

Solução: 

	Adicionar no arquivo GemFile a seguinte instrução: gem 'record_tag_helper', '~> 1.0'





