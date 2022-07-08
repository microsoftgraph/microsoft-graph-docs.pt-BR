---
title: tipo de recurso de trabalho em equipe
description: Um contêiner para o intervalo de funcionalidades do Microsoft Teams disponíveis para a organização.
author: charlieforce
ms.localizationpriority: medium
ms.prod: teamwork
doc_type: resourcePageType
ms.openlocfilehash: 3c5282ff44f2ae56d40e666548e222ccfb6e13f4
ms.sourcegitcommit: c168f2cb95b4863080a84cc199a7b878fb5eeb8e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/08/2022
ms.locfileid: "66690008"
---
# <a name="teamwork-resource-type"></a>tipo de recurso de trabalho em equipe

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Um contêiner para o intervalo de funcionalidades do Microsoft Teams disponíveis para a organização. 

Herda de [entidade](../resources/entity.md).

## <a name="methods"></a>Methods
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar deletedTeams](../api/teamwork-list-deletedteams.md)|coleção [deletedTeam](../resources/deletedteam.md)|Obtenha uma lista de objetos [deletedTeam](../resources/deletedteam.md) e suas propriedades.|
|[Listar teamTemplates](../api/teamwork-list-teamtemplates.md)|[coleção teamTemplate](../resources/teamtemplate.md)|Obtenha a lista de [objetos teamTemplate](../resources/teamtemplate.md) disponíveis para o locatário. |

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres| Um identificador exclusivo. Herdado da [entidade](../resources/entity.md).|

## <a name="relationships"></a>Relações
| Relação | Tipo | Descrição |
|:---------------|:--------|:----------|
|deletedTeams|coleção [deletedTeam](../resources/deletedteam.md)| Uma coleção de equipes excluídas.|
|dispositivos|Coleção [teamworkDevice](../resources/teamworkdevice.md)|Os dispositivos do Teams provisionados para o locatário.|
|teamsAppSettings|[teamsAppSettings](../resources/teamsappsettings.md)|Representa configurações de todo o locatário para todos os [aplicativos do Teams](teamsapp.md) no locatário.|
|teamTemplates|[coleção teamtemplate](../resources/teamtemplate.md)| Os modelos associados a uma equipe.|
|workforceIntegrations|Coleção [workforceIntegration](../resources/workforceintegration.md)| Uma integração de força de trabalho com turnos.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.teamwork",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->

``` json
{
    "@odata.type": "#microsoft.graph.teamwork",
    "id": "String (identifier)"
}
```

## <a name="see-also"></a>Confira também

- [recurso userTeamwork](userteamwork.md)

