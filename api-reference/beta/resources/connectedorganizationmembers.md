---
title: tipo complexo connectedOrganizationMembers
description: O tipo connectedOrganizationMembers identifica uma coleção de usuários no locatário que serão permitidos como solicitante, Aprovador ou revisor.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 20f4477998547d6e98572fd8409f69e811c2198d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507489"
---
# <a name="connectedorganizationmembers-complex-type"></a>tipo complexo connectedOrganizationMembers

Namespace: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Usado nas configurações de solicitação de uma [política de atribuição de pacote do Access](accesspackageassignmentpolicy.md). O `@odata.type` valor `#microsoft.graph.connectedOrganizationMembers` indica que esse tipo identifica uma coleção de usuários, os que estão associados a uma organização conectada, que terá permissão para solicitar um pacote do Access.

## <a name="properties"></a>Propriedades

Este tipo tem as seguintes propriedades:

| Propriedade                     | Tipo                      | Descrição |
| :--------------------------- | :------------------------ | :---------- |
| id |Cadeia de caracteres | A ID da organização conectada no gerenciamento de qualificação. |
| description |String | O nome da organização conectada. Somente leitura. |
| IsBackup | Boolean | Não usado no momento. |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do tipo.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.connectedOrganizationMembers",
  "baseType": "microsoft.graph.userSet"
}-->

```json
{
  "id": "string (identifier)",
  "description": "string",
  "isBackup": false
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "connectedOrganizationMembers complex type",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
