---
author: tushar20
title: Tipo de recurso sharePointIdentity
ms.localizationpriority: medium
description: Representa a SharePoint identidade de um ator.
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: b235f3271c9a39bd99672ad1e0b374f1af5e1b19
ms.sourcegitcommit: e1dd9860906e0b415fd376d70df1f928d1f3d29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/01/2021
ms.locfileid: "61243028"
---
# <a name="sharepointidentity-resource-type"></a>Tipo de recurso sharePointIdentity

Representa **a sharePointIdentity** de um _ator_.

Esse recurso se estende do recurso **de** identidade para fornecer a capacidade de expor SharePoint informações específicas; por exemplo, **loginName** ou SharePoint IDs.

## <a name="properties"></a>Propriedades

| Propriedade         | Tipo                        | Descrição |
|:------------     |:----------------------------|:--------------------------------- |
| displayName      | String                      | Nome de exibição da identidade. Observe que isso pode nem sempre estar disponível ou atualizado. Por exemplo, se um usuário troca seu nome de exibição, a API pode mostrar o novo valor em uma resposta futura, mas os itens associados ao usuário não aparecem como tendo sido alterados ao se usar [delta](../api/driveitem-delta.md). |
| id               | String                      | Identificador exclusivo da identidade. Pode ser uma ID Azure Active Directory ou uma SharePoint ID. |
| loginName        | Cadeia de caracteres                      | O nome de login da identidade SharePoint. |
| miniaturas       | Coleção [thumbnailSet][] | Coleção que contém [objetos thumbnailSet][] associados ao item. Para obter mais informações, consulte [Listar miniaturas para um driveItem][]. Somente leitura. Anulável. |

## <a name="json-representation"></a>Representação JSON

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.sharePointIdentity",
  "openType": true,
  "optionalProperties": ["displayName", "thumbnails"]
} -->

```json
{
  "loginName": "string",

  /** inherited from Identity */
  "displayName": "string",
  "id": "string",
  "thumbnails": [{ "@odata.type": "microsoft.graph.thumbnailSet" }]
}
```

[thumbnailSet]: thumbnailset.md
[Listar miniaturas para um driveItem]: ../api/driveitem-list-thumbnails.md

<!-- {
  "type": "#page.annotation",
  "description": "SharePoint Identity contains information about an app, user, or group.",
  "keywords": "sharePointIdentity, loginName, sharePointId, owner, modifier, app, user, group",
  "section": "documentation",
  "tocPath&quot;: &quot;Resources/SharePointIdentity"
} -->
