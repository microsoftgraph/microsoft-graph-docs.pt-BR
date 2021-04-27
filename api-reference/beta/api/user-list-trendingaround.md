---
title: Listar tendênciasAround
description: Insight calculado que retorna a lista de itens que estão na tendência em torno de um usuário.
author: jpettere
localization_priority: Normal
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: b1594d031f9ff007a87243ccf0cf481022b48d89
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52052583"
---
# <a name="list-trendingaround"></a>Listar tendênciasAround

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Insight calculado que retorna a lista de itens que estão na tendência em torno de um usuário.

**Observação:** Essa API será preterida e substituída pela [API de Tendência.](../resources/insights-trending.md)

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | Sites.Read.All    |
|Delegado (conta pessoal da Microsoft) | Sem suporte.    |
|Application | Sites.Read.All |

## <a name="http-request"></a>Solicitação HTTP
```http
GET /me/trendingAround
GET /users/{id | userPrincipalName}/trendingAround
GET /drive/root/createdByUser/trendingAround
GET /drive/root/lastModifiedByUser/trendingAround
```
## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais
Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.

## <a name="request-headers"></a>Cabeçalhos de solicitação
| Cabeçalho         | Valor                      |
|:---------------|:---------------------------|
| Autorização  | {token} de portador. Obrigatório.  |
| Content-Type   | application/json           |

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta 200 OK e uma coleção de [objetos driveItem](../resources/driveitem.md) no corpo da resposta.

## <a name="example"></a>Exemplo
##### <a name="request"></a>Solicitação
```http
GET https://graph.microsoft.com/beta/me/trendingAround
```
##### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 226

{
  "id": "id-value",
  "name": "name-value",
  "DateTimeCreated": "DateTimeCreated-value",
  "DateTimeLastModified": "DateTimeLastModified-value",
  "webUrl": "webUrl-value",
}
```