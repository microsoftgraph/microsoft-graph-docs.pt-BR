---
title: tipo de recurso teamsAppDefinition
description: Representa os detalhes de uma versão de um teamsApp.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 322b7f50ccb51702ae05ca55f8e73396321a0283
ms.sourcegitcommit: dc3bade0c096d5ce716d4bc07cd9c7cabb52477b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/18/2020
ms.locfileid: "46791677"
---
# <a name="teamsappdefinition-resource-type"></a>tipo de recurso teamsAppDefinition

Namespace: microsoft.graph

Representa os detalhes de uma versão de um [teamsApp](teamsapp.md).

## <a name="properties"></a>Propriedades

| Propriedade            | Tipo     | Descrição |
|:------------------- |:-------- |:----------- |
| id                  | string   | Uma ID exclusiva (não a ID do aplicativo Teams). |
| teamsAppId          | string   | A ID do manifesto do aplicativo Teams. |
| publishingState| string|O status publicado de uma versão específica de um aplicativo do teams. Os valores possíveis são:</br>`submitted` – A versão específica do aplicativo Teams foi enviada e está em revisão. </br>`published`  — A solicitação para publicar a versão específica do aplicativo Teams foi aprovada pelo administrador e o aplicativo é publicado. </br> `rejected` — A solicitação para publicar a versão específica do aplicativo Teams foi rejeitada pelo administrador. |
| displayName         | string   | O nome do aplicativo fornecido pelo desenvolvedor de aplicativos. |
| versão             | string   | O número da versão do aplicativo. |

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
  "version": "string",
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
