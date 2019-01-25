---
title: tipo de recurso de teamsAppInstallation
description: 'Um teamsApp instalado em uma equipe. '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: b4cf14c36fc0ab0b33f88d4b330e76957e65164a
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29512833"
---
# <a name="teamsappinstallation-resource-type"></a>tipo de recurso de teamsAppInstallation

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Um [teamsApp](teamsapp.md) instalado em uma [equipe](team.md). Qualquer bots que fazem parte do aplicativo se tornará parte de qualquer aplicativo é adicionado de equipe.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno  |Descrição|
|:---------------|:--------|:----------|
|[Lista de aplicativos](../api/teamsappinstallation-list.md) | [teamsAppInstallation](teamsapp.md) | Lista os aplicativos instalados em uma equipe.|
|[Adicionar aplicativo](../api/teamsappinstallation-add.md) | [teamsAppInstallation](teamsapp.md) | Adiciona (instala) um aplicativo para uma equipe.|
|[Remover aplicativo](../api/teamsappinstallation-delete.md) | Nenhum | Remove (desinstala) um aplicativo da equipe.|
|[Atualizar o aplicativo](../api/teamsappinstallation-delete.md) | Nenhum | Atualizações para a versão mais recente do aplicativo.|

## <a name="properties"></a>Propriedades

| Propriedade            | Tipo     | Descrição |
|:------------------- |:-------- |:----------- |
| id                  | string   | Uma identificação exclusiva (não o appid equipes). |

## <a name="relationships"></a>Relacionamento

| Relação   | Tipo    | Descrição |
|:---------------|:--------|:----------|
|teamsApp|[teamsApp](teamsapp.md)| O aplicativo que está instalado. |
|teamsAppDefinition|[teamsAppDefinition](teamsapp.md)| Os detalhes desta versão do aplicativo. |

## <a name="json-representation"></a>Representação JSON

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsAppInstallation",
  "baseType": "microsoft.graph.entity"
}-->

```json
{
  "id": "string",
}
```

# <a name="see-also"></a>Confira também

- [teamsApp](teamsapp.md)
- [teamsAppDefinition](teamsappdefinition.md)
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
  "suppressions": [
    "Error: /api-reference/beta/resources/teamsappinstallation.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

