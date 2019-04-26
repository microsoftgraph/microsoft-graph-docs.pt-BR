---
title: tipo de recurso teamsApp
description: Um aplicativo no catálogo de aplicativos do Microsoft Teams.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: fe60222ae6c5d8475722e18e69555df2d3892759
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32553946"
---
# <a name="teamsapp-resource-type"></a>tipo de recurso teamsApp

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Um aplicativo no catálogo de aplicativos do [Microsoft Teams](teams-api-overview.md) .

Os usuários podem ver esses aplicativos no Microsoft Teams Store, e esses aplicativos podem ser instalados [](team.md) no Teams usando o método [Add App to Team](../api/teamsappinstallation-add.md) .

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno  |Descrição|
|:---------------|:--------|:----------|
|[Listar aplicativos publicados](../api/teamsapp-list.md) | Coleção [teamsApp](teamsapp.md) | Listar aplicativos publicados do catálogo de aplicativos do Microsoft Teams.|
|[Publicar um aplicativo](../api/teamsapp-publish.md) | [teamsApp](teamsapp.md) | Publicar um aplicativo no catálogo de aplicativos da sua organização.|
|[Atualizar um aplicativo publicado](../api/teamsapp-update.md) | [teamsApp](teamsapp.md) | Atualize um aplicativo publicado no catálogo de aplicativos da sua organização.|
|[Remover um aplicativo publicado](../api/teamsapp-delete.md) | Nenhum | Remover um aplicativo publicado do catálogo de aplicativos da sua organização.|

## <a name="properties"></a>Propriedades

| Propriedade            | Tipo     | Descrição |
|:------------------- |:-------- |:----------- |
| id                  | string   | A ID do aplicativo gerado pelo aplicativo de catálogo (diferente da ID fornecida pelo desenvolvedor no [pacote de aplicativos zip do Microsoft Teams](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package). |
| externalId          | string   | A ID do catálogo fornecido pelo desenvolvedor de aplicativos no pacote de [aplicativos zip do Microsoft Teams](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package). |
| displayName                | string   | O nome do aplicativo de catálogo fornecido pelo desenvolvedor de aplicativos no [pacote de aplicativos zip do Microsoft Teams](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package). |
| distributionMethod  | teamsAppDistributionMethod     | O método de distribuição para o aplicativo. |

### <a name="teamsappdistributionmethod-values"></a>valores de teamsAppDistributionMethod

|Member|Valor|Descrição|
|:---|:---|:---|
|Guarde|,0| O aplicativo está disponível para todos os locatários por meio da loja de aplicativos do Microsoft Teams.|
|organization|1 |O aplicativo está disponível somente neste locatário.|
|suplementos foi feito|2 |O aplicativo está disponível somente para o usuário/equipe em que ele está instalado.|

## <a name="relationships"></a>Relações

| Relação | Tipo   | Descrição |
|:---------------|:--------|:----------|
|appDefinitions|coleção [teamsAppDefinition](teamsappdefinition.md)| Os detalhes para cada versão do aplicativo. |

## <a name="json-representation"></a>Representação JSON

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsApp",
  "baseType": "microsoft.graph.entity"
}-->

```json
{
  "id": "string",
  "externalId": "string",
  "displayName": "Test App",
  "distributionMethod": "Organization"
}
```

# <a name="see-also"></a>Confira também

- [teamsAppInstallation](teamsappinstallation.md)
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
    "Error: /api-reference/beta/resources/teamsapp.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

