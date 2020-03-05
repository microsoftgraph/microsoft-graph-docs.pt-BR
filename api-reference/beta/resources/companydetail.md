---
title: tipo de recurso companyDetail
description: tipo de recurso companyDetail
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: dc8da38c9da8d6631e8e46199f420ae0b3ab652e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507580"
---
# <a name="companydetail-resource-type"></a>tipo de recurso companyDetail

Namespace: Microsoft. Graph

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