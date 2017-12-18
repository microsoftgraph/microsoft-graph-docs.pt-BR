# <a name="working-with-webhooks-in-microsoft-graph"></a>Trabalhando com webhooks no Microsoft Graph

A API REST do Microsoft Graph usa um mecanismo de webhook para fornecer notificações aos clientes. Um cliente é um serviço Web que configura sua própria URL para receber notificações. Aplicativos cliente usam notificações para atualizar seu estado após alterações.

Usando a API REST do Microsoft Graph, um aplicativo pode se inscrever para alterações nos seguintes recursos:

* Mensagens
* Eventos
* Contatos
* Conversas em grupo
* Conteúdo compartilhado no OneDrive, incluindo unidades associadas a sites do SharePoint
* Pastas de OneDrive pessoais do usuário

Por exemplo, você pode criar uma assinatura para uma pasta específica: `me/mailfolders('inbox')/messages`

Ou para um recurso de nível superior: `me/messages`, `me/contacts`, `me/events`

Ou em uma unidade do Sharepoint / OneDrive for Business: `/drive/root`

Ou no OneDrive pessoal de um usuário: `/drives/{id}/root`
`/drives/{id}/root/subfolder`

Depois que o Microsoft Graph aceita a solicitação de assinatura, ele envia notificações por push para a URL especificada na assinatura. O aplicativo então realiza ações de acordo com sua lógica comercial. Por exemplo, ele busca mais dados, atualiza o cache e as exibições, etc.

