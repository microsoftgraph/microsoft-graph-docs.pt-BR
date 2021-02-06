---
title: Tipo complexo approvalSettings
description: Usada para a propriedade requestApprovalSettings de uma diretiva de atribuição de pacote de acesso. Fornece configurações adicionais para selecionar quem deve aprovar cada solicitação.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 99892e0943b993fe43edb4bd104fd2a3a8736a51
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50135252"
---
# <a name="approvalsettings-complex-type"></a>Tipo complexo approvalSettings

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Usado para a propriedade `requestApprovalSettings` de uma política de [atribuição de pacote de acesso.](accesspackageassignmentpolicy.md) Fornece configurações adicionais para selecionar quem deve aprovar cada solicitação. 

## <a name="properties"></a>Propriedades

| Propriedade                     | Tipo                      | Descrição |
| :--------------------------- | :------------------------ | :---------- |
| isApprovalRequired | Boolean | Se for falso, a aprovação não será necessária para solicitações nesta política. |
| isApprovalRequiredForExtension | Boolean| Se for falso, a aprovação não será necessária para um usuário que já tenha uma atribuição para estender sua atribuição. |
| isRequestorJustificationRequired | Boolean | Indica se o solicitante é obrigado a fornecer uma justificativa em sua solicitação. |
| approvalMode| String | Um dos `NoApproval` , `SingleStage` ou `Serial` . O `NoApproval` é usado quando é `isApprovalRequired` falso. |
| approvalStages | [coleção approvalStage](approvalstage.md)| Se a aprovação for necessária, um ou dois elementos dessa coleção definirão cada um dos estágios de aprovação. Uma matriz vazia se nenhuma aprovação for necessária.  |

## <a name="json-representation"></a>Representação JSON

A seguir está uma representação JSON da propriedade de configurações de aprovação de solicitação.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.approvalSettings"
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


