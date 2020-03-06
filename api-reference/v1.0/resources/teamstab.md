---
title: tipo de recurso teamsTab
description: 'Um teamsTab é uma guia fixa (anexada) a um canal dentro de uma equipe. '
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: c62905699b8986d9594ccad06d154d93b71313fc
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42533477"
---
# <a name="teamstab-resource-type"></a>tipo de recurso teamsTab

Namespace: microsoft.graph



Um teamsTab é uma [guia](../resources/teamstab.md) fixa (anexada) a um [canal](channel.md) dentro de uma [equipe](team.md). 

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno  |Descrição|
|:---------------|:--------|:----------|
|[Listar guias](../api/teamstab-list.md) | [teamsTab](teamstab.md) | Listar guias fixadas a um canal.|
|[Obter guia](../api/teamstab-get.md) | [teamsTab](teamstab.md) | Ler uma guia fixada a um canal.|
|[Adicionar guia](../api/teamstab-add.md) | [teamsTab](teamstab.md) | Adicionar (fixar) uma guia em um canal.|
|[Remover guia](../api/teamstab-delete.md) | Nenhum | Remover (desafixar) uma guia de um canal.|
|[Guia de atualização](../api/teamstab-update.md) | [teamsTab](teamstab.md) | Atualizar as propriedades da guia.|


## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---------------|:--------|:----------|
|  id              |   string                  |  Identificador que identifica exclusivamente uma instância específica de uma guia de canal. somente leitura.     |
|  displayName            |   string                  |  Nome da guia.     |
|  webUrl          |   cadeia de caracteres                  |  URL de link profundo da instância de guia. Somente leitura.     |
|  Configuration        |   [teamsTabConfiguration](teamstabconfiguration.md) |  Contêiner para configurações personalizadas aplicadas a uma guia. A guia é considerada configurada somente quando essa propriedade é definida.     |

## <a name="relationships"></a>Relacionamento

| Relação | Tipo   | Descrição |
|:---------------|:--------|:----------|
|teamsApp|[teamsApp](teamsapp.md) | O aplicativo que está vinculado à guia. Isso não pode ser alterado após a criação da Tabulação. |

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
  "webUrl": "string",
  "configuration" : "teamsTabConfiguration"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "teamsTab resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

## <a name="see-also"></a>Confira também

[Configurar tipos de guia internos](/graph/teams-configuring-builtin-tabs)
