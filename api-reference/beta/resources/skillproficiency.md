---
title: tipo de recurso skillProficiency
description: tipo de recurso skillProficiency
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 7c8b5a3711c7abdbbdd8ddba8f7a36c85978718b
ms.sourcegitcommit: 9a6ce4ddf75beead19b7c35a1949cf4d105b9b29
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2020
ms.locfileid: "43228870"
---
# <a name="skillproficiency-resource-type"></a>tipo de recurso skillProficiency

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa informações detalhadas sobre as habilidades associadas a um usuário em vários serviços.

Herda de [Myfacet](itemfacet.md).

## <a name="methods"></a>Métodos
 
| Método                                                         | Tipo de retorno                             | Descrição                                                             |
|:---------------------------------------------------------------|:----------------------------------------|:------------------------------------------------------------------------|
| [Obter skillProficiency](../api/skillproficiency-get.md)         | [skillProficiency](skillproficiency.md) | Leia as propriedades e os relacionamentos de um objeto **skillProficiency** . |
| [Atualizar skillProficiency](../api/skillproficiency-update.md)   | [skillProficiency](skillproficiency.md) | Atualizar um objeto **skillProficiency** .                                   |
| [Excluir skillProficiency](../api/skillproficiency-delete.md)   | Nenhum                                    | Excluir um objeto **skillProficiency** .                                   |

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo             | Descrição                                                                                                                        |
|:-------------|:-----------------|:-----------------------------------------------------------------------------------------------------------------------------------|
|categories    |String collection | Contém categorias que um usuário associou à habilidade (por exemplo, pessoal, profissional, hobby).                             |
|displayName   |Cadeia de caracteres            | Contém um nome amigável para a habilidade.                                                                                            |
|proficiência   |string            | Os possíveis valores são: `elementary`, `limitedWorking`, `generalProfessional`, `advancedProfessional`, `expert`, `unknownFutureValue`.|
|webUrl        |String            | Contém um link para uma fonte de informações sobre a habilidade.                                                                          |

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.skillProficiency",
  "baseType": ""
}-->

```json
{
  "categories": ["String"],
  "displayName": "String",
  "proficiency": "string",
  "webUrl": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "skillProficiency resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
