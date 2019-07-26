---
title: tipo de recurso teamsAppInstallation
description: 'Um teamsApp instalado em uma equipe, um chat ou o escopo pessoal de um usuário. '
author: clearab
doc_type: resourcePageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 55e1246616b7a3d76c6170a02286a2cde2a15d3a
ms.sourcegitcommit: 82b73552fff79a4ef7a2ee57fc2d1b3286b5bd4c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/26/2019
ms.locfileid: "35908506"
---
# <a name="teamsappinstallation-resource-type"></a>tipo de recurso teamsAppInstallation

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Um [teamsApp](teamsapp.md) instalado em uma [equipe](team.md), um [chat](chat.md)ou o escopo pessoal de um [usuário](user.md). Qualquer bots que faça parte do aplicativo se tornará parte de qualquer equipe, chat ou escopo pessoal do usuário ao qual o aplicativo é adicionado.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno  |Descrição|
|:---------------|:--------|:----------|
|[Listar aplicativos instalados no Team](../api/teamsappinstallation-list.md) | Coleção [teamsAppInstallation](teamsappinstallation.md) | Lista os aplicativos instalados em uma equipe.|
|[Adicionar aplicativo à equipe](../api/teamsappinstallation-add.md) |Nenhum | Adiciona (instala) um aplicativo a uma equipe.|
|[Remover aplicativo da equipe](../api/teamsappinstallation-delete.md) | Nenhum | Remove (desinstala) um aplicativo de uma equipe.|
|[Atualizar aplicativo instalado no Team](../api/teamsappinstallation-upgrade.md) | Nenhum | Atualiza para a versão mais recente do aplicativo.|
|[Listar aplicativos instalados para o usuário](../api/user-list-teamsappinstallation.md) | Coleção [teamsAppInstallation](teamsappinstallation.md) | Lista os aplicativos instalados no escopo pessoal de um usuário.|
|[Adicionar aplicativo para usuário](../api/user-add-teamsappinstallation.md) | | Adiciona (instala) um aplicativo no escopo pessoal de um usuário.|
|[Remover o aplicativo para o usuário](../api/user-delete-teamsappinstallation.md) | Nenhum | Remove (desinstala) um aplicativo no escopo pessoal de um usuário.|
|[Atualizar aplicativo instalado para o usuário](../api/user-upgrade-teamsappinstallation.md) | Nenhum | Atualiza para a versão mais recente do aplicativo instalado no escopo pessoal de um usuário.|

## <a name="properties"></a>Propriedades

| Propriedade            | Tipo     | Descrição |
|:------------------- |:-------- |:----------- |
| id                  | string   | Uma ID exclusiva (não a ID de AP da equipe). |

## <a name="relationships"></a>Relações

| Relação   | Tipo    | Descrição |
|:---------------|:--------|:----------|
|teamsApp|[teamsApp](teamsapp.md)| O aplicativo que está instalado. |
|teamsAppDefinition|[teamsAppDefinition](teamsappdefinition.md)| Os detalhes desta versão do aplicativo. |

## <a name="json-representation"></a>Representação JSON

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsAppInstallation",
  "baseType": "microsoft.graph.entity"
}-->

```json
{
  "id": "string"
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
  "suppressions": []
}
-->
