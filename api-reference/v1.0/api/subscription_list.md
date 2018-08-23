# <a name="list-subscriptions"></a>Assinaturas de lista

Recupere as propriedades e relações de assinaturas de webhook, com base no ID do aplicativo, no usuário e na função do usuário com um locatário.

## <a name="permissions"></a>Permissões

Essa API suporta os seguintes escopos de permissão; para saber mais, incluindo como escolher permissões, veja [Permissões](../../../concepts/permissions_reference.md).

| Tipo de permissão  | Permissões (da menos para a mais privilegiada)  |
|:---------------- |:-------------------------------------------- |
| [Delegada](../../../concepts/auth_v2_user.md) (conta de estudante ou corporativa) | Função necessária para [criar assinatura](subscription_get.md) ou Subscriptions.Read.All (veja a seguir). |
| [Delegada](../../../concepts/auth_v2_user.md)(conta pessoal da Microsoft) | Função necessária para [criar assinatura](./subscription_get.md) ou Subscriptions.Read.All (veja a seguir). |
| [Aplicativo](../../../concepts/auth_v2_service.md) | Função necessária para [criar assinatura](./subscription_get.md). |

Os resultados de resposta são baseados no contexto do aplicativo de chamada. Apresentamos a seguir um resumo dos cenários comuns:

### <a name="basic-scenarios"></a>Cenários básicos

Mais comumente, um aplicativo deseja recuperar as assinaturas que originalmente criou para o usuário conectado no momento, ou para todos os usuários no diretório (contas de trabalho/escola). Esses cenários não exigem quaisquer permissões especiais além do aplicativo originalmente usado para criar suas assinaturas.

| Contexto do aplicativo de chamada | A resposta conterá |
|:-----|:---------------- |
| O aplicativo está chamando em nome do usuário conectado (permissão delegada). <br/>- e -<br/>O aplicativo tem a permissão original necessária para [ criar a assinatura](subscription_post_subscriptions.md) .<br/><br/>Observação: Isso se aplica às contas pessoais e às contas de trabalho/escola da Microsoft. | Assinaturas criadas por **este aplicativo** apenas para o usuário conectado. |
| O aplicativo está chamando em nome do próprio (permissão de aplicativo).<br/>- e -<br/>O aplicativo tem a permissão original necessária para [ criar a assinatura](subscription_post_subscriptions.md) .<br/><br/>Observação: Isso se aplica apenas a contas de trabalho/escola.| Assinaturas criadas por **este aplicativo** para si mesmo ou para qualquer usuário no diretório.|

### <a name="advanced-scenarios"></a>Cenários avançados

Em alguns casos, um aplicativo deseja recuperar assinaturas criadas por outros aplicativos. Por exemplo, um usuário deseja ver todas as assinaturas criadas por qualquer aplicativo em seu nome. Ou então, um administrador talvez queira ver todas as assinaturas de todos os aplicativos no seu diretório.
Para esses cenários, uma permissão delegada Subscription.Read.All é necessária.

| Contexto do aplicativo de chamada | A resposta conterá |
|:-----|:---------------- |
| O aplicativo está chamando em nome do usuário conectado (permissão delegada). *O usuário não é um administrador*. <br/>- e -<br/>O aplicativo tem a permissão Subscription.Read.All<br/><br/>Observação: Isso se aplica às contas pessoais e às contas de trabalho/escola da Microsoft. | Assinaturas criadas por **qualquer aplicativo** apenas para o usuário conectado. |
| O aplicativo está chamando em nome do usuário conectado (permissão delegada). *O usuário é um administrador*.<br/>- e -<br/>O aplicativo tem a permissão Subscription.Read.All<br/><br/>Observação: Isso se aplica apenas a contas de trabalho/escola. | Assinaturas criadas por **qualquer aplicativo** para **qualquer usuário** no diretório.|

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->

```http
GET /subscriptions
```

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais

Este método não oferece suporte para os [Parâmetros de consulta OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) para ajudar a personalizar a resposta.

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome       | Tipo | Descrição|
|:-----------|:------|:----------|
| Autorização  | sequência de caracteres  | {token} de portador. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação

Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um `200 OK` código de resposta e uma lista de objetos de [assinatura](../resources/subscription.md) no corpo da resposta.

## <a name="example"></a>Exemplo

##### <a name="request"></a>Solicitação

<!-- {
  "blockType": "request",
  "name": "get_subscriptions"
}-->

```http
GET https://graph.microsoft.com/v1.0/subscriptions
```

##### <a name="response"></a>Resposta

Aqui está um exemplo da resposta.  Observe que ele pode estar truncado para fins de concisão.  Todas as propriedades apropriadas suportadas para a solicitação e o contexto de chamada serão retornadas de uma chamada real.

<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.subscription",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 586

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#subscriptions",
  "value": [
    {
      "id": "0fc0d6db-0073-42e5-a186-853da75fb308",
      "resource": "Users",
      "applicationId": "24d3b144-21ae-4080-943f-7067b395b913",
      "changeType": "updated,deleted",
      "clientState": null,
      "notificationUrl": "https://webhookappexample.azurewebsites.net/api/notifications",
      "expirationDateTime": "2018-03-12T05:00:00Z",
      "creatorId": "8ee44408-0679-472c-bc2a-692812af3437"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List subscriptions",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

Quando uma solicitação retorna várias páginas de dados, a resposta inclui uma `@odata.nextLink` propriedade para ajudá-lo a gerenciar os resultados.  Para saber mais, veja [Dados de paginação do Microsoft Graph em seu aplicativo](../../../concepts/paging.md).
