---
title: Inscrições de lista
description: " Consulte os cenários abaixo para obter detalhes."
localization_priority: Normal
ms.openlocfilehash: 1b751b8632d82626e2ba87bf00a054b2be4f25f9
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27876983"
---
# <a name="list-subscriptions"></a>Inscrições de lista

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Recupere uma lista das inscrições de webhook. O conteúdo da resposta depende do contexto no qual o aplicativo está chamando; Consulte os cenários abaixo para obter detalhes.

## <a name="permissions"></a>Permissions

Essa API suporta os seguintes escopos de permissão; Para saber mais, incluindo como escolher permissões, consulte [permissões](/graph/permissions-reference).

| Tipo de permissão  | Permissões (da com menos para a com mais privilégios)  |
|:---------------- |:-------------------------------------------- |
| [Delegada](/graph/auth-v2-user) (conta do trabalho ou da escola) | Permissão necessária para [criar a inscrição](subscription-post-subscriptions.md) ou Subscription.Read.All (veja abaixo). |
| [Delegada](/graph/auth-v2-user) (conta pessoal da Microsoft) | Permissão necessária para [criar a inscrição](subscription-post-subscriptions.md) ou Subscription.Read.All (veja abaixo). |
| [Application](/graph/auth-v2-service) | Permissão necessária para [criar a assinatura](subscription-post-subscriptions.md). |

Resultados de resposta são baseados no contexto do aplicativo chamado. Apresentamos a seguir um resumo dos cenários comuns:

### <a name="basic-scenarios"></a>Cenários básicos

Mais comumente, um aplicativo deseja recuperar as assinaturas que originalmente criado para o usuário conectado no momento, ou para todos os usuários no diretório (contas de trabalho/escola). Esses cenários não exigem qualquer permissões especiais além do aplicativo originalmente usado para criar suas assinaturas.

| Contexto do aplicativo chamado | Resposta conterá |
|:-----|:---------------- |
| App está chamando em nome do usuário conectado (delegada permissão). <br/>- e -<br/>App tem a permissão original necessária para [criar a assinatura](subscription-post-subscriptions.md).<br/><br/>Observação: Isso se aplica ao pessoais contas da Microsoft e contas de trabalho/escola. | Inscrições criadas por **Este aplicativo** para o usuário entrou no apenas. |
| App está chamando em nome do próprio (permissão de aplicativo).<br/>- e -<br/>App tem a permissão original necessária para [criar a assinatura](subscription-post-subscriptions.md).<br/><br/>Observação: Isso se aplica a apenas contas de trabalho/escola.| Inscrições criadas por **Este aplicativo** para si mesmo ou para qualquer usuário no diretório.|

### <a name="advanced-scenarios"></a>Cenários avançados

Em alguns casos, um aplicativo quer recuperar inscrições criadas por outros aplicativos. Por exemplo, um usuário quiser ver todas as inscrições criadas por qualquer aplicativo em nome deles. Ou então, um administrador talvez queira ver todas as inscrições de todos os aplicativos no seu diretório.
Para nesses cenários, uma permissão delegada Subscription.Read.All é necessária.

| Contexto do aplicativo chamado | Resposta conterá |
|:-----|:---------------- |
| App está chamando em nome do usuário conectado (delegada permissão). *O usuário é um não seja o administrador*. <br/>- e -<br/>App tem a permissão Subscription.Read.All<br/><br/>Observação: Isso se aplica ao pessoais contas da Microsoft e contas de trabalho/escola. | Inscrições criadas por **qualquer aplicativo** para o usuário entrou no apenas. |
| App está chamando em nome do usuário conectado (delegada permissão). *O usuário é um administrador*.<br/>- e -<br/>App tem a permissão Subscription.Read.All<br/><br/>Observação: Isso se aplica a apenas contas de trabalho/escola. | Inscrições criadas por **qualquer aplicativo** para **qualquer usuário** no diretório.|

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->

```http
GET /subscriptions
```

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais

Este método não oferece suporte para os [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome       | Tipo | Descrição|
|:-----------|:------|:----------|
| Autorização  | string  | {token} de portador. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação

Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um `200 OK` código de resposta e uma lista de objetos de [inscrição](../resources/subscription.md) no corpo da resposta.

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

Veja a seguir um exemplo da resposta. Observação: A resposta mostrada aqui pode estar truncada para fins de concisão. Todas as propriedades serão retornadas de uma chamada real.

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
<!-- {
  "type": "#page.annotation",
  "description": "List subscriptions",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

Quando uma solicitação retorna várias páginas de dados, a resposta inclui um `@odata.nextLink` propriedade para ajudá-lo a gerenciar os resultados.  Para saber mais, consulte [os dados de paginação Microsoft Graph em seu aplicativo](/graph/paging).
