---
title: tipo de recurso teamsAppInstallation
description: 'Um teamsApp instalado em uma equipe. '
author: clearab
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 70dfe86840bd908a2e626b7f965d89251b9221aa
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42533501"
---
# <a name="teamsappinstallation-resource-type"></a>tipo de recurso teamsAppInstallation

Namespace: microsoft.graph

Um [teamsApp](teamsapp.md) instalado em uma [equipe](team.md). Qualquer bots que faça parte do aplicativo se tornará parte de qualquer equipe à qual o aplicativo é adicionado.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno  |Descrição|
|:---------------|:--------|:----------|
|[Listar aplicativos](../api/teamsappinstallation-list.md) | [teamsAppInstallation](teamsappinstallation.md) | Lista os aplicativos instalados em uma equipe.|
|[Adicionar aplicativo](../api/teamsappinstallation-add.md) | [teamsAppInstallation](teamsappinstallation.md) | Adiciona (instala) um aplicativo a uma equipe.|
|[Remover aplicativo](../api/teamsappinstallation-delete.md) | Nenhum | Remove (desinstala) um aplicativo de uma equipe.|
|[Atualizar aplicativo](../api/teamsappinstallation-upgrade.md) | Nenhum | Atualiza para a versão mais recente do aplicativo.|

## <a name="properties"></a>Propriedades

| Propriedade            | Tipo     | Descrição |
|:------------------- |:-------- |:----------- |
| id                  | string   | Uma ID exclusiva (não a AppID do Teams). |

## <a name="relationships"></a>Relacionamento

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
<!-- {
  "type": "#page.annotation",
  "description": "teamsApp resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
