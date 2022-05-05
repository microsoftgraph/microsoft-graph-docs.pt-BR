---
title: Tipo de recurso operationApprovalRequest
description: A entidade OperationApprovalRequest
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: da330c06f770e099f190dc2faa127dacc166e19a
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/05/2022
ms.locfileid: "65210420"
---
# <a name="operationapprovalrequest-resource-type"></a>Tipo de recurso operationApprovalRequest

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso em produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

A entidade OperationApprovalRequest

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar operationApprovalRequests](../api/intune-rbac-operationapprovalrequest-list.md)|[coleção operationApprovalRequest](../resources/intune-rbac-operationapprovalrequest.md)|Listar propriedades e relações dos [objetos operationApprovalRequest](../resources/intune-rbac-operationapprovalrequest.md) .|
|[Obter operationApprovalRequest](../api/intune-rbac-operationapprovalrequest-get.md)|[operationApprovalRequest](../resources/intune-rbac-operationapprovalrequest.md)|Ler propriedades e relações do objeto [operationApprovalRequest](../resources/intune-rbac-operationapprovalrequest.md) .|
|[Criar operationApprovalRequest](../api/intune-rbac-operationapprovalrequest-create.md)|[operationApprovalRequest](../resources/intune-rbac-operationapprovalrequest.md)|Crie um novo [objeto operationApprovalRequest](../resources/intune-rbac-operationapprovalrequest.md) .|
|[Excluir operationApprovalRequest](../api/intune-rbac-operationapprovalrequest-delete.md)|Nenhuma|Exclui uma [operationApprovalRequest](../resources/intune-rbac-operationapprovalrequest.md).|
|[Atualizar operationApprovalRequest](../api/intune-rbac-operationapprovalrequest-update.md)|[operationApprovalRequest](../resources/intune-rbac-operationapprovalrequest.md)|Atualize as propriedades de [um objeto operationApprovalRequest](../resources/intune-rbac-operationapprovalrequest.md) .|
|[aprovar ação](../api/intune-rbac-operationapprovalrequest-approve.md)|Cadeia de Caracteres|Aprova a instância solicitada de uma operationApprovalRequest|
|[ação de rejeição](../api/intune-rbac-operationapprovalrequest-reject.md)|Cadeia de Caracteres|Rejeita a instância solicitada de uma operationApprovalRequest|
|[Ação cancelApproval](../api/intune-rbac-operationapprovalrequest-cancelapproval.md)|Cadeia de Caracteres|Cancela uma instância já aprovada de uma operationApprovalRequest|
|[Ação getRequestStatus](../api/intune-rbac-operationapprovalrequest-getrequeststatus.md)|[operationApprovalRequestEntityStatus](../resources/intune-rbac-operationapprovalrequestentitystatus.md)|Ainda não documentado|
|[Função getMyRequestById](../api/intune-rbac-operationapprovalrequest-getmyrequestbyid.md)|[operationApprovalRequest](../resources/intune-rbac-operationapprovalrequest.md)|Ainda não documentado|
|[Função getMyRequests](../api/intune-rbac-operationapprovalrequest-getmyrequests.md)|[coleção operationApprovalRequest](../resources/intune-rbac-operationapprovalrequest.md)|Ainda não documentado|
|[Ação cancelMyRequest](../api/intune-rbac-operationapprovalrequest-cancelmyrequest.md)|Nenhuma|Ainda não documentado|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|A ID da Entidade|
|requestDateTime|DateTimeOffset|O DateTime da solicitação. Essa propriedade é somente leitura.|
|expirationDateTime|DateTimeOffset|O DateTime no qual as ações na solicitação não são mais permitidas. Essa propriedade é somente leitura.|
|lastModifiedDateTime|DateTimeOffset|DateTime da última modificação. Essa propriedade é somente leitura.|
|Solicitante|[identitySet](../resources/intune-rbac-identityset.md)|A identidade do solicitante. Essa propriedade é somente leitura.|
|Aprovador|[identitySet](../resources/intune-rbac-identityset.md)|A identidade do aprovador. Essa propriedade é somente leitura.|
|status|[operationApprovalRequestStatus](../resources/intune-rbac-operationapprovalrequeststatus.md)|O status atual da solicitação de aprovação. Essa propriedade é somente leitura. Os valores possíveis são: `unknown`, `needsApproval`, `approved`, `rejected`, `cancelled`, `completed`, `expired`, `unknownFutureValue`.|
|requestJustification|Cadeia de Caracteres|A justificativa da solicitação. Essa propriedade é somente leitura.|
|approvalJustification|Cadeia de Caracteres|A justificativa para a aprovação da solicitação. Essa propriedade é somente leitura.|
|operationApprovalPolicies|Cadeia de Caracteres|As políticas de aprovação operacional usadas na solicitação. Essa propriedade é somente leitura.|

## <a name="relationships"></a>Relações
Nenhuma

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
  "approvalJustification": "String",
  "operationApprovalPolicies": "String"
}
```




