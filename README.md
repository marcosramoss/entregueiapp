# Entreguei App

Aplicativo simples para entregadores registrarem entregas e acompanharem os ganhos do dia. Funciona diretamente no navegador, sem cadastro ou instalação.

## Funcionalidades

- Cadastro de bairros com o valor recebido por entrega.
- Edição e exclusão de bairros.
- Configuração de um valor de diária e opção para somá-lo ao total recebido.
- Registro de entregas com data, horário e valor do bairro selecionado.
- Resumo diário da quantidade de entregas e do total recebido.
- Consulta de entregas por data.
- Exclusão individual de entregas ou limpeza de todas as entregas de uma data.
- Exportação dos dados para um arquivo JSON e importação de um backup.

## Como usar

1. Abra o arquivo `index.html` em um navegador atualizado.
2. Acesse **Bairros** e cadastre cada bairro e o valor pago por entrega.
3. Opcionalmente, informe o valor da diária em **Bairros** e marque **Somar a diária ao total recebido**.
4. Na aba **Entregas**, selecione um bairro e clique em **Adicionar entrega**.
5. Use o campo de data no topo para consultar ou registrar entregas em outra data.

O total exibido considera somente as entregas da data selecionada e, se ativada, soma uma vez o valor da diária. O valor da diária e a opção de inclusão são salvos junto com os dados do app. O valor e o nome do bairro também são guardados no registro da entrega; alterações ou exclusões posteriores do cadastro do bairro não alteram entregas já registradas.

## Dados e backup

Os dados ficam salvos no armazenamento local (`localStorage`) do navegador e do dispositivo em que o app foi aberto. Eles não são sincronizados entre dispositivos ou navegadores. Limpar os dados do navegador pode removê-los.

Para guardar ou transferir seus dados:

1. Na aba **Bairros**, clique em **Exportar** para baixar um backup JSON.
2. Para restaurá-lo, clique em **Importar** e selecione o arquivo. A importação substitui os dados atuais.

## Tecnologias

- HTML, CSS e JavaScript, sem etapa de build.
- Ícones Lucide carregados por CDN; é necessária conexão com a internet para carregá-los.
