---
title: 'oauth2permissiongrant: Delta'
description: Obter oauth2permissiongrants recentemente criados, atualizados ou excluídos sem executar uma leitura completa de toda a coleção de recursos.
localization_priority: Normal
author: psignoret
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: b41a12130cd447104f25251c75cedc77957b208f
ms.sourcegitcommit: 20b951f8bd245bb3a2bc7d3f5533e8619e9db084
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/27/2020
ms.locfileid: "45427428"
---
# <a name="oauth2permissiongrant-delta"></a>oauth2permissiongrant: Delta

Namespace: microsoft.graph

Obter objetos [oauth2permissiongrant](../resources/oauth2permissiongrant.md) recém-criados, atualizados ou excluídos sem executar uma leitura completa de toda a coleção de recursos. Para obter detalhes, consulte [usando a consulta Delta](/graph/delta-query-overview).

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).


|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All    |
|Delegado (conta pessoal da Microsoft) | Sem suporte.    |
|oauth2permissiongrant | Directory.Read.All, Directory.ReadWrite.All |

## <a name="http-request"></a>Solicitação HTTP


<!-- { "blockType": "ignored" } -->
```http
GET /oauth2permissiongrants/delta
```

## <a name="query-parameters"></a>Parâmetros de consulta

As alterações de controle provocam uma rodada de uma ou mais chamadas de função **Delta** . Se você usar qualquer parâmetro de consulta (diferente de `$deltatoken` e `$skiptoken`), especifique-o na primeira solicitação **delta**. O Microsoft Graph codifica automaticamente todos os parâmetros especificados na parte do token da URL `nextLink` ou `deltaLink` fornecida na resposta. Você só precisa especificar parâmetros de consulta uma vez. Em solicitações subsequentes, copie e aplique `nextLink` a `deltaLink` URL ou à resposta anterior. A URL inclui os parâmetros codificados.

| Parâmetro de consulta      | Tipo   |Descrição|
|:---------------|:--------|:----------|
| $deltatoken | cadeia de caracteres | Um [token de estado](/graph/delta-query-overview) retornado na `deltaLink` URL da chamada de função **Delta** anterior para a mesma coleção de recursos, indicando a conclusão dessa rodada de controle de alterações. Salve e aplique a `deltaLink` URL inteira, incluindo esse token, na primeira solicitação da próxima rodada de controle de alterações para essa coleção.|
| $skiptoken | string | Um [token de estado](/graph/delta-query-overview) retornado na `nextLink` URL da chamada de função **Delta** anterior, indicando que há mais alterações a serem controladas na mesma coleção de recursos. |

### <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais

Este método dá suporte a Parâmetros de consulta do OData para ajudar a personalizar a resposta.

- Você pode usar um `$select` parâmetro de consulta para especificar apenas as propriedades que você precisa para o melhor desempenho. A propriedade **id** sempre será retornada.
- O `$filter` parâmetro de consulta só pode ser usado para controlar alterações em recursos específicos usando a ID do recurso. Por exemplo, `$filter=id+eq+{value}` ou `$filter=id+eq+{value1}+or+id+eq+{value2}` .


## <a name="request-headers"></a>Cabeçalhos de solicitação
| Nome       | Descrição|
|:---------------|:----------|
| Autorização  | {token} de portador. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto da coleção [oauth2permissiongrant](../resources/oauth2permissiongrant.md) no corpo da resposta. A resposta também inclui uma URL `nextLink` ou uma URL `deltaLink`.

- Se uma `nextLink` URL for retornada, as páginas adicionais de dados poderão ser recuperadas na sessão. O **oauth2permissiongrant** continua fazendo solicitações usando a `nextLink` URL até que uma `deltaLink` URL seja incluída na resposta.
- Se uma `deltaLink` URL for retornada, não serão retornados mais dados sobre o recurso. Persista e use a `deltaLink` URL para saber mais sobre as alterações no recurso no futuro.

Para obter detalhes, consulte [usando a consulta Delta](/graph/delta-query-overview). Por exemplo, consulte [obter alterações incrementais para usuários](/graph/delta-query-users).

## <a name="example"></a>Exemplo
### <a name="request"></a>Solicitação

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "oauth2permissiongrant_delta"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/oauth2permissiongrants/delta
```

### <a name="response"></a>Resposta
>**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.
<!-- { 
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.oAuth2PermissionGrant",
  "isCollection": true 
} --> 
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#oauth2permissiongrants",
  "@odata.nextLink":"https://graph.microsoft.com/v1.0/oauth2permissiongrants/delta?$skiptoken=pqwSUjGYvb3jQpbwVAwEL7yuI3dU1LecfkkfLPtnIjsXoYQp_dpA3cNJWc",
  "value": [
    {
      "clientId": "22a3c970-8ad4-4120-8127-300837f87f2c",
      "consentType": "Principal",
      "principalId": "c2e8df37-c6a7-4d88-89b1-feb4f1fda7c5",
      "resourceId": "98dc9d95-49b6-405a-b3c0-834e969a708b",
      "scope": "User.Read Directory.AccessAsUser.All",
      "id": "cMmjItSKIEGBJzAIN_h_LJWd3Ji2SVpAs8CDTpaacIs33-jCp8aITYmx_rTx_afF"
    }
  ]
}
```

<!-- uuid: ba679d55-d10e-4518-b733-6f3e9576afb1
2020-04-09 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "oauth2permissiongrant: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
