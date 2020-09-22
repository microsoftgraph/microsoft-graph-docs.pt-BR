---
title: tipo de recurso educationalActivityDetail
description: tipo de recurso educationalActivityDetail
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 2f19f5e02ae26281a5ac1b2b48498a426f976e8b
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48055656"
---
# <a name="educationalactivitydetail-resource-type"></a>tipo de recurso educationalActivityDetail

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa detalhes adicionais sobre um Undergraduate, graduação, graduação ou outras atividades educacionais que um usuário fez e é usado em um recurso do [educationalActivity](educationalActivity.md) .

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição                                                   |
|:-------------|:------------|:--------------------------------------------------------------|
|abreviação  |Cadeia de caracteres       |Nome abreviado do grau ou do programa (exemplo: PhD, MBA)    |
|activities    |Cadeia de caracteres       |As atividades do extracurriculares são realizadas junto com o programa.   |
|awards        |Cadeia de caracteres       |Quaisquer prêmios ou honras associados ao programa.              |
|description   |String       |Breve descrição do programa fornecido pelo usuário.         |
|displayName   |Cadeia de caracteres       |Nome de formato longo do programa que o usuário forneceu.      |
|fieldsOfStudy |Cadeia de caracteres       |Principais e menores associados ao programa. (se aplicável) |
|grade         |Cadeia de caracteres       |A classificação final, turma, média ou pontuação.                          |
|notes         |String       |Observações adicionais que o usuário forneceu.                        |
|webUrl        |String       |Link para a página de grau ou de programa.                            |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationalActivityDetail",
  "baseType": null
}-->

```json
{
  "abbreviation": "String",
  "activities": "String",
  "awards": "String",
  "description": "String",
  "displayName": "String",
  "fieldsOfStudy": "String",
  "grade": "String",
  "notes": "String",
  "webUrl": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationalActivityDetail resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

