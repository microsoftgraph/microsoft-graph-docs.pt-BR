---
title: tipo de recurso de teamsTabConfiguration (Open tipo)
description: As configurações que determinam o conteúdo de uma guia.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 10cc22e70288d1643a3a2cdebe23a012e22e3879
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29519196"
---
# <a name="teamstabconfiguration-resource-type-open-type"></a>tipo de recurso de teamsTabConfiguration (Open tipo)

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

As configurações que determinam o conteúdo de uma [guia](teamstab.md). Quando uma guia interativamente estiver configurada, essas informações são definidas pelo aplicativo do provedor de guia.
Além das propriedades abaixo, alguns aplicativos de provedor de guia especificam propriedades personalizadas adicionais.

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|-|-|-|
|  entityId   |   string |  Identificador da entidade hospedados pelo provedor de guia.     |
|  contentUrl |   string |  URL usada para processar o conteúdo da guia em equipes. Obrigatório.    |
|  removeUrl  |   string |  Chamado pelo cliente de equipes, quando uma guia é removida usando o cliente de equipes de URL.     |
|  websiteUrl |   string |  URL para a exibição de conteúdo da guia fora equipes.     |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsTabConfiguration"
}-->

```json
{
   "entityId": "string",
   "contentUrl": "string (HTTPS Url)",
   "websiteUrl": "string (HTTPS Url)",
   "removeUrl": "string (HTTPS Url)"  
}

```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "teamsTabConfiguration complex type (Open Type)",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/teamstabconfiguration.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
