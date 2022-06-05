---
title: Tipo complexo approvalSettings
description: As configurações de aprovação conforme definido em uma regra de política de gerenciamento de função.
ms.localizationpriority: medium
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 0fd8af9a314052dab87908fde5987850899e8f90
ms.sourcegitcommit: 95df356bd43b8e5f60fb4c2b62bfa0d5f36a61c2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2022
ms.locfileid: "65900216"
---
# <a name="approvalsettings-complex-type"></a>Tipo complexo approvalSettings

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

As configurações de aprovação conforme definido em uma regra de política de gerenciamento de função.

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|approvalMode|Cadeia de Caracteres|Um de `SingleStage`, `Serial`, `Parallel`, `NoApproval` (padrão). `NoApproval` é usado quando `isApprovalRequired` é `false`.|
|approvalStages|[coleção approvalStage](../resources/approvalstage.md)|Se a aprovação for necessária, um ou dois elementos dessa coleção definirão cada um dos estágios de aprovação. Uma matriz vazia se nenhuma aprovação for necessária.|
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
      "@odata.type": "microsoft.graph.approvalStage"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "approvalSettings complex type",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


