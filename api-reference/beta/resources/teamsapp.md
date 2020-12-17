---
title: tipo de recurso teamsApp
description: Um aplicativo no catálogo de aplicativos do Microsoft Teams.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: eb7c75f144f2056e610e45f86b44a19d9211f306
ms.sourcegitcommit: ee9e594ad64bef5bc839cf813c0854d083c00aef
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/17/2020
ms.locfileid: "49706119"
---
# <a name="teamsapp-resource-type"></a>tipo de recurso teamsApp

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um aplicativo no catálogo de aplicativos do [Microsoft Teams](teams-api-overview.md).

Os usuários podem ver esses aplicativos no Microsoft Teams Store e esses aplicativos podem ser instalados nas [equipes](team.md) usando o método [Adicionar aplicativo à equipe](../api/team-post-installedapps.md).

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno  |Descrição|
|:---------------|:--------|:----------|
|[Listar aplicativos no catálogo](../api/appcatalogs-list-teamsapps.md) | Coleção [teamsApp](teamsapp.md) | Listar todos os aplicativos no catálogo de aplicativos do Microsoft Teams.|
|[Carregar aplicativo no catálogo](../api/teamsapp-publish.md) | [teamsApp](teamsapp.md) | Carregar um aplicativo para o catálogo de aplicativos da sua organização.|
|[Atualizar aplicativo no catálogo](../api/teamsapp-update.md) | [teamsApp](teamsapp.md) | Atualize um aplicativo no catálogo de aplicativos da sua organização.|
|[Excluir aplicativo do catálogo](../api/teamsapp-delete.md) | Nenhum(a) | Remover um aplicativo do catálogo de aplicativos da sua organização.|
|[Obter bot associado ao aplicativo no catálogo](../api/teamworkbot-get.md) | [teamworkbot](teamworkbot.md) | Obter o bot associado ao aplicativo Teams.|

## <a name="properties"></a>Propriedades

| Propriedade            | Tipo     | Descrição |
|:------------------- |:-------- |:----------- |
| id                  | cadeia de caracteres   | A ID do aplicativo gerada no catálogo de aplicativos (diferente da ID fornecida pelo desenvolvedor em [pacote de aplicativos compactados do Microsoft Teams](/microsoftteams/platform/concepts/apps/apps-package). |
| externalId          | string   | A ID do catálogo fornecido pelo desenvolvedor do aplicativo do [pacote de aplicativos compactados do Microsoft Teams](/microsoftteams/platform/concepts/apps/apps-package). |
| displayName                | string   | O nome do catálogo de aplicativos fornecido pelo desenvolvedor do aplicativo no [pacote de aplicativos compactados do Microsoft Teams](/microsoftteams/platform/concepts/apps/apps-package). |
| distributionMethod  | teamsAppDistributionMethod     | O método de distribuição para o aplicativo. Somente leitura.|

### <a name="teamsappdistributionmethod-values"></a>valores teamsAppDistributionMethod

|Membro|Valor|Descrição|
|:---|:---|:---|
|loja|,0| O aplicativo está disponível para todos os locatários na loja de aplicativos do Microsoft Teams.|
|organização|1|O aplicativo está disponível somente nesse locatário.|
|sideloaded|duas|O aplicativo está disponível apenas para usuário/equipe onde ele está instalado.|

## <a name="relationships"></a>Relações

| Relação | Tipo   | Descrição |
|:---------------|:--------|:----------|
|appDefinitions|Coleção [teamsAppDefinition](teamsappdefinition.md) | Os detalhes para cada versão do aplicativo. |

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
  "displayName": "string",
  "distributionMethod": "string"
}
```

## <a name="see-also"></a>Confira também

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
  "suppressions": []
}
-->



