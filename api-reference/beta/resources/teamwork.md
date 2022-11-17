---
title: tipo de recurso de trabalho em equipe
description: Um contêiner dos recursos do Microsoft Teams disponíveis para a organização.
author: akjo
doc_type: resourcePageType
ms.localizationpriority: high
ms.prod: microsoft-teams
ms.openlocfilehash: 721335785b1fa70ad9433d1c03b7fe4c9ae89d05
ms.sourcegitcommit: cf2b3c67cb9ce832944cfbac66171590bbbd83de
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/06/2022
ms.locfileid: "66645292"
---
# <a name="teamwork-resource-type"></a>tipo de recurso de trabalho em equipe

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Um contêiner para o intervalo de funcionalidades do Microsoft Teams disponíveis para a organização.

## <a name="methods"></a>Métodos

| Método                                                  | Tipo de retorno                                         |Descrição                                                                               |
|:--------------------------------------------------------|:----------------------------------------------------|:-----------------------------------------------------------------------------------------|
|[Listar deletedTeams](../api/teamwork-list-deletedteams.md)|coleção [deletedTeam](../resources/deletedteam.md)|Obtenha uma lista de objetos [deletedTeam](../resources/deletedteam.md) e suas propriedades.|

## <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição |
|:---------------|:--------|:----------|
|id|cadeia de caracteres| Um identificador exclusivo. |

## <a name="relationships"></a>Relações

| Relação | Tipo | Descrição |
|:---------------|:--------|:----------|
|deletedTeams|coleção [deletedTeam](../resources/deletedteam.md)| Uma coleção de equipes excluídas.|
|dispositivos|Coleção [teamworkDevice](../resources/teamworkdevice.md)|Os dispositivos do Teams provisionados para o locatário.|
|teamsAppSettings|[teamsAppSettings](../resources/teamsappsettings.md)|Representa configurações de todo o locatário para todos os [aplicativos do Teams](teamsapp.md) no locatário.|
|workforceIntegrations|Coleção [workforceIntegration](../resources/workforceintegration.md)| Uma integração de força de trabalho com turnos.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamwork",
  "baseType": "microsoft.graph.entity"
}-->

``` json
{
    "@odata.type": "#microsoft.graph.teamwork",
    "id": "String (identifier)"
}
```

## <a name="see-also"></a>Confira também

- [recurso userTeamwork](userteamwork.md)

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
