---
title: tipo de recurso positionDetail
description: tipo de recurso positionDetail
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 6c77c116f013000ec4d419ec20c1e45c07187a22
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521590"
---
# <a name="positiondetail-resource-type"></a>tipo de recurso positionDetail

Namespace: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa informações sobre posições relacionadas a entidades dentro de um [perfil](profile.md)de usuário.

## <a name="properties"></a>Propriedades

| Propriedade       | Tipo                             | Descrição                                            |
|:---------------|:---------------------------------|:-------------------------------------------------------|
|empresarial         |[companyDetail](companydetail.md) | Detalhes sobre a empresa ou o empregador.                  |
|description     |String                            | Descrição da posição em questão.               |
|endMonthYear    |Data                              | Quando a posição terminou.                               |
|jobTitle        |String                            | O título mantido na posição.                  |
|role            |String                            | A função em que a posição é encaudada.                        |
|startMonthYear  |Data                              | O mês e o ano de início da posição.              |
|summary         |String                            |Breve resumo da posição.                          |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.positionDetail",
  "baseType": null
}-->

```json
{
  "company": {"@odata.type": "microsoft.graph.companyDetail"},
  "description": "String",
  "endMonthYear": "String (timestamp)",
  "jobTitle": "String",
  "role": "String",
  "startMonthYear": "String (timestamp)",
  "summary": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "positionDetail resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->