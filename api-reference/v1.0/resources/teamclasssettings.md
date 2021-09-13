---
title: Tipo de recurso teamClassSettings
description: Representa configurações específicas para equipes do tipo Classe.
ms.localizationpriority: medium
author: akjo
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: fd7a3163abd23d7c009ef3a03c668335eeb1e453
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59134357"
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

