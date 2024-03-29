---
title: Criar accessAssignments
description: Crie um novo objeto delegatedAdminAccessAssignment.
author: adtangir
ms.localizationpriority: medium
ms.prod: customer-relationship-management
doc_type: apiPageType
ms.openlocfilehash: b794795a5c71a8a8e25eb6f2aa5ee51dead874a9
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/05/2022
ms.locfileid: "65210791"
---
# <a name="create-accessassignments"></a>Criar accessAssignments
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Crie um novo [objeto delegatedAdminAccessAssignment](../resources/delegatedadminaccessassignment.md) .

## <a name="permissions"></a>Permissions
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)| DelegatedAdminRelationship.ReadWrite.All |
|Delegado (conta pessoal da Microsoft)| Sem suporte. |
|Aplicativo| Sem suporte. |

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /tenantRelationships/delegatedAdminRelationships/{delegatedAdminRelationshipId}/accessAssignments
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|
|Content-Type|application/json. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, forneça uma representação JSON do objeto [delegatedAdminAccessAssignment](../resources/delegatedadminaccessassignment.md) .

Você pode especificar as propriedades a seguir ao criar **um delegatedAdminAccessAssignment**.

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|accessContainer|[delegatedAdminAccessContainer](../resources/delegatedadminaccesscontainer.md)|O contêiner de acesso por meio do qual os membros recebem acesso. Por exemplo, um grupo de segurança.|
|accessDetails|[delegatedAdminAccessDetails](../resources/delegatedadminaccessdetails.md)|Os identificadores das funções administrativas atribuídas pelo parceiro no locatário do cliente.|


## <a name="response"></a>Resposta

Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [delegatedAdminAccessAssignment](../resources/delegatedadminaccessassignment.md) no corpo da resposta. Um **cabeçalho** Location na resposta aponta para o objeto **delegatedAdminAccessAssignment** criado.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_delegatedadminaccessassignment_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/tenantRelationships/delegatedAdminRelationships/72a7ae7e-4887-4e34-9755-2e1e9b26b943-63f017cb-9e0d-4f14-94bd-4871902b3409/accessAssignments
Content-Type: application/json

{
  "accessContainer": {
    "accessContainerId": "869713c9-0b28-4d08-8949-ae07ae1bf528",
    "accessContainerType": "securityGroup"
  },
  "accessDetails": {
    "unifiedRoles": [
      {
        "roleDefinitionId": "29232cdf-9323-42fd-ade2-1d097af3e4de"
      },
      {
        "roleDefinitionId": "f2ef992c-3afb-46b9-b7cf-a126ee74c451"
      },
      {
        "roleDefinitionId": "729827e3-9c14-49f7-bb1b-9608f156bbb8"
      },
      {
        "roleDefinitionId": "3a2c62db-5318-420d-8d74-23affee5d9d5"
      }
    ]
  }
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-delegatedadminaccessassignment-from--csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-delegatedadminaccessassignment-from--javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-delegatedadminaccessassignment-from--objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-delegatedadminaccessassignment-from--java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/create-delegatedadminaccessassignment-from--go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a>Resposta
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.delegatedAdminAccessAssignment"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Location: https://graph.microsoft.com/beta/tenantRelationships/delegatedAdminRelationships/72a7ae7e-4887-4e34-9755-2e1e9b26b943-63f017cb-9e0d-4f14-94bd-4871902b3409/accessAssignments/a9d6cf90-083a-47dc-ace2-1da98be3f344

{

  "@odata.type": "#microsoft.graph.delegatedAdminAccessAssignment",
  "@odata.context": "https://graph.microsoft.com/beta/tenantRelationships/$metadata#accessAssignments",
  "@odata.etag": "W/\"JyIxODAwZTY4My0wMDAwLTAyMDAtMDAwMC02MTU0OWFmMDAwMDAiJw==\"",
  "id": "a9d6cf90-083a-47dc-ace2-1da98be3f344",
  "status": "pending",
  "createdDateTime": "2022-02-13T10:33:52.3182097Z",
  "lastModifiedDateTime": "2022-02-13T10:33:52.3182097Z",
  "accessContainer": {
    "accessContainerId": "869713c9-0b28-4d08-8949-ae07ae1bf528",
    "accessContainerType": "securityGroup"
  },
  "accessDetails": {
    "unifiedRoles": [
      {
        "roleDefinitionId": "29232cdf-9323-42fd-ade2-1d097af3e4de"
      },
      {
        "roleDefinitionId": "f2ef992c-3afb-46b9-b7cf-a126ee74c451"
      },
      {
        "roleDefinitionId": "729827e3-9c14-49f7-bb1b-9608f156bbb8"
      },
      {
        "roleDefinitionId": "3a2c62db-5318-420d-8d74-23affee5d9d5"
      }
    ]
  }
}
```

