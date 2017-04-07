# <a name="working-with-webhooks-in-microsoft-graph"></a>Trabalhando com webhooks no Microsoft Graph

A API REST do Microsoft Graph usa um mecanismo de webhook para fornecer notificações aos clientes. Um cliente é um serviço Web que configura sua própria URL para receber notificações. Aplicativos cliente usam notificações para atualizar seu estado após alterações.

Usando a API REST do Microsoft Graph, um aplicativo pode se inscrever para alterações nos seguintes recursos:

* Mensagens
* Eventos
* Contatos
* Conversas em grupo
* Itens raiz de unidade

Depois que o Microsoft Graph aceita a solicitação de assinatura, ele envia notificações por push para a URL especificada na assinatura. O aplicativo então realiza ações de acordo com sua lógica comercial. Por exemplo, ele busca mais dados, atualiza o cache e as exibições, etc.

Os aplicativos devem renovar suas assinaturas antes de expirarem. Eles também podem cancelar a assinatura a qualquer momento para deixarem de receber notificações.

Veja os exemplos de código a seguir no GitHub.

* [Exemplo de webhooks do Microsoft Graph para Node.js](https://github.com/OfficeDev/Microsoft-Graph-Nodejs-Webhooks)
* [Exemplo de webhooks do Microsoft Graph para ASP,NET](https://github.com/OfficeDev/Microsoft-Graph-ASPNET-Webhooks)

Vamos examinar o processo de assinatura.

# <a name="creating-a-subscription"></a>Criando uma assinatura

Criar uma assinatura é a primeira etapa para começar a receber notificações de um recurso. O processo de assinatura ocorre da seguinte maneira:

1. O cliente envia uma solicitação de assinatura (POST) para um recurso específico.
2. O Microsoft Graph verifica a solicitação.
  * Se a solicitação for válida, o Microsoft Graph enviará um token de validação para a URL de notificação.
  * Se a solicitação for inválida, o Microsoft Graph enviará uma resposta de erro com um código e detalhes.
3. O cliente enviará o token de validação de volta para o Microsoft Graph.

O cliente deve armazenar a ID da assinatura para correlacionar uma notificação com a assinatura correspondente.

## <a name="characteristics-of-subscriptions"></a>Características de assinaturas

Você pode criar assinaturas para recursos, como mensagens, eventos, contatos e itens de raiz de unidade.

Você pode criar uma assinatura para uma pasta específica: `https://graph.microsoft.com/v1.0/me/mailfolders('inbox')/messages`

Ou para um recurso de nível superior: `https://graph.microsoft.com/v1.0/me/messages`

Ou em um item raiz de unidade: `https://graph.microsoft.com/v1.0/me/drive/root`

Na maioria dos casos, criar uma assinatura exige escopo de leitura para o recurso. Por exemplo, para obter mensagens de notificações, seu aplicativo precisa da permissão `mail.read`. Observe que, atualmente, a permissão `Files.ReadWrite` é obrigatória para itens raiz de unidade do OneDrive, enquanto unidades associadas a sites do SharePoint exigem `Files.ReadWrite.All`.

Assinaturas possuem uma data de expiração. O tempo de expiração mais longo é de três dias menos 90 a 4230 minutos do tempo de criação. Os aplicativos precisam renovar suas assinaturas antes do tempo de expiração. Caso contrário, eles precisarão criar uma nova assinatura.

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

As propriedades changeType, notificationUrl, resource e expirationDateTime são obrigatórias. Confira [Tipo de recurso de assinatura](subscription.md) para valores e definições de propriedade. Embora clientState não seja obrigatória, você deve incluí-la para manter a conformidade com nosso processo recomendada de manipulação de notificações.

Se tiver êxito, o Microsoft Graph retornará um código `200 OK` e um objeto [subscription](subscription.md) no corpo.

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

* id – A ID da assinatura à qual essa notificação pertence.
* expirationDateTime – O tempo de expiração da assinatura.
* clientState – A propriedade clientState especificada na solicitação de assinatura.
* changeType – O tipo de evento que gerou a notificação. Por exemplo, *created* ao receber um email ou *updated* ao marcar uma mensagem como lida.
* resource – O URI do recurso relativo a `https://graph.microsoft.com`. 
* resourceData – O objeto dependente do recurso que está sendo assinado.  Por exemplo, para recursos do Outlook:
  * @odata.type – O tipo de entidade OData no Microsoft Graph que descreve o objeto representado.
  * @odata.id – O identificador OData do objeto.
  * @odata.etag – A marca de entidade HTTP que representa uma versão do objeto.
  * Id – O identificador do objeto.


> Observação: O valor de Id fornecido em resourceData é válido no momento em que a notificação é enfileirada. Algumas ações, como mover uma mensagem para outra pasta, podem resultar na alteração da Id de um recurso. 

## <a name="notification-example"></a>Exemplo de notificação

Quando o usuário recebe um email, o Microsoft Graph envia uma notificação semelhante à seguinte:

```
{
  "value":[
  {
    "id":"<subscription_guid>",
    "expirationDateTime":"\"2016-03-19T22:11:09.952Z\"",
    "clientState":"SecretClientState",
    "changeType":"Created",
    "resource":"Users/{user_guid}@<tenant_guid>/Messages/{long_id_string}",
    "resourceData":
    {
      "@odata.type":"#Microsoft.Graph.Message",
      "@odata.id":"Users/{user_guid}@<tenant_guid>/Messages/{long_id_string}",
      "@odata.etag":"W/\"CQAAABYAAADkrWGo7bouTKlsgTZMr9KwAAAUWRHf\"",
      "Id":"<long_id_string>"
    }
  }
  ]
}
```

Observe que o objeto value contém uma lista. Se houver muitas notificações na fila, o Microsoft Graph as enviará em uma única solicitação.

## <a name="processing-the-notification"></a>Processando a notificação

Depois que o seu aplicativo começar a receber notificações, ele precisa processá-las. Estas são as tarefas mínimas que o seu aplicativo deve realizar para processar uma notificação:

1. Validar a propriedade `clientState`. A propriedade clientState na notificação deve corresponder àquela enviada com a solicitação de assinatura.
  > Observação: Se isso não for verdadeiro, você não deve considerá-la uma notificação válida. Você também deve investigar de onde vem a notificação e tomar as medidas apropriadas.

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
