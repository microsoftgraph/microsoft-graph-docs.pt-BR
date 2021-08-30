---
title: tipo de recurso userTeamwork
description: 'Um contêiner dos recursos do Microsoft Teams disponíveis por usuário. '
author: akjo
doc_type: resourcePageType
ms.localizationpriority: high
ms.prod: microsoft-teams
ms.openlocfilehash: 89ad4d479135972c0bbcfa14163a750ba10841a3
ms.sourcegitcommit: c333953a9188b4cd4a9ab94cbe68871e8f3563e5
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/30/2021
ms.locfileid: "58695592"
---
# <a name="userteamwork-resource-type"></a>tipo de recurso userTeamwork

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Um contêiner para o intervalo de funcionalidades do Microsoft Teams disponíveis por usuário no locatário.

## <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição |
|:---------------|:--------|:----------|
|id|cadeia de caracteres| Um identificador exclusivo. |

## <a name="relationships"></a>Relações

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


