---
title: Tipo de recurso de usuário
description: 'Um canal é uma coleção de chatMessages dentro de uma equipe. '
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: d58a3e0b867a675e378fa126108331fd5b27856c
ms.sourcegitcommit: a4773239d8559899c3f9433b3073e250a56d2e04
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/13/2019
ms.locfileid: "29994465"
---
# <a name="channel-resource-type"></a>Tipo de recurso de usuário

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Um canal é uma coleção de [chatMessages](chatmessage.md) dentro de um [equipe](../resources/team.md). Um canal representa um tópico e, portanto, um isolamento lógico da discussão em uma equipe. Os exemplos podem ser o canal “Equipe de almoço da sexta-feira” e o canal “Discussão de arquitetura" .


## <a name="methods"></a>Métodos

| Método       | Tipo de retorno  |Descrição|
|:---------------|:--------|:----------|
|[List channels](../api/channel-list.md) | [channel](channel.md) collection | Obtenha a lista de canais nessa equipe.|
|[Create channel](../api/channel-post.md) | [channel](channel.md) | Crie um novo canal ao incluir o nome de exibição e a descrição.|
|[Get channel](../api/channel-get.md) | [channel](channel.md) | Leia as propriedades e as relações do canal.|
|[Update channel](../api/channel-patch.md) | [channel](channel.md) | Atualize as propriedades do canal.|
|[Delete channel](../api/channel-delete.md) | Nenhum | Exclua um canal.|
|[List channel messages](../api/channel-list-messages.md)  | [chatMessage](../resources/chatmessage.md) | Obtenha mensagens em um canal. |
|[Enviar a mensagem do canal](../api/channel-post-chatmessage.md)  | [chatMessage](../resources/chatmessage.md) | [Enviar uma mensagem para um canal](../api/channel-post-chatmessage.md) |


## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|description|String|Descrição textual opcional do canal.|
|displayName|String|Nome do canal como ele aparecerá ao usuário no Microsoft Teams.|
|id|String|O identificador exclusivo do canal. Somente leitura.|
|isFavoriteByDefault|Boolean|Se o canal deve automaticamente ser marcado como “favorito” para todos os membros da equipe. Padrão: `false`.|
|email|Boolean| O endereço de email para enviar mensagens ao canal. Somente leitura.|
|webUrl|String|Um hiperlink que navegará até o canal no Microsoft Teams. Essa é a URL que você recebe ao clicar com o botão direito do mouse em um canal Microsoft Teams e selecionar Obter o link para o canal. Essa URL deve ser tratada como um blob opaco e não analisado. Somente leitura.|


## <a name="relationships"></a>Relacionamento
| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
|messages|[chatMessage](chatmessage.md) collection|Uma coleção de todas as mensagens do canal. Uma propriedade de navegação. Anulável. No momento, esse API tem suporte apenas à leitura, mas eventualmente terá suporte a mensagens escritas também.|
|guias|[teamsTab](../resources/teamstab.md) collection|Uma coleção de todas as guias do canal. Uma propriedade de navegação.|


## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "messages"
  ],
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
<!--
{
  "type": "#page.annotation",
  "description": "channel resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/channel.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
