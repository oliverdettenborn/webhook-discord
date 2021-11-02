# O que são webhooks e para que eles servem ?

<p>
  Sabe aquela série sua favorita que você está contando os dias para saber quando vai ser lançada? Para saber se já está disponível, você vai na página do streaming e ver se ela já está disponível. Mas não seria ótimo se você não precisasse ficar ativamente indo atrás dessa informação e quando estivesse disponível algo te avisa-se? Então, isso é um webhook 😊
</p>

<p>
  Webhooks é uma forma de recebimento de informações de um programa que são enviadas quando um evento acontece. Por exemplo, você poderia ter um webhook que te avisa no slack quando uma nova série é lançada. Ele é uma maneira prática de um aplicativo seu receber informações em tempo real de eventos que acontecem em outros programas. Existem diversas formas de implementar um webhook e ele pode ser usado em diversos cenários dependendo do problema que você está buscando resolver.
</p>

### Ficou curioso e quer criar seu primeiro webhook hoje?

<p>
  Vamos criar o seguinte webhook, vamos escolher um repositório qualquer no seu github. Sempre que ele sofrer alguma mudança, algo acontecer nele, gostariamos de ser avisados em um canal de um servidor discord. Beleza?
</p>

<ol>
  <li>No servidor escolhido, crie um canal de texto chamado github. E vamos abrir as configurações dele.</li>
  <img src="/images/step-1.png" />
  <br>

  <li>Vamos agora no menu integrações, e clicar em criar webhook. Vamos dar um nome para ele, salvar as alterações, e então copiar a url do webhook</li>
  <img src="/images/step-2.png" />
  <br>

  <li>Com a url em mão, você vai lá no repositório que escolheu e entra nas configurações dele. E entra no menu webhooks e clica em adicionar um novo webhook.</li>
  <img src="/images/step-3.png" />
  <br>

  <li>No campo payload URL vamos adicionar o link que copiamos lá do discord adicionando ao final do link um /github. No content-type vamos escolher “application/json”, para ele nos mandar um objeto JSON. E no campo de quais eventos queremos receber, escolhemos “send me everything”. E clicamos em adicionar, e está pronto :)</li>
  <img src="/images/step-4.png" />
  <br>

  <li>Vou fazer um commit no repositório e testar se ele está me avisando… E vemos a magia acontecer no discord</li>
  <img src="/images/step-5.png" />
</ol>

<div align="center">
  <img src="/images/party-parrot.gif" width="50px">
</div>

----------------------------------------------------------------
<a href="https://support.discord.com/hc/pt-br/articles/228383668-Usando-Webhooks">
  Documentação de referência
</a>
