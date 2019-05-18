#Passos
# Instruções para baixar e compilar as imagens Docker do Ispotifai

## Obtendo o código fonte
. Baixe o código do repositório Git com o comando a seguir.
git clone https://github.com/pauloemmilio/ispotifai
cd ispotifai

## Para compilar a imagem 
cd ispotifai/ispotifai
docker build -t rqdzs/ispotifai:0.0.1 .

##Inicie o conteiner
Use o comando a seguir para iniciar um conteiner do ispotifai
docker run -d -p 8080:8080 --name ispotifai rqdzs/ispotifai:0.0.1
