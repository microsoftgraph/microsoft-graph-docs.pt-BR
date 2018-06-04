# <a name="share-outlook-message-folders-between-users"></a>Compartilhar pastas de mensagens do Outlook entre usuários

<!-- remove similar content in other topics when ready to publish - list messages, get message, get mail folder.
These topics also have similar section - list events, get event, get calendar, list contacts, get contact, get contact folder.
-->

O Outlook permite que clientes compartilhem pastas entre si e forneçam acesso para ler, criar ou modificar pastas individuais ou a caixa de correio inteira. Isso também é conhecido como "delegação" no Outlook.

O Microsoft Graph oferece suporte de forma programática para receber mensagens em pastas de email que foram compartilhadas por outros usuários, além de receber as pastas compartilhadas em si.

Por exemplo, Henrique compartilhou com Diogo sua caixa de entrada com acesso de leitura. Se Diogo estiver conectado em seu aplicativo e tiver fornecido permissões delegadas (Mail.Read.Shared ou Mail.ReadWrite.Shared), o aplicativo poderá acessar o email e a caixa de entrada do Henrique conforme descrito abaixo.

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

Se Henrique não tiver compartilhado a pasta de mensagens dele com Diogo nem delegado a caixa de correio dele a Diogo, a especificação da ID de usuário do Henrique ou do nome de entidade de segurança nessas operações GET retornará um erro. 


## <a name="next-steps"></a>Próximas etapas

Saiba mais sobre:

- [Por que integrar-se com o email do Outlook](outlook-mail-concept-overview.md)
- [Como usar a API de email](../api-reference/v1.0/resources/mail_api_overview.md) e seus [casos de uso](../api-reference/v1.0/resources/mail_api_overview.md#common-use-cases) do Microsoft Graph versão 1.0.