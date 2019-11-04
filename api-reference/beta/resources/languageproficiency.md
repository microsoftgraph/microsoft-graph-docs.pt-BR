---
title: tipo de recurso languageProficiency
description: tipo de recurso languageProficiency
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 4e2ea70eca4e830ef334e5bf61be724cb05f1cfc
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939289"
---
# <a name="languageproficiency-resource-type"></a>tipo de recurso languageProficiency

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa informações detalhadas sobre os idiomas que um usuário adicionou ao [perfil](profile.md).

Herda de [Myfacet](itemFacet.md).

## <a name="methods"></a>Métodos

| Método                                                       | Tipo de retorno                                   | Descrição                                                      | 
|:-------------------------------------------------------------|:----------------------------------------------|:-----------------------------------------------------------------|
| [Obter languageProficiency](../api/languageproficiency-get.md) | [languageProficiency](languageproficiency.md) | Leia as propriedades e os relacionamentos de um objeto **languageProficiency** . |
| [Atualizar languageProficiency](../api/languageproficiency-update.md)               | [languageProficiency](languageproficiency.md) | Atualizar um objeto **languageProficiency** .                               |
| [Excluir languageProficiency](../api/languageproficiency-delete.md)               | Nenhum                                          | Excluir um objeto **languageProficiency** .                               |

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição                                                                                                                                                 |
|:-------------|:------------|:------------------------------------------------------------------------------------------------------------------------------------------------------------|
|displayName   |String       | Contém o nome de formato longo para o idioma.                                                                                                   |
|proficiência   |string       | Os valores possíveis são: `elementary`, `conversational`, `limitedWorking`, `professionalWorking`, `fullProfessional`, `nativeOrBilingual`, `unknownFutureValue`.|
|tag           |String       | Contém o nome BCP47 de quatro caracteres para o idioma (en-US, no-NB, en-AU).                                                                                  |

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso. 

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.languageProficiency",
  "baseType": ""
}-->

```json
{
  "displayName": "String",
  "proficiency": "string",
  "tag": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "languageProficiency resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
