---
title: tipo de recurso userTeamwork
description: 'Um contêiner dos recursos do Microsoft Teams disponíveis por usuário. '
author: clearab
doc_type: resourcePageType
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: f633f6ea214374aa7171bdd6ada24f4fadb4b507
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519488"
---
# <a name="userteamwork-resource-type"></a>tipo de recurso userTeamwork

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Um contêiner para o intervalo de funcionalidades do Microsoft Teams disponíveis por usuário no locatário.

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
  "@odata.type": "microsoft.graph.userTeamwork",
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
  "description": "userteamwork resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
