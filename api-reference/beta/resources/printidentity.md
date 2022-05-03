---
title: Tipo de recurso printIdentity
description: Representa uma identidade dentro do serviço de Impressão Universal. Mapas a um Azure AD grupo.
author: braedenp-msft
ms.localizationpriority: medium
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 6132cabcb0aa7dfff94207a38b963aefe568fe29
ms.sourcegitcommit: 267e3baf545c8dc71ba2ab69497e3ec369379f43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/03/2022
ms.locfileid: "65176335"
---
# <a name="printidentity-resource-type"></a>Tipo de recurso printIdentity

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma identidade dentro do serviço de Impressão Universal. Mapas a um [grupo Azure Active Directory (Azure AD).](group.md)

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|id|Cadeia de caracteres|O identificador de printIdentity. Somente leitura.|
|displayName|Cadeia de caracteres|O nome de exibição da printIdentity.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.printIdentity",
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity"
}-->

```json
{
  "id": "String (identifier)",
  "displayName": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "printIdentity resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


