---
title: Atualizar operationApprovalRequest
description: Atualize as propriedades de um objeto operationApprovalRequest.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 1ce96e13b791db9667cc1ea07fb3ee1d21182410
ms.sourcegitcommit: 4a960067cf2cd7d3c605550150eb3c9259adfe92
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/19/2021
ms.locfileid: "60485038"
---
# <a name="update-operationapprovalrequest"></a>Atualizar operationApprovalRequest

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Atualize as propriedades de um [objeto operationApprovalRequest.](../resources/intune-rbac-operationapprovalrequest.md)

## <a name="prerequisites"></a>Pré-requisitos
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|DeviceManagementRBAC.ReadWrite.All|
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|DeviceManagementRBAC.ReadWrite.All|

## <a name="http-request"></a>Solicitação HTTP
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/operationApprovalRequests/{operationApprovalRequestId}
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Cabeçalho|Valor|
|:---|:---|
|Autorização|&lt;Token&gt; de portador obrigatório.|
|Aceitar|application/json|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, fornece uma representação JSON para o [objeto operationApprovalRequest.](../resources/intune-rbac-operationapprovalrequest.md)

A tabela a seguir mostra as propriedades que são necessárias ao criar [operationApprovalRequest](../resources/intune-rbac-operationapprovalrequest.md).

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|A ID da Entidade|
|requestDateTime|DateTimeOffset|DateTime da solicitação. Essa propriedade é somente leitura.|
|expirationDateTime|DateTimeOffset|O DateTime em que as ações na solicitação não são mais permitidas. Essa propriedade é somente leitura.|
|lastModifiedDateTime|DateTimeOffset|DateTime modificado pela última vez. Essa propriedade é somente leitura.|
|requestor|[identitySet](../resources/intune-rbac-identityset.md)|A identidade do solicitante. Essa propriedade é somente leitura.|
|aprovador|[identitySet](../resources/intune-rbac-identityset.md)|A identidade do aprovador. Essa propriedade é somente leitura.|
|status|[operationApprovalRequestStatus](../resources/intune-rbac-operationapprovalrequeststatus.md)|O status atual da solicitação de aprovação. Essa propriedade é somente leitura. Os valores possíveis são: `unknown`, `needsApproval`, `approved`, `rejected`, `cancelled`, `completed`, `expired`.|
|requestJustification|Cadeia de caracteres|A justificativa da solicitação. Essa propriedade é somente leitura.|
|approvalJustification|Cadeia de caracteres|A justificativa para a aprovação da solicitação. Essa propriedade é somente leitura.|



## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um código de resposta e um `200 OK` objeto [operationApprovalRequest](../resources/intune-rbac-operationapprovalrequest.md) atualizado no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/operationApprovalRequests/{operationApprovalRequestId}
Content-type: application/json
Content-length: 1346

{
  "@odata.type": "#microsoft.graph.operationApprovalRequest",
  "requestDateTime": "2017-01-01T00:03:07.1589002-08:00",
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "requestor": {
    "@odata.type": "microsoft.graph.identitySet",
    "application": {
      "@odata.type": "microsoft.graph.identity",
      "id": "Id value",
      "displayName": "Display Name value"
    },
    "device": {
      "@odata.type": "microsoft.graph.identity",
      "id": "Id value",
      "displayName": "Display Name value"
    },
    "user": {
      "@odata.type": "microsoft.graph.identity",
      "id": "Id value",
      "displayName": "Display Name value"
    }
  },
  "approver": {
    "@odata.type": "microsoft.graph.identitySet",
    "application": {
      "@odata.type": "microsoft.graph.identity",
      "id": "Id value",
      "displayName": "Display Name value"
    },
    "device": {
      "@odata.type": "microsoft.graph.identity",
      "id": "Id value",
      "displayName": "Display Name value"
    },
    "user": {
      "@odata.type": "microsoft.graph.identity",
      "id": "Id value",
      "displayName": "Display Name value"
    }
  },
  "status": "needsApproval",
  "requestJustification": "Request Justification value",
  "approvalJustification": "Approval Justification value"
}
```

### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1459

{
  "@odata.type": "#microsoft.graph.operationApprovalRequest",
  "id": "4e9eed82-ed82-4e9e-82ed-9e4e82ed9e4e",
  "requestDateTime": "2017-01-01T00:03:07.1589002-08:00",
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "requestor": {
    "@odata.type": "microsoft.graph.identitySet",
    "application": {
      "@odata.type": "microsoft.graph.identity",
      "id": "Id value",
      "displayName": "Display Name value"
    },
    "device": {
      "@odata.type": "microsoft.graph.identity",
      "id": "Id value",
      "displayName": "Display Name value"
    },
    "user": {
      "@odata.type": "microsoft.graph.identity",
      "id": "Id value",
      "displayName": "Display Name value"
    }
  },
  "approver": {
    "@odata.type": "microsoft.graph.identitySet",
    "application": {
      "@odata.type": "microsoft.graph.identity",
      "id": "Id value",
      "displayName": "Display Name value"
    },
    "device": {
      "@odata.type": "microsoft.graph.identity",
      "id": "Id value",
      "displayName": "Display Name value"
    },
    "user": {
      "@odata.type": "microsoft.graph.identity",
      "id": "Id value",
      "displayName": "Display Name value"
    }
  },
  "status": "needsApproval",
  "requestJustification": "Request Justification value",
  "approvalJustification": "Approval Justification value"
}
```



