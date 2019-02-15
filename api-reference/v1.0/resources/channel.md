---
title: Tipo de recurso de usuário
description: 'Um canal é um conjunto de mensagens dentro de uma equipe. '
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: 052c6d8fc298e929dfd1c69e1b64debb7e14eb4a
ms.sourcegitcommit: a4773239d8559899c3f9433b3073e250a56d2e04
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/13/2019
ms.locfileid: "29994451"
---
# <a name="channel-resource-type"></a>Tipo de recurso de usuário



Um canal é um conjunto de mensagens em um [equipe](../resources/team.md). Um canal representa um tópico e, portanto, um isolamento lógico da discussão em uma equipe. Os exemplos podem ser o canal “Equipe de almoço da sexta-feira” e o canal “Discussão de arquitetura" .


## <a name="methods"></a>Métodos

| Método       | Tipo de retorno  |Descrição|
|:---------------|:--------|:----------|
|[List channels](../api/channel-list.md) | [channel](channel.md) collection | Obtenha a lista de canais nessa equipe.|
|[Create channel](../api/channel-post.md) | [channel](channel.md) | Crie um novo canal ao incluir o nome de exibição e a descrição.|
|[Get channel](../api/channel-get.md) | [channel](channel.md) | Leia as propriedades e as relações do canal.|
|[Update channel](../api/channel-patch.md) | [channel](channel.md) | Atualize as propriedades do canal.|
|[Delete channel](../api/channel-delete.md) | Nenhum | Exclua um canal.|

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|description|String|Descrição textual opcional do canal.|
|displayName|String|Nome do canal como ele aparecerá ao usuário no Microsoft Teams.|
|id|String|O identificador exclusivo do canal. Somente leitura.|

## <a name="relationships"></a>Relacionamento
| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
|guias|[teamsTab](../resources/teamstab.md) collection|Uma coleção de todas as guias do canal. Uma propriedade de navegação.|


## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.channel"
}-->

```json
{
  "description": "string",
  "displayName": "string",
  "id": "string (identifier)",
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "channel resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
