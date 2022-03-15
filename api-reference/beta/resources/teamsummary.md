---
title: Tipo de recurso teamSummary
description: Contém informações sobre uma equipe no Microsoft Teams, incluindo números de proprietários, membros e convidados.
ms.localizationpriority: medium
author: akhilkohlimicrosoft
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 497ac22cf95c30b4510c08b04e591c7acaf8c449
ms.sourcegitcommit: 0fa7148e0b776663eaca3e79e72b85046d4b8b1a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/15/2022
ms.locfileid: "63500977"
---
# <a name="teamsummary-resource-type"></a>Tipo de recurso teamSummary

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Contém informações sobre uma equipe no Microsoft Teams, incluindo o número de proprietários, membros e convidados.

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|guestsCount|Int32|Contagem de convidados em uma equipe.|
|membersCount|Int32|Contagem de membros em uma equipe.|
|ownersCount|Int32|Contagem de proprietários em uma equipe.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamSummary"
}-->

```json
{
    "guestsCount": "Integer",
    "membersCount": "Integer",
    "ownersCount": "Integer",
}
```


