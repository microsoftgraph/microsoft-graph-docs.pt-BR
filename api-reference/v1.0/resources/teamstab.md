---
title: tipo de recurso teamsTab
description: 'Um teamsTab é uma guia fixa (anexada) a um canal dentro de uma equipe. '
localization_priority: Normal
author: AkJo
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 8314604d6ed15eeb154ff46c8e3b90f4be4f5cde
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/11/2020
ms.locfileid: "49658545"
---
# <a name="teamstab-resource-type"></a>tipo de recurso teamsTab

Namespace: microsoft.graph



Um teamsTab é uma [guia](../resources/teamstab.md) fixa (anexada) a um [canal](channel.md) dentro de uma [equipe](team.md). 

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno  |Descrição|
|:---------------|:--------|:----------|
|[Listar guias](../api/channel-list-tabs.md) | [teamsTab](teamstab.md) | Listar guias fixadas a um canal.|
|[Obter guia](../api/channel-get-tabs.md) | [teamsTab](teamstab.md) | Ler uma guia fixada em um canal.|
|[Adicionar guia](../api/channel-post-tabs.md) | [teamsTab](teamstab.md) | Adicionar (fixar) uma guia a um canal.|
|[Guia de atualização](../api/channel-patch-tabs.md) | [teamsTab](teamstab.md) | Atualize as propriedades da guia.|
|[Remover guia](../api/channel-delete-tabs.md) | Nenhum | Remover (Desafixar) uma Tabulação de um canal.|


## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---------------|:--------|:----------|
|  id              |   string                  |  Identificador que identifica exclusivamente uma instância específica de uma guia de canal. somente leitura.     |
|  displayName            |   string                  |  Nome da guia.     |
|  webUrl          |   cadeia de caracteres                  |  URL de link profundo da instância de guia. Somente leitura.     |
|  configuração        |   [teamsTabConfiguration](teamstabconfiguration.md) |  Contêiner para configurações personalizadas aplicadas a uma guia. A guia é considerada configurada somente quando essa propriedade é definida.     |

## <a name="relationships"></a>Relações

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

