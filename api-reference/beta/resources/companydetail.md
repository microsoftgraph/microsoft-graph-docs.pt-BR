---
title: tipo de recurso companyDetail
description: tipo de recurso companyDetail
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 04e33c9fdae1eae811ee88e7cdef95b4b97b2c3f
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37936836"
---
# <a name="companydetail-resource-type"></a>tipo de recurso companyDetail

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa informações sobre as empresas relacionadas às entidades em seu [perfil](profile.md).

## <a name="properties"></a>Propriedades

| Propriedade       | Tipo                                | Descrição                                 |
|:---------------|:------------------------------------|:--------------------------------------------|
|address         |[physicalAddress](physicaladdress.md)| Endereço da empresa.                     |
|department      |String                               | Nome do departamento dentro de uma empresa.           |
|displayName     |Cadeia de caracteres                               | Nome da empresa.                               |
|officeLocation  |String                               | Local do escritório da pessoa que se refere.  |
|pronúncia   |String                               | Guia de pronúncia para o nome da empresa.   |
|webUrl          |String                               | Link para a Home Page da empresa.              |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.companyDetail",
  "baseType": null
}-->

```json
{
  "address": {"@odata.type": "microsoft.graph.physicalAddress"},
  "department": "String",
  "displayName": "String",
  "officeLocation": "String",
  "pronunciation": "String",
  "webUrl": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "companyDetail resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->