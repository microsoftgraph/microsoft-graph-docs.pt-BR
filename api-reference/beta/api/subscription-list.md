---
title: Listar assinaturas
description: " consulte os cenários abaixo para obter detalhes."
ms.localizationpriority: medium
author: Jumaodhiss
doc_type: apiPageType
ms.prod: change-notifications
ms.openlocfilehash: 2a4bb437b039d591babe911e5b2ea0dd2f0fecfc
ms.sourcegitcommit: 0759717104292bda6012dd2e9e3a362567aa2b64
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/12/2021
ms.locfileid: "60947137"
---
# <a name="list-subscriptions"></a>Listar assinaturas

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Recupere uma lista de assinaturas de webhook. O conteúdo da resposta depende do contexto no qual o aplicativo está chamando; consulte os cenários abaixo para obter detalhes.

## <a name="permissions"></a>Permissões

Esta API suporta os seguintes escopos de permissão; para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

| Tipo de permissão  | Permissões (da com menos para a com mais privilégios)  |
|:---------------- |:-------------------------------------------- |
| [Delegada](/graph/auth-v2-user) (conta de trabalho ou de estudante) | Permissão necessária para criar [assinatura ou](subscription-post-subscriptions.md) Subscription.Read.All (consulte abaixo). |
| [Delegada](/graph/auth-v2-user) (conta pessoal da Microsoft) | Permissão necessária para criar [assinatura ou](subscription-post-subscriptions.md) Subscription.Read.All (consulte abaixo). |
| [Aplicativo](/graph/auth-v2-service) | Permissão necessária para criar [assinatura](subscription-post-subscriptions.md). |

Os resultados da resposta são baseados no contexto do aplicativo de chamada. A seguir, um resumo dos cenários comuns:

### <a name="basic-scenarios"></a>Cenários Básicos

Comumente, um aplicativo deseja recuperar assinaturas originalmente criadas para o usuário atualmente conectado ou para todos os usuários no diretório (contas corporativas/de estudante). Esses cenários não exigem permissões especiais além daquelas usadas originalmente pelo aplicativo para criar suas assinaturas.

| Contexto do aplicativo de chamada | A resposta contém |
|:-----|:---------------- |
| O aplicativo está chamando em nome do usuário conectado (permissão delegada). <br/>-e-<br/>O aplicativo tem a permissão original necessária para [criar a assinatura](subscription-post-subscriptions.md).<br/><br/>Nota: Isso se aplica a contas pessoais da Microsoft e contas de trabalho/escola. | Assinaturas criadas por **este aplicativo** apenas para o usuário conectado. |
| O aplicativo está chamando em nome de si mesmo (permissão de aplicativo).<br/>-e-<br/>O aplicativo tem a permissão original necessária para [criar a assinatura](subscription-post-subscriptions.md).<br/><br/>Nota: Isso se aplica apenas a contas de trabalho/escola.| Assinaturas criadas por **este aplicativo** para si ou para qualquer usuário no diretório.|

### <a name="advanced-scenarios"></a>Cenários avançados

Em alguns casos, um aplicativo deseja recuperar assinaturas criadas por outros aplicativos. Por exemplo, um usuário deseja ver todas as assinaturas criadas por qualquer aplicativo em seu nome. Ou, um administrador pode querer ver todas as assinaturas de todos os aplicativos em seu diretório.
Para esses cenários, é necessária uma permissão delegada Subscription.Read.All.

| Contexto do aplicativo de chamada | A resposta contém |
|:-----|:---------------- |
| O aplicativo está chamando em nome do usuário conectado (permissão delegada). *O usuário é um não administrador*. <br/>-e-<br/>O aplicativo tem a permissão Subscription.Read.All<br/><br/>Nota: Isso se aplica a contas pessoais da Microsoft e contas de trabalho/escola. | Assinaturas criadas por **qualquer aplicativo** apenas para o usuário conectado. |
| O aplicativo está chamando em nome do usuário conectado (permissão delegada). *O usuário é um administrador*.<br/>-e-<br/>O aplicativo tem a permissão Subscription.Read.All<br/><br/>Nota: Isso se aplica apenas a contas de trabalho/escola. | Assinaturas criadas por **qualquer aplicativo** para **qualquer usuário** no diretório.|

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->

```http
GET /subscriptions
```

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais

Este método não é compatível com os [Parâmetros de Consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome       | Tipo | Descrição|
|:-----------|:------|:----------|
| Autorização  | string  | {token} de portador. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação

Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se bem sucedido, este método retorna um código de resposta `200 OK` e uma lista de objetos de [assinatura](../resources/subscription.md) no corpo da resposta.

## <a name="example"></a>Exemplo

##### <a name="request"></a>Solicitação


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_subscriptions"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/subscriptions
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-subscriptions-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-subscriptions-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-subscriptions-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-subscriptions-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a>Resposta

Veja a seguir um exemplo da resposta. Observação: a resposta mostrada aqui pode ser truncada para brevidade. Todas as propriedades serão retornadas de uma chamada real.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.subscription",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#subscriptions",
  "value": [
    {
      "id": "0fc0d6db-0073-42e5-a186-853da75fb308",
      "resource": "Users",
      "applicationId": "24d3b144-21ae-4080-943f-7067b395b913",
      "changeType": "updated,deleted",
      "clientState": null,
      "notificationUrl": "https://webhookappexample.azurewebsites.net/api/notifications",
      "lifecycleNotificationUrl":"https://webhook.azurewebsites.net/api/send/lifecycleNotifications",
      "expirationDateTime": "2018-03-12T05:00:00Z",
      "creatorId": "8ee44408-0679-472c-bc2a-692812af3437",
      "latestSupportedTlsVersion": "v1_2",
      "encryptionCertificate": "",
      "encryptionCertificateId": "",
      "includeResourceData": false,
      "notificationContentType": "application/json"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List subscriptions",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->

> **Observação:** o valor da propriedade `clientState` não é retornado para fins de segurança.  

Quando uma solicitação retorna várias páginas de dados, a resposta inclui uma propriedade `@odata.nextLink` para ajudá-lo a gerenciar os resultados.  Para saber mais, consulte [Paginação de dados do Microsoft Graph em seu aplicativo](/graph/paging).
