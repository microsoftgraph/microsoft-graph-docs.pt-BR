# <a name="get-outlook-messages-in-a-shared-or-delegated-folder"></a>Obter mensagens do Outlook em uma pasta compartilhada ou delegada

<!-- remove similar content in other topics when ready to publish - list messages, get message, get mail folder.
These topics also have similar section - list events, get event, get calendar, list contacts, get contact, get contact folder.
-->

Permite que os clientes do Outlook compartilhem pastas de email entre si e fornece acesso para "ler", "criar", "modificar" ou "excluir" pastas individuais. O Outlook também permite que um cliente delegue a outro usuário permissão para agir em seu nome e acessar pastas de email específicas ou toda a caixa de correio do cliente; Isso também é conhecido como "delegação" no Outlook.

O Microsoft Graph oferece suporte de forma programática para receber mensagens em pastas de email que foram compartilhadas por outros usuários, além de receber as pastas compartilhadas em si. O suporte também se aplica às pastas que foram delegadas.

Por exemplo, Garth compartilhou a sua caixa de entrada com John e lhe deu acesso de leitura. Se John estiver conectado no seu aplicativo e tiver fornecido permissões delegadas (Mail.Read.Shared ou Mail.ReadWrite.Shared), o seu aplicativo poderá acessar o email e a caixa de entrada de Garth, conforme descrito abaixo.

## <a name="get-a-message-in-the-shared-folder"></a>Obter uma mensagem na pasta compartilhada

Você pode obter uma mensagem específica na caixa de entrada do Henrique:

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/mailfolders('Inbox')/messages/{id}
```

Após a conclusão bem-sucedida, você receberá HTTP 200 OK e a instância de [message](../api-reference/v1.0/resources/message.md) identificada por `{id}` da caixa de entrada do Henrique.

## <a name="get-all-messages-in-the-shared-folder"></a>Obter todas as mensagens na pasta compartilhada

Obtenha todas as mensagens na caixa de entrada do Henrique:

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/mailfolders('Inbox')/messages
```

Após a conclusão bem-sucedida, você receberá HTTP 200 OK um conjunto de instâncias de [message](../api-reference/v1.0/resources/message.md) na caixa de entrada do Henrique.

## <a name="get-the-shared-folder"></a>Obter a pasta compartilhada

Obtenha a pasta (caixa de entrada) que Henrique compartilhou com Diogo.

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/mailfolders('Inbox')
```

Após a conclusão bem-sucedida, você receberá HTTP 200 OK e uma instância de [mailFolder](../api-reference/v1.0/resources/mailfolder.md) que representa a pasta de caixa de entrada do Henrique.

Os mesmos recursos de GET se aplicam se Henrique delegar a Diogo mais acesso à sua caixa de entrada ou se Henrique delegar toda a sua caixa de correio a Diogo.

Se Garth não tiver compartilhado sua caixa de entrada com John, nem delegado sua caixa de correio para John, especificar a identificação de usuário de Garth ou nome UPN nessas operações GET retornará um erro. 


## <a name="next-steps"></a>Próximas etapas

Saiba mais sobre:

- [Por que integrar-se com o email do Outlook](outlook-mail-concept-overview.md)
- [Como usar a API de email](../api-reference/v1.0/resources/mail_api_overview.md) e seus [casos de uso](../api-reference/v1.0/resources/mail_api_overview.md#common-use-cases) do Microsoft Graph versão 1.0.