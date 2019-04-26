---
title: Listar de assinaturas
description: " Veja os cenários abaixo para obter detalhes."
localization_priority: Normal
author: piotrci
ms.openlocfilehash: 3ffcf78c7df28faba22b92a7389f473f0ea91613
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33335808"
---
# <a name="list-subscriptions"></a>Listar de assinaturas

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Recupere uma lista de assinaturas de webhook. O conteúdo da resposta depende do contexto no qual o aplicativo está chamando; Veja os cenários abaixo para obter detalhes.

## <a name="permissions"></a>Permissões

Essa API suporta os seguintes escopos de permissão; para saber mais, incluindo como escolher permissões, consulte [permissões](/graph/permissions-reference).

| Tipo de permissão  | Permissões (da com menos para a com mais privilégios)  |
|:---------------- |:-------------------------------------------- |
| [Delegado](/graph/auth-v2-user) (conta corporativa ou de estudante) | Permissão necessária para [criar assinatura](subscription-post-subscriptions.md) ou assinatura. Read. All (veja abaixo). |
| [Delegado](/graph/auth-v2-user) (conta pessoal da Microsoft) | Permissão necessária para [criar assinatura](subscription-post-subscriptions.md) ou assinatura. Read. All (veja abaixo). |
| [Application](/graph/auth-v2-service) | Permissão necessária para [criar a assinatura](subscription-post-subscriptions.md). |

Os resultados da resposta são baseados no contexto do aplicativo de chamada. Veja a seguir um resumo dos cenários comuns:

### <a name="basic-scenarios"></a>Cenários básicos

Normalmente, um aplicativo deseja recuperar as assinaturas criadas originalmente para o usuário conectado no momento ou para todos os usuários no diretório (contas corporativas/de estudante). Esses cenários não exigem nenhuma permissão especial além daquelas que o aplicativo usava originalmente para criar suas assinaturas.

| Contexto do aplicativo de chamada | Resposta contém |
|:-----|:---------------- |
| O aplicativo está chamando em nome do usuário conectado (permissão delegada). <br/>e<br/>O aplicativo tem a permissão original necessária para [criar a assinatura](subscription-post-subscriptions.md).<br/><br/>Observação: isso se aplica às contas da Microsoft pessoais e às contas corporativas/de estudante. | Assinaturas criadas por **este aplicativo** somente para o usuário conectado. |
| O aplicativo está chamando em nome de si mesmo (permissão de aplicativo).<br/>e<br/>O aplicativo tem a permissão original necessária para [criar a assinatura](subscription-post-subscriptions.md).<br/><br/>Observação: isso se aplica apenas às contas corporativas/de estudante.| Assinaturas criadas por **este aplicativo** para si mesmo ou para qualquer usuário no diretório.|

### <a name="advanced-scenarios"></a>Cenários avançados

Em alguns casos, um aplicativo deseja recuperar assinaturas criadas por outros aplicativos. Por exemplo, um usuário deseja ver todas as assinaturas criadas por qualquer aplicativo em seu nome. Ou, um administrador pode querer ver todas as assinaturas de todos os aplicativos em seu diretório.
Para esses cenários, uma assinatura de permissão delegada. Read. All é necessário.

| Contexto do aplicativo de chamada | Resposta contém |
|:-----|:---------------- |
| O aplicativo está chamando em nome do usuário conectado (permissão delegada). *O usuário não é um administrador*. <br/>e<br/>O aplicativo tem a permissão Subscription. Read. All<br/><br/>Observação: isso se aplica às contas da Microsoft pessoais e às contas corporativas/de estudante. | Assinaturas criadas por **qualquer aplicativo** somente para o usuário conectado. |
| O aplicativo está chamando em nome do usuário conectado (permissão delegada). *O usuário é um administrador*.<br/>e<br/>O aplicativo tem a permissão Subscription. Read. All<br/><br/>Observação: isso se aplica apenas às contas corporativas/de estudante. | Assinaturas criadas por **qualquer aplicativo** para **qualquer usuário** no diretório.|

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->

```http
GET /subscriptions
```

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais

Este método não oferece suporte aos [parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome       | Tipo | Descrição|
|:-----------|:------|:----------|
| Autorização  | string  | {token} de portador. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação

Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará `200 OK` um código de resposta e uma lista de objetos [Subscription](../resources/subscription.md) no corpo da resposta.

## <a name="example"></a>Exemplo

##### <a name="request"></a>Solicitação

<!-- {
  "blockType": "request",
  "name": "get_subscriptions"
}-->

```http
GET https://graph.microsoft.com/beta/subscriptions
```

##### <a name="response"></a>Resposta

Veja a seguir um exemplo da resposta. Observação: a resposta mostrada aqui pode ser truncada por brevidade. Todas as propriedades serão retornadas de uma chamada real.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.subscription",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 586

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
      "expirationDateTime": "2018-03-12T05:00:00Z",
      "creatorId": "8ee44408-0679-472c-bc2a-692812af3437"
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
  "suppressions": []
}
-->

Quando uma solicitação retorna várias páginas de dados, a resposta inclui uma `@odata.nextLink` propriedade para ajudá-lo a gerenciar os resultados.  Para saber mais, confira paGinação [de dados do Microsoft Graph em seu aplicativo](/graph/paging).
