---
title: tipo complexo connectedOrganizationMembers
description: O tipo connectedOrganizationMembers identifica uma coleção de usuários no locatário que serão permitidos como solicitante, aprovador ou revisor.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 725926bc39583bda653294f0cc917ea7d2f08a45
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761811"
---
# <a name="connectedorganizationmembers-complex-type"></a>tipo complexo connectedOrganizationMembers

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Usado nas configurações de solicitação de uma política de atribuição [de pacote de acesso.](accesspackageassignmentpolicy.md) O valor indica que esse tipo identifica uma coleção de usuários, aqueles associados a uma organização conectada, que terão permissão para solicitar `@odata.type` `#microsoft.graph.connectedOrganizationMembers` um pacote de acesso. [](connectedorganization.md)

## <a name="properties"></a>Propriedades

Esse tipo tem as seguintes propriedades:

| Propriedade                     | Tipo                      | Descrição |
| :--------------------------- | :------------------------ | :---------- |
| id |Cadeia de caracteres | A ID da organização conectada no gerenciamento de direitos. |
| descrição |Cadeia de caracteres | O nome da organização conectada. Somente leitura. |
| isBackup | Boolean | Não é usado no momento. |

## <a name="json-representation"></a>Representação JSON

A seguir está uma representação JSON do tipo.

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


