# data-warehouse-keplo-bikes

Repositório destinado ao segundo projeto do curso [Formação Engenharia de Dados: Domine Big Data!](https://www.udemy.com/course/engenheiro-de-dados/)

### Descrição do projeto
Construção do Data Warehouse de uma loja de bicicletas no banco de dados [PostgreSQL](https://www.postgresql.org/) em uma instância do [EC2](https://aws.amazon.com/pt/ec2/?trk=273714db-4e14-42ba-be75-e3e36c4bc786&sc_channel=ps&ef_id=CjwKCAjwx_eiBhBGEiwA15gLN0FldiPzmUbYiG9yqpGB4vVDQMKOC3W0VjoQx3qbP_YwaX_GRZZurhoCmSQQAvD_BwE:G:s&s_kwcid=AL!4422!3!589890540382!e!!g!!ec2!16393914376!135045745338) da [AWS](https://aws.amazon.com/).

Continuação do projeto [keplo-Bikes](https://github.com/keplindheison/keplo-bikes)


## Requerimentos:
<img  aling="center"  alt="amazon-web-services"  width="40"  height="40"  src="https://img.icons8.com/color/48/amazon-web-services.png"  />


## Tecnologias Usadas:
<div  style="display: inline_block"><br>
<img  aling="center"  alt="amazon-web-services"  width="40"  height="40"  src="https://img.icons8.com/color/48/amazon-web-services.png"  />
<img aling="center"  alt="linux"  width="40"  height="40" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/linux/linux-original.svg" />
<img aling="center"  alt="ubuntu"  width="40"  height="40" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/ubuntu/ubuntu-plain-wordmark.svg" />
<img  aling="center"  alt ="postgresql"  heigth="30"  width="40"  src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/postgresql/postgresql-original-wordmark.svg"  />
</div>

## Como Começar
Vamos continuar usando a máquina do projeto [keplo-Bikes](https://github.com/keplindheison/keplo-bikes).

Apos logar na máquina rodar os comando abixo:

Mudar para usúario postgres
```
sudo su - postgres
```

Mostrar diretorio atual
```
pwd
```

Criar diretorio dimensional
```
mkdir dimensional
```

Baixar repositorio como .zip
```
wget https://github.com/keplindheison/data-warehouse-keplo-bikes/archive/refs/heads/master.zip
```

Descompactar arquivo baixado
```
unzip master.zip
```

Logar no Postgres
```
psql
```

Mudar para o banco ed
```
\c ed;
```

Executar script 1.criandoTabelas.sql  
```
\i /var/lib/postgresql/dimensional/data-warehouse-keplo-bikes-master/1.criandoTabelas.sql
```

Executar script 2.inserindoDimensaoTempo.sql  
```
\i /var/lib/postgresql/dimensional/data-warehouse-keplo-bikes-master/2.inserindoDimensaoTempo.sql
```

Recomendado executar comando por comando do script 3.Interativo.sql

Executar script 4.desnormalizacao.sql  
```
\i /var/lib/postgresql/dimensional/data-warehouse-keplo-bikes-master/4.desnormalizacao.sql
```

Executar script 5.kpi.sql  
```
\i /var/lib/postgresql/dimensional/data-warehouse-keplo-bikes-master/5.kpi
```