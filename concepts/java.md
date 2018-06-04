# <a name="get-started-with-microsoft-graph-in-a-java-app"></a>Introdução ao Microsoft Graph em aplicativo Java

Este artigo usa o [console-java-connect-sample](https://github.com/microsoftgraph/console-java-connect-sample) para explicar o envio de emails por meio do Microsoft Graph em um aplicativo de console Java. O artigo mostra o código que é preciso incluir no aplicativo Java para poder usar a API do Microsoft Graph. O aplicativo acessa o Microsoft Graph usando o [SDK do Microsoft Graph para Java](https://github.com/microsoftgraph/msgraph-sdk-java).

## <a name="choose-an-authentication-library"></a>Escolher uma biblioteca de autenticação

O Microsoft Graph adotou os padrões do OAuth 2.0 e do Open ID Connect, que permite escolher entre várias bibliotecas OAuth 2 para Java de software livre. A equipe do Azure AD recomenda usar o [ScribeJava](https://github.com/scribejava/scribejava), uma biblioteca OAuth2 simples para Java.

O exemplo implementa o fluxo de Concessão do Código de Autorização, que é a escolha certa para o cenário de autorização de cliente, um usuário, e um ponto de extremidade habilitado do OAuth 2 habilitado. Em aplicativos Java de produção de servidor-a-servidor, é usado o fluxo de autorização de Credenciais de Cliente. O **ScribeJava** controla ambos os fluxos de autorização. Para facilitar o registro, a autenticação e a execução deste exemplo, demonstraremos o fluxo mais simples.

Antes de seu aplicativo poder fazer chamadas no Microsoft Graph, ele deve conseguir acessar um token do Azure Active Directory (Azure AD). Este token deve estar presente em um cabeçalho de autenticação HTTP com cada chamada para o Microsoft Graph. O **SDK do Microsoft Graph** é responsável por inserir o cabeçalho e adicionar o token para cada chamada quando você implementa o [IAuthenticationProvider](https://github.com/microsoftgraph/msgraph-sdk-java/blob/dev/src/main/java/com/microsoft/graph/authentication/IAuthenticationProvider.java). O **ScribeJava** controla a autenticação e a obtenção do token de acesso. O aplicativo fornece o token de acesso ao SDK do Microsoft Graph por meio da interface **IAuthenticationProvider**.

## <a name="install-and-run-the-sample"></a>Instalar e executar o exemplo

Para instalar e configurar o aplicativo de exemplo, siga as instruções no documento [Leia-me](https://github.com/microsoftgraph/console-java-connect-sample/blob/master/README.md) no repositório **console-java-connect-sample** no GitHub. Você pode clonar o exemplo e examinar o código em seu Java IDE favorito usando este comando para clonar repositório:

```
git@github.com:microsoftgraph/console-java-connect-sample.git
```

Quando você [registra o aplicativo do Console do Java de Conexão](https://github.com/microsoftgraph/console-java-connect-sample/blob/master/README.md#register-your-app), atribui escopos delegados (permissões) ao exemplo. Certifique-se de que os escopos estejam conforme mostrado na imagem a seguir:

![Permissões de exemplo do Console do Java de Conexão](../concepts/images/console-java-connnect-sample-permissions.JPG)

Depois de registrar o aplicativo e [configurar o exemplo](https://github.com/microsoftgraph/console-java-connect-sample/blob/master/README.md#configure-your-app) quanto à **ID do aplicativo** que obteve no registro do aplicativo, será possível criar e executar o exemplo.

## <a name="console-java-connect-code"></a>Código do Console-Java-Connect 

Antes de observar o fluxo lógico do exemplo, reserve alguns minutos para obter mais informações sobre a [estrutura do projeto do exemplo](#sample-project-structure). Quando estiver tudo pronto, vamos explorar passo a passo a lógica do exemplo:


   
### <a name="walk-through-the-code"></a>Examinar o código
Examinaremos o código do exemplo de forma acurada e aprofundarmos os detalhes de como criar uma mensagem de email e enviá-la.

#### <a name="the-user-experience"></a>A experiência do usuário

Esta seção aborda a lógica que inicia o aplicativo e, em seguida, mostra o exemplo de saída que o usuário vê quando ele executa o exemplo.

O método estático **principal** [PublicClient](https://github.com/microsoftgraph/console-java-connect-sample/blob/master/src/main/java/com/microsoft/graphsample/PublicClient.java) cria uma instância de **PublicClient** e então inicia o processo de entrada e autenticação.  

O [AuthenticationManager](https://github.com/microsoftgraph/console-java-connect-sample/blob/master/src/main/java/com/microsoft/graphsample/connect/AuthenticationManager) fornece uma instância singleton que é usada para conectar o usuário ao Microsoft Graph. O **AuthenticationManager** expõe um **token de acesso** como uma propriedade de cadeia de caracteres. O **Azure AD** retorna o token de acesso quando o usuário é autenticado e fornece a permissão para o exemplo acessar os recursos solicitados no Microsoft Graph. 

O método **PublicClient.startSendMail** executa as seguintes etapas:

- Cria uma nova instância da classe [GraphSendMail](https://github.com/microsoftgraph/console-java-connect-sample/blob/master/src/main/java/com/microsoft/graphsample/msgraph/GraphSendMail.java). 
- Chama **GraphSendMail.getMeUser()** para retornar o perfil do usuário atual do **Azure AD** para que o objeto do console do exemplo possa personalizar os prompts que são exibidos ao usuário. 
- O console exibe:

   `Hello, Laura Steele. Would you like to send an email to yourself or someone else?`

   `Enter the address to which you'd like to send a message. If you enter nothing, the message will go to your address`

- Chama o método **GraphSendMail.sendMail** que leva a entrada do usuário. Se for fornecido um endereço de email, **sendMail** envia uma mensagem para esse endereço. Caso contrário, a mensagem é enviada para o usuário atual. 

- Solicita ao usuário que envie outro email ou feche o aplicativo do console.

   `Email sent!`

   `Want to send another message? Type 'y' for yes and any other key to exit.`

#### <a name="the-send-mail-logic"></a>A lógica para envio de email

A lógica para envio de email contém as seguintes etapas:



1. **Obter imagem do perfil**:<br/> Chama **GraphServiceController.getUserProfilePicture()** para obter uma matriz de bytes que representa a imagem do perfil do usuário do **Azure AD** que entrou no aplicativo de exemplo.

   **A chamada de API**

```java
            photoStream = mGraphServiceClient
                    .me()
                    .photo()
                    .content()
                    .buildRequest()
                    .get();

```
2. **Carregar imagem no OneDrive**:
<br/>Chama **GraphServiceController.uploadPictureToOneDrive(bytes)** para POSTAR a imagem de perfil na pasta-raiz do OneDrive do usuário. O objeto **DriveItem** da SDK do Microsoft Graph retorna. 

   **A chamada de API**
```java
            driveItem = mGraphServiceClient
                    .me()
                    .drive()
                    .root()
                    .itemWithPath("me2.png")
                    .content()
                    .buildRequest()
                    .put(picture);

```
3. **Obter o link de compartilhamento do OneDrive para a imagem**:<br/>Chama **GraphServiceController.getPermissionSharingLink** para criar um novo link de compartilhamento. O objeto **Permission** da SDK do Microsoft Graph é retornado.

   **A chamada de API**
```java
            permission = mGraphServiceClient
                    .me()
                    .drive()
                    .items(id)
                    .createLink("view", "organization")
                    .buildRequest()
                    .post();

```
4. **Substituir o conteúdo da marca de ancoragem do modelo HTML ** com o **webUrl** para o link de compartilhamento na etapa anterior. 
> **Observação:** o corpo da mensagem enviada pelo aplicativo origina-se como um modelo HTML armazenado no [Constants.java](https://github.com/microsoftgraph/console-java-connect-sample/blob/master/src/main/java/com/microsoft/graphsample/connect/Constants.java) como uma cadeia de caracteres estática. Quando enviado, o corpo da mensagem contém um hiperlink de compartilhamento público para uma imagem que o exemplo carrega na pasta-raiz do usuário do OneDrive. 
5. **Criar uma mensagem de rascunho**: <br/>Chama **GraphServiceController.createDraftMail**, passando o endereço de email do destinatário, texto do assunto e o modelo HTML atualizado. Uma mensagem de rascunho é criada e POSTada na pasta de mensagem de rascunho do usuário.

   **A chamada de API**
```java
            message = mGraphServiceClient
                    .me()
                    .messages()
                    .buildRequest()
                    .post(message);

```
6. **Anexar imagem à mensagem de rascunho**: <br/>Chama **GraphServiceController.addPictureToDraftMessage** para obter a mensagem de rascunho e adicionar a imagem à mensagem como um anexo de objeto.

   **A chamada de API**
```java
            FileAttachment fileAttachment = new FileAttachment();
            fileAttachment.oDataType = "#microsoft.graph.fileAttachment";
            fileAttachment.contentBytes = attachementBytes;
            fileAttachment.name = "me.png";
            fileAttachment.size = attachementBytes.length;
            fileAttachment.isInline = false;
            fileAttachment.id = "my profile picture";

            attachment = mGraphServiceClient
                    .me()
                    .messages(messageId)
                    .attachments()
                    .buildRequest()
                    .post(fileAttachment);

```
7. **Envia a mensagem de rascunho**:<br/>Chama **GraphServiceController.sendDraftMessage** para enviar a mensagem de rascunho atualizada para o usuário pretendido.

   **A chamada de API**
```java
            mGraphServiceClient
                    .me()
                    .mailFolders("Drafts")
                    .messages(messageId)
                    .send()
                    .buildRequest()
                    .post();

```



### <a name="sample-project-structure"></a>Estrutura do projeto do exemplo

### <a name="connect-package"></a>pacote connect
Esse pacote contém a lógica do fluxo de autenticação OAuth2 e a configuração será atualizada.

- [AuthenticationManager.java](https://github.com/microsoftgraph/console-java-connect-sample/blob/master/src/main/java/com/microsoft/graphsample/connect/AuthenticationManager.java): esta classe importa os objetos **ScribeJava** usados para o fluxo de Concessão do Código de Autorização.
- [Constants.java](https://github.com/microsoftgraph/console-java-connect-sample/blob/master/src/main/java/com/microsoft/graphsample/connect/Constants.java): mantém cadeias de caracteres estáticas públicas para fornecer valores relacionados ao registro e ao modelo para a mensagem de email que o aplicativo envia.
- [Debug.Java](https://github.com/microsoftgraph/console-java-connect-sample/blob/master/src/main/java/com/microsoft/graphsample/connect/Debug.java): sinalizador de nível de depurador público. Definir o valor dele para alterar o comportamento de registro no log do aplicativo de exemplo.
- [DebugLogger.java](https://github.com/microsoftgraph/console-java-connect-sample/blob/master/src/main/java/com/microsoft/graphsample/connect/DebugLogger.java): utilitário de log que grava informações no console de acordo com o conjunto de nível de depuração.
- [IConnectCallback](https://github.com/microsoftgraph/console-java-connect-sample/blob/master/src/main/java/com/microsoft/graphsample/connect/IConnectCallback.java): define o método de retorno de chamada que você usaria para chamar a sobrecarga assíncrona do método **ScribeJava.getAccessToken**.
- [SendMailException](https://github.com/microsoftgraph/console-java-connect-sample/blob/master/src/main/java/com/microsoft/graphsample/msgraph/SendMailException.java): uma classe derivada da **Exceção** que encapsula informações de exceção específicas do Microsoft Graph. As classes no pacote **GraphSendMail** podem gerar esse tipo de exceção.

### <a name="msgraph-package"></a>pacote msgraph

Esse pacote contém toda a lógica que faz chamadas no Microsoft Graph.

- [GraphSendMail](https://github.com/microsoftgraph/console-java-connect-sample/blob/master/src/main/java/com/microsoft/graphsample/msgraph/GraphSendMail.java): vincula chamadas no **GraphServiceController** (uma classe auxiliar do exemplo da API do Microsoft Graph) para criar e enviar uma mensagem de email com um anexo de imagem.
- [GraphServiceClientManager.java](https://github.com/microsoftgraph/console-java-connect-sample/blob/master/src/main/java/com/microsoft/graphsample/msgraph/GraphServiceClientManager.java): cria a instância do SDK do Microsoft Graph [GraphServiceClient](https://github.com/microsoftgraph/msgraph-sdk-java/blob/dev/src/main/java/com/microsoft/graph/requests/extensions/GraphServiceClient.java) e adiciona um token de acesso para todas as chamadas da API de saída no ponto de extremidade do Microsoft Graph.

- [GraphServiceController.java](https://github.com/microsoftgraph/console-java-connect-sample/blob/master/src/main/java/com/microsoft/graphsample/msgraph/GraphServiceController.java): usa o SDK do Microsoft Graph para fazer todas as chamadas no **GraphServiceClient**. As chamadas incluem:

   - **createDraftMail**: cria uma mensagem de rascunho e a salva na pasta de mensagens de rascunho.
   - **sendNewMessageAsync**: cria e envia uma mensagem de email.
   - **addPictureToDraftMessage**: posta um anexo de arquivo a uma mensagem de rascunho por ID da mensagem
   - **addAttachmentToDraftAsync**: adiciona um anexo a uma mensagem de rascunho.
   - **sendDraftMessage**: envia uma mensagem da pasta de Rascunhos.
   - **getDraftMessage**: recebe uma mensagem da coleção de mensagens do usuário por ID da mensagem.
   - **getUser**: obtém o usuário local que é autenticado com o ponto de extremidade da API do Microsoft Graph.
   - **getUserProfilePicture**: obtém, do Microsoft Graph, a foto de perfil do usuário que entrou.
   - **uploadPictureToOneDrive**: carrega uma imagem como a matriz de bytes para a pasta-raiz do OneDrive do usuário.
   - **getPermissionSharingLink**: solicita ao OneDrive a criação de um link de compartilhamento público para uma imagem armazenada no OneDrive.

## <a name="other-microsoft-graph-samples"></a>Outros exemplos do Microsoft Graph

[Envie uma questão](https://github.com/microsoftgraph/console-java-connect-sample/issues) para nos informar sobre uma amostra específica que você queira ver. Gostaríamos de ouvir seus comentários sobre qualquer evento do Microsoft Graph que você queira criar no Java!

A API do Microsoft Graph é uma API unificadora muito poderosa que pode ser usada para interagir com todos os tipos de dados da Microsoft. Confira a [documentação de desenvolvedor](https://developer.microsoft.com/pt-BR/graph/docs/concepts/overview) ou o [Explorador do Graph](https://developer.microsoft.com/pt-BR/graph/graph-explorer) para explorar o que mais você pode realizar com o Microsoft Graph.
