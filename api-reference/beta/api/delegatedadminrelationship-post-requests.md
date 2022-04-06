---
title: Criar solicitações
description: Crie um novo objeto delegatedAdminRelationshipRequest.
author: adtangir
ms.localizationpriority: medium
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 96760913dc8dc5e4745cd1231f1b69a18a313b6f
ms.sourcegitcommit: cc9e5b3630cb84c48bbbb2d84a963b9562d1fb78
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/31/2022
ms.locfileid: "64589561"
---
# <a name="create-requests"></a>Criar solicitações
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Crie um novo [objeto delegatedAdminRelationshipRequest](../resources/delegatedadminrelationshiprequest.md) .

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
POST /tenantRelationships/delegatedAdminRelationships/{delegatedAdminRelationshipId}/requests
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|
|Content-Type|application/json. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, fornece uma representação JSON do [objeto delegatedAdminRelationshipRequest](../resources/delegatedadminrelationshiprequest.md) .

Você pode especificar as seguintes propriedades ao criar **um delegatedAdminRelationshipRequest**.

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|ação|delegatedAdminRelationshipRequestAction|A ação a ser executada na relação de administrador delegada. Obrigatório. Os valores possíveis são: `lockForApproval`, `terminate`.|

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um `201 Created` código de resposta e um [objeto delegatedAdminRelationshipRequest](../resources/delegatedadminrelationshiprequest.md) no corpo da resposta. A resposta contém um header **Location** que contém uma URL para a solicitação de relação de administrador delegada criada.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação
<!-- {
  "blockType": "request",
  "name": "create_delegatedadminrelationshiprequest_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/tenantRelationships/delegatedAdminRelationships/5d027261-d21f-4aa9-b7db-7fa1f56fb163-8777b240-c6f0-4469-9e98-a3205431b836/requests
Content-Type: application/json

{
  "action": "lockForApproval"
}
```


### <a name="response"></a>Resposta
>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.delegatedAdminRelationshipRequest"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Location: https://graph.microsoft.com/beta/tenantRelationships/delegatedAdminRelationships/c45e5ffb-3de2-4938-a214-b7eed802db66-4be56058-bb48-4a8e-8282-6cf0e98e6c9d/requests/5a6666c9-7282-0a41-67aa-25a5a3fbf339

{
  "@odata.type": "#microsoft.graph.delegatedAdminRelationshipRequest",
  "@odata.context": "https://graph.microsoft.com/beta/tenantRelationships/$metadata#requests",
  "id": "5a6666c9-7282-0a41-67aa-25a5a3fbf339",
  "action": "lockForApproval",
  "status": "created",
  "createdDateTime": "2022-02-10T10:55:47.1180588Z",
  "lastModifiedDateTime": "2022-02-10T10:55:47.1180588Z"
}
```

