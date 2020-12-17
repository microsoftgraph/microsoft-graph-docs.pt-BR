---
title: tipo de recurso teamsAppDefinition
description: Os detalhes de uma versão de um teamsApp.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 6b5fd771d1fb38de5354c74778f5eae798ccc91e
ms.sourcegitcommit: ee9e594ad64bef5bc839cf813c0854d083c00aef
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/17/2020
ms.locfileid: "49706112"
---
# <a name="teamsappdefinition-resource-type"></a>tipo de recurso teamsAppDefinition

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Os detalhes de uma versão de um [teamsApp](teamsapp.md).

## <a name="properties"></a>Propriedades

| Propriedade            | Tipo     | Descrição |
|:------------------- |:-------- |:----------- |
| id                  | string   | Uma ID exclusiva (não a AppID do Teams). |
| teamsAppId          | string   | A ID do manifesto do aplicativo Teams. |
| publishingState| string|O status publicado de uma versão específica de um aplicativo do teams. Os valores possíveis são:</br>`submitted` – A versão específica do aplicativo Teams foi enviada e está em revisão. </br>`published`  — A solicitação para publicar a versão específica do aplicativo Teams foi aprovada pelo administrador e o aplicativo é publicado. </br> `rejected` — A solicitação para publicar a versão específica do aplicativo Teams foi rejeitada pelo administrador. |
| azureADAppId        | string   | O WebApplicationInfo.id do manifesto do aplicativo Teams. |
| displayName         | string   | O nome do aplicativo fornecido pelo desenvolvedor de aplicativos. |
| versão             | string   | O número da versão do aplicativo. |

## <a name="relationships"></a>Relações

| Relação | Tipo   | Descrição |
|:---------------|:--------|:----------|
|bot|[teamworkBot](teamworkbot.md) | Os detalhes do bot especificado no manifesto do aplicativo Teams. |

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
  "displayName": "Test App",
  "version": "1.0.0"
}
```

## <a name="see-also"></a>Confira também

- [teamsApp](teamsapp.md)
- [teamsAppInstallation](teamsappinstallation.md)
- [teamsTab](../resources/teamstab.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "teamsApp resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


