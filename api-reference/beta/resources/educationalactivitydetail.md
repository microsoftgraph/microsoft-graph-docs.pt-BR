---
title: tipo de recurso educationalActivityDetail
description: tipo de recurso educationalActivityDetail
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: ccacf02184bbf54e49949d7671d34dde93b3859f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42502820"
---
# <a name="educationalactivitydetail-resource-type"></a>tipo de recurso educationalActivityDetail

Namespace: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa detalhes adicionais sobre um Undergraduate, graduação, graduação ou outras atividades educacionais que um usuário fez e é usado em um recurso do [educationalActivity](educationalActivity.md) .

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição                                                   |
|:-------------|:------------|:--------------------------------------------------------------|
|abreviação  |String       |Nome abreviado do grau ou do programa (exemplo: PhD, MBA)    |
|activities    |String       |As atividades do extracurriculares são realizadas junto com o programa.   |
|concede        |String       |Quaisquer prêmios ou honras associados ao programa.              |
|description   |String       |Breve descrição do programa fornecido pelo usuário.         |
|displayName   |Cadeia de caracteres       |Nome de formato longo do programa que o usuário forneceu.      |
|fieldsOfStudy |String       |Principais e menores associados ao programa. (se aplicável) |
|grade         |String       |A classificação final, turma, média ou pontuação.                          |
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