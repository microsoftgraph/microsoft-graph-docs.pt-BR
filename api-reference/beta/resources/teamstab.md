---
title: tipo de recurso teamsTab
description: 'Um teamsTab é uma guia fixa (anexada) a um canal dentro de uma equipe. '
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
ms.openlocfilehash: 6666fbcd69ac46e778ef46380c426c4e94a129fc
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33345671"
---
# <a name="teamstab-resource-type"></a>tipo de recurso teamsTab

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Um teamsTab é uma [guia](../resources/teamstab.md) fixa (anexada) a um [canal](channel.md) dentro de uma [equipe](team.md). 

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno  |Descrição|
|:---------------|:--------|:----------|
|[Listar guias](../api/teamstab-list.md) | [teamsTab](teamstab.md) | Lista guias fixadas a um canal.|
|[Obter guia](../api/teamstab-get.md) | [teamsTab](teamstab.md) | Lê uma guia fixada a um canal.|
|[Adicionar guia](../api/teamstab-add.md) | [teamsTab](teamstab.md) | Adiciona (fixa) uma guia a um canal.|
|[Guia remover](../api/teamstab-delete.md) | Nenhum | Remove (desfixa) uma guia de um canal.|
|[Atualizar guia](../api/teamstab-update.md) | [teamsTab](teamstab.md) | Atualiza as propriedades da guia.|


## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---------------|:--------|:----------|
|  id              |   string                  |  Identificador que identifica exclusivamente uma instância específica de uma guia de canal. somente leitura.     |
|  displayName            |   string                  |  Nome da guia.     |
|  name            |   string                  |  Preterido Nome da guia.     |
|  teamsAppId           |   string             |  Identificador de definição de aplicativo da guia. Este valor não pode ser alterado após a criação de tabulação.     |
|  sortOrderIndex  |   string                  |  Índice da ordem usada para classificar as guias.     |
|  webUrl          |   cadeia de caracteres                  |  URL de link profundo da instância de guia. Somente leitura.     |
|  Configuration        |   [teamsTabConfiguration](teamstabconfiguration.md) |  Contêiner para configurações personalizadas aplicadas a uma guia. A guia é considerada configurada somente quando essa propriedade é definida.     |

## <a name="relationships"></a>Relações

| Relação | Tipo   | Descrição |
|:---------------|:--------|:----------|
|teamsApp|[teamsApp](teamsapp.md) | O aplicativo que está vinculado à guia. |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.


<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.teamsTab"
}-->

```json
{
  "id": "string",
  "displayName": "string",
  "teamsAppId": "string",
  "sortOrderIndex": "string",
  "webUrl": "string",
  "configuration": "teamsTabConfiguration",
  "name": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "teamsTab resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->

## <a name="see-also"></a>Confira também

[Configurar tipos de guia internos](/graph/teams-configuring-builtin-tabs)
