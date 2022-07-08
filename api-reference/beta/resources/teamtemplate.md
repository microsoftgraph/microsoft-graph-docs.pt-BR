---
title: Tipo de recurso teamTemplate
description: Representa um contêiner lógico para todas as definições e versões do mesmo modelo de equipe.
author: nkramer
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 489818310abeb39ae4055c7360e8f1d909ea9525
ms.sourcegitcommit: c168f2cb95b4863080a84cc199a7b878fb5eeb8e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/08/2022
ms.locfileid: "66690104"
---
# <a name="teamtemplate-resource-type"></a>Tipo de recurso teamTemplate

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um contêiner lógico para todas as definições e versões do mesmo modelo de equipe.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar teamTemplates](../api/teamwork-list-teamtemplates.md)|[coleção teamTemplate](../resources/teamtemplatedefinition.md)| Obtenha uma lista dos **objetos teamTemplate** disponíveis para o locatário.|
|[Definições de lista](../api/teamtemplate-list-definitions.md)| [Coleção teamTemplateDefinition](../resources/teamtemplatedefinition.md) | Liste [os objetos teamTemplateDefinition](../resources/teamstemplate.md) associados a um **teamTemplate**.  |

## <a name="properties"></a>Propriedades

| Propriedade            | Tipo     | Descrição |
|:------------------- |:-------- |:----------- |
| id                  | Cadeia de caracteres   | Identificador exclusivo do modelo. Não pode ser nulo. |

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|Definições|[coleção teamtemplatedefinition](../resources/teamtemplatedefinition.md)| Uma representação genérica de uma definição de modelo de equipe para uma equipe com uma estrutura e configuração específicas.|

## <a name="json-representation"></a>Representação JSON

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamtemplate",
}-->

```json
{
  "id": "string"
}
```

## <a name="see-also"></a>Confira também

- [equipe](team.md)
- [teamTemplateDefinition](teamtemplatedefinition.md)
