# <a name="create-subscription"></a>Criar assinatura

Assina um aplicativo de escuta para receber notificações quando os dados no Microsoft Graph são alterados.

## <a name="permissions"></a>Permissões

Criar uma assinatura exige escopo de leitura para o recurso. Por exemplo, para obter mensagens de notificações, seu aplicativo precisa da permissão `Mail.Read`. A tabela a seguir lista a permissão sugerida necessária para cada recurso. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).

| Tipo de recurso/item        | Permissão          |
|-----------------------------|---------------------|
| Contatos                    | Contacts.Read       |
| Conversas               | Group.Read.All      |
| Eventos                      | Calendars.Read      |
| Mensagens                    | Mail.Read           |
| Grupos                      | Group.Read.All      |
| Usuários                       | User.Read.All       |
| Drive (o OneDrive do usuário)    | Files.ReadWrite     |
| Unidades (unidades e conteúdo compartilhado do SharePoint) | Files.ReadWrite.All |

 > **Observação:** O ponto de extremidade /v1.0 concede permissões de aplicativo para a maioria dos recursos. Não há suporte para conversas em grupo e itens da unidade raiz do OneDrive com permissões de aplicativo.

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->

```http
POST /subscriptions
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome       | Tipo | Descrição|
|:-----------|:------|:----------|
| Autorização  | sequência de caracteres  | {token} de portador. Obrigatório. |

## <a name="response"></a>Resposta

Se bem-sucedido, este método retorna o código de resposta `201 Created` e um objeto [subscription](../resources/subscription.md) no corpo da resposta.

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
   "clientState": "secretClientValue"
}
```

No corpo da solicitação, forneça uma representação JSON do objeto [subscription](../resources/subscription.md).
O preenchimento do campo `clientState` é opcional.

##### <a name="resources-examples"></a>Exemplos de recursos

Estes são os valores válidos da propriedade de recurso da assinatura:

| Tipo de recurso | Exemplos |
|:------ |:----- |
|Email|me/mailfolders('inbox')/messages<br />me/messages|
|Contatos|me/contacts|
|Calendários|me/events|
|Usuários|users|
|Grupos|groups|
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
Content-type: application/json
Content-length: 252

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#subscriptions/$entity",
  "id": "7f105c7d-2dc5-4530-97cd-4e7ae6534c07",
  "resource": "me/mailFolders('Inbox')/messages",
  "applicationId": "24d3b144-21ae-4080-943f-7067b395b913",
  "changeType": "created,updated",
  "clientState": "secretClientValue",
  "notificationUrl": "https://webhook.azurewebsites.net/api/send/myNotifyClient",
  "expirationDateTime": "2016-11-20T18:23:45.9356913Z",
  "creatorId": "8ee44408-0679-472c-bc2a-692812af3437"
}
```

## <a name="notification-endpoint-validation"></a>Validação de ponto de extremidade de notificação

O ponto de extremidade de notificação de assinatura (especificado na propriedade `notificationUrl`) deve ser capaz de responder a uma solicitação de validação, conforme descrito em [Configurar notificações para alterações nos dados do usuário](../../../concepts/webhooks.md#notification-endpoint-validation). Se a validação falhar, a solicitação para criar a assinatura retornará um erro 400 de solicitação inválida.

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create subscription",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
