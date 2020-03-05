---
title: tipo de recurso languageProficiency
description: tipo de recurso languageProficiency
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 0934ea66c15e090a4f9ba9bcaa62a6c7eb900cd5
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42522992"
---
# <a name="languageproficiency-resource-type"></a>tipo de recurso languageProficiency

Namespace: Microsoft. Graph

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
