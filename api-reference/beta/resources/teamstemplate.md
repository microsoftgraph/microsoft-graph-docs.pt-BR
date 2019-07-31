---
title: tipo de recurso Teams
description: Descreve a entidade Teams.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: dde08e6c4ecde3b3a600958a5af5cd93b5fc600f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35964386"
---
# <a name="teamstemplate-resource-type"></a>tipo de recurso Teams

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Um modelo de equipe é um gráfico para a criação de uma [equipe](../resources/team.md) no Microsoft Teams. Um modelo especifica a estrutura, as configurações e até o conteúdo que deve ser provisionado em uma nova equipe criada usando o modelo. A Microsoft fornece um pacote de modelos básicos e os clientes podem salvar seus próprios modelos personalizados.

## <a name="properties"></a>Propriedades

| Propriedade            | Tipo     | Descrição |
|:------------------- |:-------- |:----------- |
| id                  | String   | Identificador exclusivo do modelo. Não pode ser nulo. |

## <a name="json-representation"></a>Representação JSON

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsTemplate",
  "baseType": "microsoft.graph.entity"
}-->

```json
{
  "id": "string"
}
```

# <a name="see-also"></a>Confira também

- [team](team.md)

