---
title: Tipo de recurso operationApprovalRequest
description: A entidade OperationApprovalRequest
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 45c2b30a39c9930ee8a8d7def27a06e7617fddbf
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/08/2021
ms.locfileid: "61346742"
---
# <a name="operationapprovalrequest-resource-type"></a>Tipo de recurso operationApprovalRequest

Namespace: microsoft.graph

> **Importante:** As GRAPH da Microsoft na versão /beta estão sujeitas a alterações; o uso de produção não é suportado.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

A entidade OperationApprovalRequest

## <a name="methods"></a>Methods
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar operationApprovalRequests](../api/intune-rbac-operationapprovalrequest-list.md)|[Coleção operationApprovalRequest](../resources/intune-rbac-operationapprovalrequest.md)|Listar propriedades e relações dos [objetos operationApprovalRequest.](../resources/intune-rbac-operationapprovalrequest.md)|
|[Obter operationApprovalRequest](../api/intune-rbac-operationapprovalrequest-get.md)|[operationApprovalRequest](../resources/intune-rbac-operationapprovalrequest.md)|Leia propriedades e relações do [objeto operationApprovalRequest.](../resources/intune-rbac-operationapprovalrequest.md)|
|[Criar operationApprovalRequest](../api/intune-rbac-operationapprovalrequest-create.md)|[operationApprovalRequest](../resources/intune-rbac-operationapprovalrequest.md)|Crie um novo [objeto operationApprovalRequest.](../resources/intune-rbac-operationapprovalrequest.md)|
|[Excluir operationApprovalRequest](../api/intune-rbac-operationapprovalrequest-delete.md)|Nenhum|Exclui uma [operaçãoApprovalRequest](../resources/intune-rbac-operationapprovalrequest.md).|
|[Atualizar operationApprovalRequest](../api/intune-rbac-operationapprovalrequest-update.md)|[operationApprovalRequest](../resources/intune-rbac-operationapprovalrequest.md)|Atualize as propriedades de um [objeto operationApprovalRequest.](../resources/intune-rbac-operationapprovalrequest.md)|
|[aprovar ação](../api/intune-rbac-operationapprovalrequest-approve.md)|String|Aprova a instância solicitada de uma operationApprovalRequest|
|[rejeitar ação](../api/intune-rbac-operationapprovalrequest-reject.md)|String|Rejeita a instância solicitada de uma operationApprovalRequest|
|[Ação cancelApproval](../api/intune-rbac-operationapprovalrequest-cancelapproval.md)|String|Cancela uma instância já aprovada de uma operaçãoApprovalRequest|
|[Ação getRequestStatus](../api/intune-rbac-operationapprovalrequest-getrequeststatus.md)|[operationApprovalRequestEntityStatus](../resources/intune-rbac-operationapprovalrequestentitystatus.md)|Ainda não documentado|
|[função getMyRequestById](../api/intune-rbac-operationapprovalrequest-getmyrequestbyid.md)|[operationApprovalRequest](../resources/intune-rbac-operationapprovalrequest.md)|Ainda não documentado|
|[função getMyRequests](../api/intune-rbac-operationapprovalrequest-getmyrequests.md)|[Coleção operationApprovalRequest](../resources/intune-rbac-operationapprovalrequest.md)|Ainda não documentado|
|[Ação cancelMyRequest](../api/intune-rbac-operationapprovalrequest-cancelmyrequest.md)|Nenhuma|Ainda não documentado|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|A ID da Entidade|
|requestDateTime|DateTimeOffset|DateTime da solicitação. Essa propriedade é somente leitura.|
|expirationDateTime|DateTimeOffset|O DateTime em que as ações na solicitação não são mais permitidas. Essa propriedade é somente leitura.|
|lastModifiedDateTime|DateTimeOffset|DateTime modificado pela última vez. Essa propriedade é somente leitura.|
|requestor|[identitySet](../resources/intune-rbac-identityset.md)|A identidade do solicitante. Essa propriedade é somente leitura.|
|aprovador|[identitySet](../resources/intune-rbac-identityset.md)|A identidade do aprovador. Essa propriedade é somente leitura.|
|status|[operationApprovalRequestStatus](../resources/intune-rbac-operationapprovalrequeststatus.md)|O status atual da solicitação de aprovação. Essa propriedade é somente leitura. Os valores possíveis são: `unknown`, `needsApproval`, `approved`, `rejected`, `cancelled`, `completed`, `expired`.|
|requestJustification|String|A justificativa da solicitação. Essa propriedade é somente leitura.|
|approvalJustification|String|A justificativa para a aprovação da solicitação. Essa propriedade é somente leitura.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.operationApprovalRequest"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.operationApprovalRequest",
  "id": "String (identifier)",
  "requestDateTime": "String (timestamp)",
  "expirationDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "requestor": {
    "@odata.type": "microsoft.graph.identitySet",
    "application": {
      "@odata.type": "microsoft.graph.identity",
      "id": "String",
      "displayName": "String"
    },
    "device": {
      "@odata.type": "microsoft.graph.identity",
      "id": "String",
      "displayName": "String"
    },
    "user": {
      "@odata.type": "microsoft.graph.identity",
      "id": "String",
      "displayName": "String"
    }
  },
  "approver": {
    "@odata.type": "microsoft.graph.identitySet",
    "application": {
      "@odata.type": "microsoft.graph.identity",
      "id": "String",
      "displayName": "String"
    },
    "device": {
      "@odata.type": "microsoft.graph.identity",
      "id": "String",
      "displayName": "String"
    },
    "user": {
      "@odata.type": "microsoft.graph.identity",
      "id": "String",
      "displayName": "String"
    }
  },
  "status": "String",
  "requestJustification": "String",
  "approvalJustification": "String"
}
```




