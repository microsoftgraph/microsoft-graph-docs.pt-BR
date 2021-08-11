---
title: Tipo de recurso teamClassSettings
description: Representa configurações específicas para equipes do tipo Classe.
localization_priority: Normal
author: akjo
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 5a28eb208ea36091b272bd38815a6b8bfb3839cbc84fe9c47075f2c85a863e32
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54228972"
---
# <a name="teamclasssettings-resource-type"></a>Tipo de recurso teamClassSettings

Namespace: microsoft.graph

Representa propriedades específicas da classe de uma [equipe](team.md). Disponível apenas quando a equipe representa uma classe.

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|notifyGuardiansAboutAssignments|Booliano|Se definido como , habilita o envio de atribuições semanais digere emails para pais/responsáveis, desde que o administrador do locatário tenha habilitado a `true` configuração globalmente.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamClassSettings"
}-->

```json
{
  "notifyGuardiansAboutAssignments": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "team's classSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->

