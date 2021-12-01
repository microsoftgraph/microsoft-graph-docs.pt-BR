---
author: tushar20
title: Tipo de recurso sharePointIdentitySet
ms.localizationpriority: medium
description: Representa uma coleção chave de recursos de identidade e sharePointIdentity.
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 7b830d593c2fab775a7be8c4513a50fc278fdd37
ms.sourcegitcommit: e1dd9860906e0b415fd376d70df1f928d1f3d29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/01/2021
ms.locfileid: "61243032"
---
# <a name="sharepointidentityset-resource-type"></a>Tipo de recurso sharePointIdentitySet

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma coleção chave de [recursos sharePointIdentity.](sharePointidentity.md) Esse recurso se estende do recurso **identitySet** para fornecer a capacidade de expor SharePoint informações específicas ao usuário.

Esse recurso é usado para representar um conjunto de identidades associado a vários eventos para um item, como criado por _ou_ modificado pela última _vez por_.

Para obter informações de uso, [consulte driveItem][].

## <a name="properties"></a>Propriedades

| Propriedade    | Tipo                   | Descrição |
|:------------|:-----------------------|:----------------------------------------------------------- |
| aplicativo | [identity][]           | O aplicativo associado a essa ação. Opcional. |
| device      | [identity][]           | O dispositivo associado a essa ação. Opcional. |
| group       | [identity][]           | O grupo associado a essa ação. Opcional. |
| usuário        | [identity][]           | O usuário associado a essa ação. Opcional. |
| siteUser    | [sharePointIdentity][] | O SharePoint usuário associado a essa ação. Opcional. |
| siteGroup   | [sharePointIdentity][] | O SharePoint grupo associado a essa ação. Opcional. |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.sharePointIdentitySet",
       "optionalProperties": ["user", "application", "group", "device", "siteUser", "siteGroup"],
       "openType": true } -->

```json
{
  /** inherited from IdentitySet **/
  "application": {"@odata.type": "microsoft.graph.identity"},
  "device": {"@odata.type": "microsoft.graph.identity"},
  "user": {"@odata.type": "microsoft.graph.identity"},
  
  "group": {"@odata.type": "microsoft.graph.identity"},
  "siteUser": {"@odata.type": "microsoft.graph.sharePointIdentity"},
  "siteGroup":{"@odata.type": "microsoft.graph.sharePointIdentity"}
}
```

[driveItem]: driveitem.md
[identity]: identity.md
[sharePointIdentity]: sharePointidentity.md

<!-- {
  "type": "#page.annotation",
  "description": "SharePointIdentity set is a collection of identities/sharePointIdentities",
  "section": "documentation",
  "tocPath&quot;: &quot;Resources/SharePointIdentitySet"
} -->
