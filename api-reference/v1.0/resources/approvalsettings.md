---
title: Tipo de recurso approvalSettings
description: As configurações de aprovação conforme definido em uma regra de política de gerenciamento de função.
author: rkarim-ms
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 2dc0240fd272e4d79209ee37bf79f293052eb400
ms.sourcegitcommit: dae41f5828677b993ba89f38c1d1c42d91c0ba02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/29/2022
ms.locfileid: "65133890"
---
# <a name="approvalsettings-resource-type"></a>Tipo de recurso approvalSettings

Namespace: microsoft.graph

As configurações de aprovação conforme definido em uma regra de política de gerenciamento de função.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|approvalMode|Cadeia de caracteres|Um de `SingleStage`, `Serial`, `Parallel`, `NoApproval` (padrão). `NoApproval` é usado quando `isApprovalRequired` é `false`.|
|approvalStages|[Coleção unifiedApprovalStage](../resources/unifiedapprovalstage.md)|Se a aprovação for necessária, um ou dois elementos dessa coleção definirão cada um dos estágios de aprovação. Uma matriz vazia se nenhuma aprovação for necessária.|
|isApprovalRequired|Booliano|Indica se a aprovação é necessária para solicitações nesta política.|
|isApprovalRequiredForExtension|Booliano|Indica se a aprovação é necessária para que um usuário estenda sua atribuição.|
|isRequestorJustificationRequired|Booliano|Indica se o solicitante é necessário para fornecer uma justificativa em sua solicitação.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.approvalSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.approvalSettings",
  "isApprovalRequired": "Boolean",
  "isApprovalRequiredForExtension": "Boolean",
  "isRequestorJustificationRequired": "Boolean",
  "approvalMode": "String",
  "approvalStages": [
    {
      "@odata.type": "microsoft.graph.unifiedApprovalStage"
    }
  ]
}
```

