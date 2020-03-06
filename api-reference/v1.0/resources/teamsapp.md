---
title: tipo de recurso teamsApp
description: Um aplicativo no catálogo de aplicativos do Microsoft Teams.
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 5a7cae3ba43915f8dd024e3a9260876adb3ac2a4
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42533510"
---
# <a name="teamsapp-resource-type"></a>tipo de recurso teamsApp

Namespace: microsoft.graph



Um aplicativo no catálogo de aplicativos do [Microsoft Teams](teams-api-overview.md).

Os usuários podem ver esses aplicativos no Microsoft Teams Store e esses aplicativos podem ser instalados nas [equipes](team.md) usando o método [Adicionar aplicativo à equipe](../api/teamsappinstallation-add.md).

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno  |Descrição|
|:---------------|:--------|:----------|
|[Lista de aplicativos publicados](../api/teamsapp-list.md) | Coleção [teamsApp](teamsapp.md) | Lista de aplicativos publicados do catálogo de aplicativos do Microsoft Teams.|
|[Publicar um aplicativo](../api/teamsapp-publish.md) | [teamsApp](teamsapp.md) | Publica um aplicativo ao catálogo de aplicativos da sua organização.|
|[Atualizar um aplicativo publicado](../api/teamsapp-update.md) | [teamsApp](teamsapp.md) | Atualize um aplicativo publicado no catálogo de aplicativos da sua organização.|
|[Remover um aplicativo publicado](../api/teamsapp-delete.md) | Nenhum | Remova um aplicativo publicado do catálogo de aplicativos da sua organização.|

## <a name="properties"></a>Propriedades

| Propriedade            | Tipo     | Descrição |
|:------------------- |:-------- |:----------- |
| id                  | string   | A ID do aplicativo gerada no catálogo de aplicativos (diferente da ID fornecida pelo desenvolvedor em [pacote de aplicativos compactados do Microsoft Teams](/microsoftteams/platform/concepts/apps/apps-package). |
| externalId          | cadeia de caracteres   | A ID do catálogo fornecido pelo desenvolvedor do aplicativo do [pacote de aplicativos compactados do Microsoft Teams](/microsoftteams/platform/concepts/apps/apps-package). |
| displayName                | string   | O nome do catálogo de aplicativos fornecido pelo desenvolvedor do aplicativo no [pacote de aplicativos compactados do Microsoft Teams](/microsoftteams/platform/concepts/apps/apps-package). |
| distributionMethod  | teamsAppDistributionMethod     | O método de distribuição para o aplicativo. |

### <a name="teamsappdistributionmethod-values"></a>valores teamsAppDistributionMethod

|Membro|Valor|Descrição|
|:---|:---|:---|
|loja|0| O aplicativo está disponível para todos os locatários na loja de aplicativos do Microsoft Teams.|
|organização|1|O aplicativo está disponível somente nesse locatário.|
|sideloaded|2|O aplicativo está disponível apenas para usuário/equipe onde ele está instalado.|

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
  "displayName": "Test App",
  "distributionMethod": "Organization"
}
```

## <a name="see-also"></a>Confira também

- [teamsAppInstallation](teamsappinstallation.md)
- [teamsAppDefinition](teamsappdefinition.md)
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

