---
title: tipo de recurso teamsTab
description: 'Um teamsTab é uma guia fixa (anexada) a um canal dentro de uma equipe. '
localization_priority: Normal
author: AkJo
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 38351b0bde174b03f0e01392e7c8ec9c4df0db44
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/11/2020
ms.locfileid: "49660111"
---
# <a name="teamstab-resource-type"></a>tipo de recurso teamsTab

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Um teamsTab é uma [guia](../resources/teamstab.md) fixa (anexada) a um [canal](channel.md) dentro de uma [equipe](team.md). 

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno  |Descrição|
|:---------------|:--------|:----------|
|[Listar guias no canal](../api/channel-list-tabs.md) | [teamsTab](teamstab.md) | Listar guias fixadas a um canal.|
|[Guia obter no canal](../api/channel-get-tabs.md) | [teamsTab](teamstab.md) | Ler uma guia fixada a um canal.|
|[Adicionar uma guia ao canal](../api/channel-post-tabs.md) | [teamsTab](teamstab.md) | Adicionar (fixar) uma guia a um canal.|
|[Guia atualizar no canal](../api/channel-patch-tabs.md) | [teamsTab](teamstab.md) | Atualiza as propriedades de uma guia em um canal.|
|[Remover guia do canal](../api/channel-delete-tabs.md) | Nenhum | Remover (Desafixar) uma Tabulação de um canal.|
|[Guias de lista no chat](../api/chat-list-tabs.md) | [teamsTab](teamstab.md) | Listar guias fixadas a um chat.|
|[Guia obter no chat](../api/chat-get-tabs.md) | [teamsTab](teamstab.md) | Obtenha uma guia específica fixada para um chat.|
|[Adicionar guia ao chat](../api/chat-post-tabs.md) | [teamsTab](teamstab.md) | Adicionar (fixar) uma guia a um chat.|
|[Guia atualizar no chat](../api/chat-patch-tabs.md) | [teamsTab](teamstab.md) | Atualizar as propriedades de uma guia em um chat.|
|[Guia remover do chat](../api/chat-delete-tabs.md) | Nenhum | Remover (Desafixar) uma guia de um chat.|



## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---------------|:--------|:----------|
|  id              |   string                  |  Identificador que identifica exclusivamente uma instância específica de uma guia de canal. somente leitura.     |
|  displayName            |   string                  |  Nome da guia.     |
|  nome (preterido)      |   string                  |  Nome da guia.     |
|  teamsAppId (preterido)|   string             |  Identificador de definição de aplicativo da guia. Este valor não pode ser alterado após a criação de tabulação. Como essa propriedade foi preterida, recomendamos expandir **teamsApp** para recuperar o aplicativo vinculado à guia. |
|  sortOrderIndex  |   string                  |  Índice da ordem usada para classificar as guias.     |
|  webUrl          |   cadeia de caracteres                  |  URL de link profundo da instância de guia. Somente leitura.     |
|  configuração        |   [teamsTabConfiguration](teamstabconfiguration.md) |  Contêiner para configurações personalizadas aplicadas a uma guia. A guia é considerada configurada somente quando essa propriedade é definida.     |

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


