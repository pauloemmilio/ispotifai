#Imagem base
FROM openjdk:8-jdk-alpine

#Informacoes sobre a imagem
LABEL autor="Rebeca Dantas, Paulo Emílio, Lilían Lucena, Vinicius" \
      email="rebeca.queiroz@dce.ufpb.br" \
      data_criacao="18/05/2019" \
      versao="1.0.0" \
      descricao="Especifica a imagem Docker do Ispotifay" \
      licenca="copyright"

# Configurando JAR

ARG JAR_FILE
COPY src/${JAR_FILE} /src/ispotifai.jar

#Iniciando o servico ao iniciar o conteiner
ENTRYPOINT ["java","-Djava.security.egd=file:/dev/./urandom","-jar","/src/ispotifai.jar"]
