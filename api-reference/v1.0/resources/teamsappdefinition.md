---
title: Tipo de recurso teamsAppDefinition
description: Representa os detalhes de uma versão de um teamsApp.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: b247432171f5de9d2624d7793f25ab6bfdce91fe
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50470666"
---
# <a name="teamsappdefinition-resource-type"></a>Tipo de recurso teamsAppDefinition

Namespace: microsoft.graph

Representa os detalhes de uma versão de um [teamsApp](teamsapp.md).

## <a name="properties"></a>Propriedades

| Propriedade            | Tipo     | Descrição |
|:------------------- |:-------- |:----------- |
| id                  | string   | Uma ID exclusiva (não a ID do aplicativo do Teams). |
| teamsAppId          | string   | A ID do manifesto do aplicativo teams. |
| publishingState| string|O status publicado de uma versão específica de um aplicativo do Teams. Os valores possíveis são:</br>`submitted` — A versão específica do aplicativo teams foi enviada e está sob revisão. </br>`published`  — A solicitação para publicar a versão específica do aplicativo teams foi aprovada pelo administrador e o aplicativo é publicado. </br> `rejected` — A solicitação para publicar a versão específica do aplicativo teams foi rejeitada pelo administrador. |
| displayName         | string   | O nome do aplicativo fornecido pelo desenvolvedor do aplicativo. |
| versão             | string   | O número da versão do aplicativo. |
| shortDescription    | string   | Descrição curta do aplicativo. |
| description         | string   | Descrição detalhada do aplicativo. |

## <a name="relationships"></a>Relações

| Relação | Tipo   | Descrição |
|:---------------|:--------|:----------|
|bot|[teamworkBot](teamworkbot.md) | Os detalhes do bot especificados no manifesto do aplicativo teams. |

## <a name="json-representation"></a>Representação JSON

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsAppDefinition",
  "baseType": "microsoft.graph.entity"
}-->

```json
{
  "id": "string",
  "teamsAppId": "string",
  "displayName": "string",
  "version": "string"
}
```

## <a name="see-also"></a>Confira também

- [teamsApp](teamsapp.md)
- [teamsAppInstallation](teamsappinstallation.md)
- [teamsTab](../resources/teamstab.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "teamsApp resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

