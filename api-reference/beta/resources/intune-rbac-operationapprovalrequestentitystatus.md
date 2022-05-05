---
title: Tipo de recurso operationApprovalRequestEntityStatus
description: O objeto OperationApprovalRequestEntityStatus
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: ffc877ddf0a724b1471c55e2b9edb0455e4da0fb
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/05/2022
ms.locfileid: "65209125"
---
# <a name="operationapprovalrequestentitystatus-resource-type"></a>Tipo de recurso operationApprovalRequestEntityStatus

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso em produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

O objeto OperationApprovalRequestEntityStatus

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|Requestid|Cadeia de Caracteres|A ID do OperationApprovalRequest para esta Entidade. Essa propriedade é somente leitura.|
|requestExpirationDateTime|DateTimeOffset|O DateTime no qual as ações na solicitação não são mais permitidas. Essa propriedade é somente leitura.|
|Requeststatus|[operationApprovalRequestStatus](../resources/intune-rbac-operationapprovalrequeststatus.md)|O status atual da solicitação de aprovação. Essa propriedade é somente leitura. Os valores possíveis são: `unknown`, `needsApproval`, `approved`, `rejected`, `cancelled`, `completed`, `expired`, `unknownFutureValue`.|
|entityLocked|Booliano|O status da Entidade em relação às alterações, se outras solicitações são permitidas ou se a Entidade está bloqueada. Essa propriedade é somente leitura.|

## <a name="relationships"></a>Relações
Nenhuma

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.operationApprovalRequestEntityStatus"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.operationApprovalRequestEntityStatus",
  "requestId": "String",
  "requestExpirationDateTime": "String (timestamp)",
  "requestStatus": "String",
  "entityLocked": true
}
```




