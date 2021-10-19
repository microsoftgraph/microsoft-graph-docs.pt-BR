---
title: Tipo de recurso operationApprovalRequestEntityStatus
description: O objeto OperationApprovalRequestEntityStatus
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: cef153334cdd30044a75ed1cc0e322f6e94ecb64
ms.sourcegitcommit: 4a960067cf2cd7d3c605550150eb3c9259adfe92
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/19/2021
ms.locfileid: "60487881"
---
# <a name="operationapprovalrequestentitystatus-resource-type"></a>Tipo de recurso operationApprovalRequestEntityStatus

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

O objeto OperationApprovalRequestEntityStatus

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|requestId|Cadeia de caracteres|A ID do OperationApprovalRequest para esta entidade. Essa propriedade é somente leitura.|
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



