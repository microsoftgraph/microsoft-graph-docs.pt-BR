---
title: Tipo de recurso teamsAppIcon
description: Um ícone associado a um aplicativo no Microsoft Teams.
author: jecha
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 3e8a256dc0b9e92c414cd3d362bb36579708083f
ms.sourcegitcommit: d033e7de12bccf92efcbe40c7b671e419a3e5b94
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/17/2021
ms.locfileid: "51882638"
---
# <a name="teamsappicon-resource-type"></a>Tipo de recurso teamsAppIcon

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Um ícone associado a um [teamsApp](teamsapp.md).

## <a name="methods"></a>Métodos

| Método                                            | Tipo de retorno                                       | Descrição                                                    | 
| :------------------------------------------------ | :------------------------------------------------ | :------------------------------------------------------------- |
| [Obter ícone](../api/teamsappicon-get.md)     | [teamsAppIcon](teamsappicon.md)                   | Obter um ícone associado a uma versão específica de um aplicativo do Teams. |
| [Obter conteúdo hospedado](../api/teamworkhostedcontent-get.md) | [teamworkHostedContent](teamworkhostedcontent.md) | Obter conteúdo hospedado (e seus bytes) para um ícone.                |

## <a name="properties"></a>Propriedades

| Propriedade      | Tipo                        | Descrição                                                                             |
| :------------ | :-------------------------- | :-------------------------------------------------------------------------------------- |
| id            | cadeia de caracteres                      | A ID exclusiva do ícone do aplicativo.                                                          |
| webUrl        | cadeia de caracteres                      | A URL da Web que pode ser usada para baixar a imagem.                                 |

## <a name="relationships"></a>Relações

| Relação  | Tipo                                              | Descrição                                                                         |
| :------------ | :------------------------------------------------ | :---------------------------------------------------------------------------------- |
| hostedContent | [teamworkHostedContent](teamworkhostedcontent.md) | O conteúdo do ícone do aplicativo se o ícone estiver hospedado na infraestrutura do Teams. |

## <a name="json-representation"></a>Representação JSON

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsAppIcon",
  "baseType": "microsoft.graph.entity"
}-->

```json
{
  "id": "string",
  "webUrl": "string"
}
```

## <a name="see-also"></a>Confira também

- [teamsApp](teamsapp.md)
- [teamsAppDefinition](teamsappdefinition.md)
