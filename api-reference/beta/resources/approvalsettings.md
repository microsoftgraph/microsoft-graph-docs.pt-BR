---
title: tipo complexo approvalSettings
description: Usado para a propriedade requestApprovalSettings de uma política de atribuição de pacote do Access. Fornece configurações adicionais para selecionar quem deve aprovar cada solicitação.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 23227bd4f363748bade73999a4004747d691a364
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42508230"
---
# <a name="approvalsettings-complex-type"></a>tipo complexo approvalSettings

Namespace: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Usada para a `requestApprovalSettings` propriedade de uma [política de atribuição de pacote do Access](accesspackageassignmentpolicy.md). Fornece configurações adicionais para selecionar quem deve aprovar cada solicitação. 

## <a name="properties"></a>Propriedades

| Propriedade                     | Tipo                      | Descrição |
| :--------------------------- | :------------------------ | :---------- |
| isApprovalRequired | Boolean | Se for false, a aprovação não será necessária para solicitações nesta política. |
| isApprovalRequiredForExtension | Boolean| Se for false, a aprovação não será necessária para um usuário que já tenha uma atribuição para estender sua atribuição. |
| isRequestorJustificationRequired | Boolean | Indica se o solicitante é necessário para fornecer uma justificativa em sua solicitação. |
| approvalmode| String | Um de `NoApproval`, `SingleStage` ou `Serial`. O `NoApproval` é usado quando `isApprovalRequired` é falso. |
| approvalStages | coleção [approvalStage](approvalstage.md)| Se for necessário aprovar, um ou dois elementos dessa coleção define cada um dos estágios de aprovação. Uma matriz vazia se nenhuma aprovação for necessária.  |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON da propriedade solicitar configurações de aprovação.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.approvalSettings",
  "baseType": ""
}-->

```json
{
    "isApprovalRequired": true,
    "isApprovalRequiredForExtension": false,
    "isRequestorJustificationRequired": true,
    "approvalMode": "Serial",
    "approvalStages": [{"@odata.type": "microsoft.graph.approvalStage"}]
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