Os aplicativos precisam renovar suas assinaturas antes do tempo de expiração. Caso contrário, será preciso criar uma nova assinatura. Confira a lista de prazos máximos em [Prazo máximo de assinatura por tipo de recurso](subscription.md#maximum-length-of-subscription-per-resource-type).

Os aplicativos também podem cancelar a assinatura a qualquer momento para deixarem de receber notificações.

Em geral, as operações de assinatura exigem permissão de leitura ao recurso. Por exemplo, para obter notificações de mensagens, seu aplicativo precisa da permissão `Mail.Read`. O artigo [criar assinatura](../api/subscription_post_subscriptions.md) lista as permissões necessárias para cada tipo de recurso. A tabela a seguir lista os tipos de permissões que o aplicativo pode solicitar para usar webhooks para tipos específicos de recursos. 

| Tipo de permissão | Tipos de recurso com suporte na v1.0 |
|:----------------|:---------------------------------|
| Delegado - conta corporativa ou de estudante | [contact](contact.md), [conversation](conversation.md), [drive](drive.md), [event](event.md), [message](message.md) |
| Delegado - conta pessoal da Microsoft | Nenhum |
| Aplicativo | [contact](contact.md), [conversation](conversation.md), [event](event.md), [message](message.md) |

## <a name="code-samples"></a>Code samples

Os exemplos de código a seguir estão disponíveis no GitHub.

* [Exemplo de webhooks do Microsoft Graph para Node.js](https://github.com/OfficeDev/Microsoft-Graph-Nodejs-Webhooks)
* [Exemplo de webhooks do Microsoft Graph para ASP,NET](https://github.com/OfficeDev/Microsoft-Graph-ASPNET-Webhooks)

# <a name="creating-a-subscription"></a>Criando uma assinatura

Criar uma assinatura é a primeira etapa para começar a receber notificações de um recurso. O processo de assinatura ocorre da seguinte maneira:

1. O cliente envia uma solicitação de assinatura (POST) para um recurso específico.
2. O Microsoft Graph verifica a solicitação.
  * Se a solicitação for válida, o Microsoft Graph enviará um token de validação para a URL de notificação.
  * Se a solicitação for inválida, o Microsoft Graph enviará uma resposta de erro com um código e detalhes.
3. O cliente enviará o token de validação de volta para o Microsoft Graph.

O cliente deve armazenar a ID da assinatura para correlacionar uma notificação com a assinatura correspondente.

## <a name="notification-url-validation"></a>Validação da URL de notificação

O Microsoft Graph valida a URL de notificação em uma solicitação de assinatura antes de criar a assinatura. O processo de validação ocorre da seguinte maneira:

1. O Microsoft Graph envia uma solicitação POST para a URL de notificação:

  ```
  POST https://{notificationUrl}?validationToken={TokenDefinedByMicrosoftGraph}
  ClientState: {Data sent in ClientState value in subscription request (if any)}
  ```
 
2. O cliente deve fornecer uma resposta com as seguintes características em até 10 segundos:

  * Um código de status 200 (OK).
  * O tipo de conteúdo deve ser texto sem formatação. 
  * O corpo deve incluir o token de validação fornecido pelo Microsoft Graph.

O cliente deve descartar o token de validação depois de o fornecer na resposta.

## <a name="subscription-request-example"></a>Exemplo de solicitação de assinatura

```
POST https://graph.microsoft.com/v1.0/subscriptions
Content-Type: application/json
{
  "changeType": "created,updated",
  "notificationUrl": "https://webhook.azurewebsites.net/notificationClient",
  "resource": "/me/mailfolders('inbox')/messages",
  "expirationDateTime": "2016-03-20T11:00:00.0000000Z",
  "clientState": "SecretClientState"
}
```

As propriedades `changeType`, `notificationUrl`, `resource` e `expirationDateTime` são obrigatórias. Confira os valores e as definições de propriedade em [tipo de recurso de assinatura](subscription.md). Embora a `clientState` não seja obrigatória, você deve incluí-la para manter a conformidade com nosso processo recomendado de manipulação de notificações.

Se tiver êxito, o Microsoft Graph retornará um código `201 Created` e um objeto [subscription](subscription.md) no corpo.

# <a name="renewing-a-subscription"></a>Renovar uma assinatura

O cliente pode renovar uma assinatura com uma data de expiração específica de até três dias desde a hora da solicitação. A propriedade expirationDateTime é obrigatória.

## <a name="subscription-renewal-example"></a>Exemplo de renovação de assinatura

```
PATCH https://graph.microsoft.com/v1.0/subscriptions/{id};
Content-Type: application/json
{
  "expirationDateTime": "2016-03-22T11:00:00.0000000Z"
}
```

Se tiver êxito, o Microsoft Graph retornará um código `200 OK` e um objeto [subscription](subscription.md) no corpo. O objeto subscription inclui o novo valor de expirationDateTime. 

# <a name="deleting-a-subscription"></a>Excluindo uma assinatura

O cliente pode parar de receber notificações excluindo a assinatura com o uso de sua ID.

```
DELETE https://graph.microsoft.com/v1.0/subscriptions/{id}
```

Se tiver êxito, o Microsoft Graph retornará um código `204 No Content`.

# <a name="notifications"></a>Notificações

O cliente começa a receber notificações depois de criar a assinatura. O Microsoft Graph envia uma solicitação POST à URL de notificação quando ocorrem alterações no recurso. O cliente só recebe notificações de acordo com o tipo de alteração especificada, como *created*.

## <a name="notification-properties"></a>Propriedades de notification

O objeto notification tem as seguintes propriedades:

* subscriptionId – A ID da assinatura à qual essa notificação pertence.
* subscriptionExpirationDateTime – O tempo de expiração da assinatura.
* clientState – A propriedade clientState especificada na solicitação de assinatura.
* changeType – O tipo de evento que gerou a notificação. Por exemplo, *created* ao receber um email ou *updated* ao marcar uma mensagem como lida.
* resource – O URI do recurso relativo a `https://graph.microsoft.com`. 
* resourceData – O objeto dependente do recurso que está sendo assinado.  Por exemplo, para recursos do Outlook:
  * @odata.type – O tipo de entidade OData no Microsoft Graph que descreve o objeto representado.
  * @odata.id – O identificador OData do objeto.
  * @odata.etag – A marca da entidade HTTP que representa uma versão do objeto.
  * id – O identificador do objeto.


> Observação: o valor de Id fornecido em resourceData é válido no momento em que a notificação é enfileirada. Algumas ações, como mover uma mensagem para outra pasta, podem resultar na alteração da Id de um recurso. 

## <a name="notification-example"></a>Exemplo de notificação

Quando o usuário recebe um email, o Microsoft Graph envia uma notificação semelhante à seguinte:

```
{
  "value":[
  {
    "subscriptionId":"<subscription_guid>",
    "subscriptionExpirationDateTime":"2016-03-19T22:11:09.952Z",
    "clientState":"SecretClientState",
    "changeType":"Created",
    "resource":"Users/{user_guid}@<tenant_guid>/Messages/{long_id_string}",
    "resourceData":
    {
      "@odata.type":"#Microsoft.Graph.Message",
      "@odata.id":"Users/{user_guid}@<tenant_guid>/Messages/{long_id_string}",
      "@odata.etag":"W/\"CQAAABYAAADkrWGo7bouTKlsgTZMr9KwAAAUWRHf\"",
      "id":"<long_id_string>"
    }
  }
  ]
}
```

Observe que o objeto value contém uma lista. Se houver muitas notificações na fila, o Microsoft Graph as enviará em uma única solicitação.

## <a name="processing-the-notification"></a>Processando a notificação

Depois que o seu aplicativo começar a receber notificações, ele precisa processá-las. Estas são as tarefas mínimas que o seu aplicativo deve realizar para processar uma notificação:

1. Validar a propriedade `clientState`. A propriedade clientState na notificação deve corresponder àquela enviada com a solicitação de assinatura.
  > Observação: se isso não for verdadeiro, você não deve considerá-la uma notificação válida. Você também deve investigar de onde vem a notificação e tomar as medidas apropriadas.

2. Atualize seu aplicativo com base na sua lógica comercial.
3. Envie um código de status `202 - Accepted` na sua resposta para o Microsoft Graph. Se o Microsoft Graph não receber um código de classe 2xx, ele tentará reenviar a notificação várias vezes.
  > Você deve enviar um código de status `202 - Accepted` mesmo que a propriedade clientState não corresponda àquela enviada com a solicitação de assinatura.

Repita o procedimento para outras notificações na solicitação.

# <a name="additional-resources"></a>Recursos adicionais

* [Tipo de recurso de assinatura](subscription.md)
* [Obter assinatura](../api/subscription_get.md)
* [Criar assinatura](../api/subscription_post_subscriptions.md)
* [Exemplo de webhooks do Microsoft Graph para Node.js](https://github.com/OfficeDev/Microsoft-Graph-Nodejs-Webhooks)
* [Exemplo de webhooks do Microsoft Graph para ASP,NET](https://github.com/OfficeDev/Microsoft-Graph-ASPNET-Webhooks)
