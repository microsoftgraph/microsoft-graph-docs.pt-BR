---
title: Tipo de recurso operationApprovalRequestEntityStatus
description: O objeto OperationApprovalRequestEntityStatus
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 7449a0fd644e23bd7cba49398ecb3c84ac6e739d
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/08/2021
ms.locfileid: "61343585"
---
# <a name="operationapprovalrequestentitystatus-resource-type"></a>Tipo de recurso operationApprovalRequestEntityStatus

Namespace: microsoft.graph

> **Importante:** As GRAPH da Microsoft na versão /beta estão sujeitas a alterações; o uso de produção não é suportado.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

O objeto OperationApprovalRequestEntityStatus

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|requestId|String|A ID do OperationApprovalRequest para esta entidade. Essa propriedade é somente leitura.|
|requestExpirationDateTime|DateTimeOffset|O DateTime em que as ações na solicitação não são mais permitidas. Essa propriedade é somente leitura.|
|requestStatus|[operationApprovalRequestStatus](../resources/intune-rbac-operationapprovalrequeststatus.md)|O status atual da solicitação de aprovação. Essa propriedade é somente leitura. Os valores possíveis são: `unknown`, `needsApproval`, `approved`, `rejected`, `cancelled`, `completed`, `expired`.|
|entityLocked|Booliano|O status da Entidade em relação às alterações, se outras solicitações são permitidas ou a Entidade está bloqueada. Essa propriedade é somente leitura.|

## <a name="relationships"></a>Relações
Nenhum

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




