---
title: Listar solicitações
description: Obtenha uma lista dos objetos delegatedAdminRelationshipRequest e suas propriedades.
author: adtangir
ms.localizationpriority: medium
ms.prod: customer-relationship-management
doc_type: apiPageType
ms.openlocfilehash: db0ebb59bea4fa6b278e15580fda9108768b115a
ms.sourcegitcommit: 5a43129dbf705f2d1a6afcff36af9f41ecee026d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/07/2022
ms.locfileid: "64704279"
---
# <a name="list-requests"></a>Listar solicitações
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Obtenha uma lista dos [objetos delegatedAdminRelationshipRequest](../resources/delegatedadminrelationshiprequest.md) e suas propriedades.

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)| DelegatedAdminRelationship.Read.All, DelegatedAdminRelationship.ReadWrite.All |
|Delegado (conta pessoal da Microsoft)| Sem suporte. |
|Aplicativo| Sem suporte. |

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /tenantRelationships/delegatedAdminRelationships/{delegatedAdminRelationshipId}/requests
```

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais
Esse método dá suporte aos `$expand`[parâmetros](/graph/query-parameters) `$filter`de consulta , `$select`, `$top`, e `$count``$skipToken` OData para ajudar a personalizar a resposta.  

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se bem-sucedido, este método retorna `200 OK` um código de resposta e uma coleção de objetos [delegatedAdminRelationshipRequest](../resources/delegatedadminrelationshiprequest.md) no corpo da resposta.

Cada **objeto delegatedAdminRelationshipRequest** contém uma **propriedade @odata.etag** de acordo com RFC2616.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação
<!-- {
  "blockType": "request",
  "name": "list_delegatedadminrelationshiprequest"
}
-->
``` http
GET https://graph.microsoft.com/beta/tenantRelationships/delegatedAdminRelationships/5d027261-d21f-4aa9-b7db-7fa1f56fb163-8777b240-c6f0-4469-9e98-a3205431b836/requests
```


### <a name="response"></a>Resposta
>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.delegatedAdminRelationshipRequest)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/tenantRelationships/$metadata#requests",
  "value": [
    {
      "@odata.type": "#microsoft.graph.delegatedAdminRelationshipRequest",
      "@odata.etag": "W/\"JyIxODAwZTY4My0wMDAwLTAyMDAtMDAwMC02MTU0OWFmMDAwMDAiJw==\"",
      "id": "ae5a6b9e-6355-43dd-b708-48486b69c3ff",
      "action": "lockForApproval",
      "status": "complete",
      "createdDateTime": "2022-02-01T06:14:55.5398865Z",
      "lastModifiedDateTime": "2022-02-01T06:14:55.5398865Z"
    },
    {
      "@odata.type": "#microsoft.graph.delegatedAdminRelationshipRequest",
      "@odata.etag": "W/\"JyIxODAwZTY4My0wMDAwLTAyMDAtMDAwMC02MTU0OWFmMDAwMDAiJw==\"",
      "id": "8a1b6676-5c12-47ba-8d3a-1d38387b0909",
      "action": "terminate",
      "status": "running",
      "createdDateTime": "2022-03-02T06:11:55.5398865Z",
      "lastModifiedDateTime": "2022-03-02T06:11:55.5398865Z"
    }
  ]
}
```

