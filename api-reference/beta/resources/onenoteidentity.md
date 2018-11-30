---
title: tipo de recurso de oneNoteIdentity
description: '**Suporte em breve**'
ms.openlocfilehash: 09c4ee9882a420fb07c6a51be5f361b601573969
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27039744"
---
# <a name="onenoteidentity-resource-type"></a>tipo de recurso de oneNoteIdentity

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

**Suporte em breve**

O tipo de OneNoteIdentity representa uma identidade de um _usuário_.

No futuro, esse tipo de será mesclado com [identidade](identity.md)


## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onenoteidentity"
}-->

```json
{
  "displayName": "string",
  "id": "string"
}

```
## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|displayName|string|Nome para exibição da identidade.|
|id|string|Identificador exclusivo da identidade.|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "oneNoteIdentity resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
