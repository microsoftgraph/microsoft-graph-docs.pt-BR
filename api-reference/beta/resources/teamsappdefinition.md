---
title: Tipo de recurso teamsAppDefinition
description: Os detalhes de uma versão de um teamsApp.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 205c656e81ed9dfc75e97cbe0734eeb36c5c0127
ms.sourcegitcommit: aa18eb8a9965f99cc97680808abba8df46f31ba5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/08/2021
ms.locfileid: "51638904"
---
# <a name="teamsappdefinition-resource-type"></a>Tipo de recurso teamsAppDefinition

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Os detalhes de uma versão de um [teamsApp](teamsapp.md).

## <a name="properties"></a>Propriedades

| Propriedade            | Tipo     | Descrição |
|:------------------- |:-------- |:----------- |
| id                  | string   | Uma id exclusiva (não as equipes appid). |
| teamsAppId          | string   | A id do manifesto do Aplicativo do Teams. |
| publishingState| string|O status publicado de uma versão específica de um aplicativo do Teams. Os valores possíveis são:</br>`submitted` — A versão específica do aplicativo teams foi enviada e está sob revisão. </br>`published`  — A solicitação para publicar a versão específica do aplicativo teams foi aprovada pelo administrador e o aplicativo é publicado. </br> `rejected` — A solicitação para publicar a versão específica do aplicativo teams foi rejeitada pelo administrador. |
| azureADAppId        | string   | O WebApplicationInfo.id do manifesto do Aplicativo do Teams. |
| displayName         | string   | O nome do aplicativo fornecido pelo desenvolvedor do aplicativo. |
| versão             | string   | O número da versão do aplicativo. |
| allowedInstallationScopes | Coleção teamsAppInstallationScope | Uma coleção de escopos onde o aplicativo teams pode ser instalado. Os valores possíveis são:</br>`team` — Indica que o aplicativo do Teams pode ser instalado em uma equipe e está autorizado a acessar os dados dessa equipe. </br>`groupChat`  — Indica que o aplicativo do Teams pode ser instalado em um chat de grupo e está autorizado a acessar os dados desse chat de grupo. </br> `personal` — Indica que o aplicativo do Teams pode ser instalado no escopo pessoal de um usuário e está autorizado a acessar os dados desse usuário. | 

## <a name="relationships"></a>Relações

| Relação | Tipo   | Descrição |
|:---------------|:--------|:----------|
|bot|[teamworkBot](teamworkbot.md) | Os detalhes do bot especificados no manifesto do aplicativo teams. |

## <a name="json-representation"></a>Representação JSON

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsAppDefinition",
  "baseType": "microsoft.graph.entity"
}-->

```json
{
  "id": "string",
  "teamsAppId": "string",
  "displayName": "Test App",
  "version": "1.0.0"
}
```

## <a name="see-also"></a>Confira também

- [teamsApp](teamsapp.md)
- [teamsAppInstallation](teamsappinstallation.md)
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


