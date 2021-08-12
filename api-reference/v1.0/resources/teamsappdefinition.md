---
title: Tipo de recurso teamsAppDefinition
description: Representa os detalhes de uma versão de um teamsApp.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 9ca384f507fec1bf813fea20ffb3b0034a5e43de0d92604c81cad84b514f37b8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54218398"
---
# <a name="teamsappdefinition-resource-type"></a>Tipo de recurso teamsAppDefinition

Namespace: microsoft.graph

Representa os detalhes de uma versão de um [teamsApp](teamsapp.md).

## <a name="properties"></a>Propriedades

| Propriedade            | Tipo     | Descrição |
|:------------------- |:-------- |:----------- |
| id                  | string   | Uma ID exclusiva (não Teams ID do aplicativo). |
| teamsAppId          | string   | A ID do manifesto Teams aplicativo. |
| publishingState| string|O status publicado de uma versão específica de um Teams app. Os valores possíveis são:</br>`submitted`— A versão específica do aplicativo Teams foi enviada e está sob revisão. </br>`published`— A solicitação para publicar a versão específica do aplicativo Teams foi aprovada pelo administrador e o aplicativo é publicado. </br> `rejected`— A solicitação para publicar a versão específica do aplicativo Teams foi rejeitada pelo administrador. |
| displayName         | string   | O nome do aplicativo fornecido pelo desenvolvedor do aplicativo. |
| versão             | string   | O número da versão do aplicativo. |
| shortDescription    | string   | Descrição curta do aplicativo. |
| description         | string   | Descrição detalhada do aplicativo. |

## <a name="relationships"></a>Relações

| Relação | Tipo   | Descrição |
|:---------------|:--------|:----------|
|bot|[teamworkBot](teamworkbot.md) | Os detalhes do bot especificados no manifesto Teams aplicativo. |

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

