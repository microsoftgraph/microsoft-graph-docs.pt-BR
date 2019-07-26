---
title: tipo de recurso de trabalho em equipe
description: Um contêiner dos recursos do Microsoft Teams disponíveis para a organização.
author: clearab
doc_type: resourcePageType
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: 7a72e34fc3d9d02a36e34295f7d4469536506df3
ms.sourcegitcommit: 82b73552fff79a4ef7a2ee57fc2d1b3286b5bd4c
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/26/2019
ms.locfileid: "35908590"
---
# <a name="teamwork-resource-type"></a>tipo de recurso de trabalho em equipe

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Um contêiner para o intervalo de funcionalidades do Microsoft Teams disponíveis para a organização.

## <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição |
|:---------------|:--------|:----------|
|id|cadeia de caracteres| Um identificador exclusivo. |

## <a name="relationships"></a>Relacionamentos

| Relação | Tipo | Descrição |
|:---------------|:--------|:----------|
|installedApps|Coleção [teamsAppInstallation](teamsappinstallation.md)|Os aplicativos instalados no escopo pessoal desse usuário.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamwork",
  "baseType": "microsoft.graph.entity"
}-->

```json
{
  "id": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "teamwork resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->

## <a name="see-also"></a>Confira Também

- [recurso userTeamwork](userteamwork.md)
