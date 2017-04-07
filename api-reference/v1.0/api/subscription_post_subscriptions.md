# <a name="create-subscription"></a>Criar assinatura

Assina um aplicativo de escuta para receber notificações quando os dados no Microsoft Graph são alterados.
## <a name="prerequisites"></a>Pré-requisitos
Um dos seguintes valores de **escopos**, dependendo do recurso de destino, é obrigatório para executar essa API: *Mail.Read*, *Calendars.Read*, *Contacts.Read*, *Group.Read.All*, *Files.ReadWrite* ou *Files.ReadWrite.All*. ***Observação:*** O ponto de extremidade /v1.0 dá permissões do aplicativo para a maioria dos recursos. Não há suporte para conversas em grupo e itens da unidade raiz do OneDrive com permissões de aplicativo.

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->

```http
POST /subscriptions

```

## <a name="request-headers"></a>Cabeçalhos de solicitação
| Nome       | Tipo | Descrição|
|:-----------|:------|:----------|
| Autorização  | string  | <token> de portador. Obrigatório. |


## <a name="response"></a>Resposta
Se for bem-sucedido, esse método retornará um código de resposta `201, Created` e um objeto [subscription](../resources/subscription.md) no corpo da resposta.

## <a name="example"></a>Exemplo
##### <a name="request"></a>Solicitação
Veja a seguir um exemplo da solicitação para enviar uma notificação quando o usuário receber um novo email.
<!-- {
  "blockType": "request",
  "name": "create_subscription_from_subscriptions"
}-->
```http
POST https://graph.microsoft.com/v1.0/subscriptions
Content-type: application/json

{
   "changeType": "created,updated",
   "notificationUrl": "https://webhook.azurewebsites.net/api/send/myNotifyClient",
   "resource": "me/mailFolders('Inbox')/messages",
   "expirationDateTime":"2016-11-20T18:23:45.9356913Z",
   "clientState": "subscription-identifier"
}
```
No corpo da solicitação, forneça uma representação JSON do objeto [subscription](../resources/subscription.md). O campo *clientState* é opcional.

##### <a name="resources-examples"></a>Exemplos de recursos
Estes são os valores válidos da propriedade de recurso da assinatura:

| Tipo de recurso | Exemplos |
|:------ |:----- |
|Email|me/mailfolders('inbox')/messages<br />me/messages|
|Contatos|me/contacts|
|Calendários|me/events|
|Conversas|groups('*{id}*')/conversations|
|Unidades|me/drive/root|

##### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.subscription"
} -->
```http
HTTP/1.1 201 Created

{
  "id":"7f105c7d-2dc5-4530-97cd-4e7ae6534c07",
  "resource":"me/mailFolders('Inbox')/messages",
  "changeType":"created, updated",
  "clientState":"subscription-identifier",
  "notificationUrl":"https://webhook.azurewebsites.net/api/send/myNotifyClient",
  "expirationDateTime":"2016-11-20T18:23:45.9356913Z"
}
```
## <a name="subscription-validation"></a>Validação de assinaturas
Para evitar que assinaturas incorretas direcionem notificações para URLs arbitrárias, o ponto de extremidade de notificação de assinatura deve ser capaz de responder a uma solicitação de validação. Durante o processamento de `POST` para o ponto de extremidade `/subscriptions`, o Microsoft Graph enviará uma solicitação `POST` de volta ao seu `notificationUrl`, da seguinte maneira: 
```http
POST https://webhook.azurewebsites.net/api/send/myNotifyClient?validationToken=<token>
```
O ponto de extremidade de notificação deve enviar uma resposta 200 com o valor de `<token>` como o corpo e um tipo de conteúdo de `text/plain`, conforme mostrado abaixo, dentro de 10 segundos. Caso contrário, a solicitação de criação será descartada.
```http
HTTP/1.1 200 OK
Content-type: text/plain
Content-length: 7
<token>
```
##### <a name="notification-payload"></a>Carga de notificação
Quando o recurso assinado mudar, a as alterações de recurso inscrito, as instalações de webhooks enviarão uma notificação para a URL de notificação com a seguinte carga.  O ponto de extremidade de notificação deve enviar uma resposta de 200 ou 204 sem um corpo de resposta dentro de 30 segundos. Caso contrário, a tentativa de notificação será repetida em intervalos exponencialmente crescentes.  Os serviços que demoram consistentemente 30 segundos ou mais podem ser limitados e recebem um conjunto de notificação mais esparso.

Os serviços também podem retornar uma resposta 422 de uma notificação. Nesse caso, a assinatura será automaticamente excluída, e o fluxo de notificações será interrompido.

Dependendo do recurso assinado, um campo resourceData adicional pode fornecer informações adicionais.

```http
{
   "value":[
      {
         "subscriptionId":"7f105c7d-2dc5-4530-97cd-4e7ae6534c07",
         "subscriptionExpirationDateTime":"2015-11-20T18:23:45.9356913Z",
         "clientState":"subscription-identifier",
         "changeType":"Created",
         "resource":"Users/ddfcd489-628b-7d04-b48b-20075df800e5@1717622f-1d94-c0d4-9d74-f907ad6677b4/messages/AAMkADMxZmEzMDM1LTFjODQtNGVkMC04YzY3LTBjZTRlNDFjNGE4MwBGAAAAAAAr-q_ZG7oXSaqxum7oZW5RBwCoeN6SYXGLRrvRm_CYrrfQAAAAAAEMAACoeN6SYXGLRrvRm_CYrrfQAACvtMe6AAA=",
         "resourceData":{
            "@odata.type":"#Microsoft.Graph.Message",
            "@odata.id":"Users/ddfcd489-628b-7d04-b48b-20075df800e5@1717622f-1d94-c0d4-9d74-f907ad6677b4/messages/AAMkADMxZmEzMDM1LTFjODQtNGVkMC04YzY3LTBjZTRlNDFjNGE4MwBGAAAAAAAr-q_ZG7oXSaqxum7oZW5RBwCoeN6SYXGLRrvRm_CYrrfQAAAAAAEMAACoeN6SYXGLRrvRm_CYrrfQAACvtMe6AAA=",
            "@odata.etag":"W/\"CQAAABYAAACoeN6SYXGLRrvRm+CYrrfQAACvvGdb\"",
            "Id":"AAMkADMxZmEzMDM1LTFjODQtNGVkMC04YzY3LTBjZTRlNDFjNGE4MwBGAAAAAAAr-q_ZG7oXSaqxum7oZW5RBwCoeN6SYXGLRrvRm_CYrrfQAAAAAAEMAACoeN6SYXGLRrvRm_CYrrfQAACvtMe6AAA="
         }
      }
   ]
}
```
Ao receber notificações de assinaturas de Drive, resourceData será nulo, e a API [delta](item_delta.md) deverá ser chamada para determinar as alterações que ocorreram. Veja a seguir um exemplo de notificação de Drive:
```http
{
  "subscriptionId": "aa269f87-2a92-4cff-a43e-2771878c3727",
  "clientState": "My client state",
  "changeType": "updated",
  "resource": "me/drive/root",
  "subscriptionExpirationDateTime": "2016-08-26T23:08:37.00+00:00",
  "resourceData": null
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create subscription",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
