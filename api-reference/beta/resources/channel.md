---
title: tipo de recurso de canal
description: 'Um canal é uma coleção de chatMessages dentro de uma equipe. '
ms.openlocfilehash: 90a2c6641a79829e340f2487d7f0381998d2a205
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27040288"
---
# <a name="channel-resource-type"></a>tipo de recurso de canal

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Um canal é uma coleção de [chatMessages](chatmessage.md) dentro de uma [equipe](../resources/team.md). Um canal representa um tópico e, portanto, um isolamento lógico discussão, dentro de uma equipe. Exemplos podem ser canal "Sexta-feira equipe almoço" e "Discussão sobre a arquitetura" channel.


## <a name="methods"></a>Métodos

| Método       | Tipo de retorno  |Descrição|
|:---------------|:--------|:----------|
|[Canais de lista](../api/channel-list.md) | coleção de [canal](channel.md) | Obter a lista de canais nesse conjunto.|
|[Criar canal](../api/channel-post.md) | [canal](channel.md) | Crie um novo canal, incluindo o nome para exibição e a descrição.|
|[Obtenha o canal](../api/channel-get.md) | [canal](channel.md) | Leia as propriedades e os relacionamentos do canal.|
|[Canal de atualização](../api/channel-patch.md) | [canal](channel.md) | Atualize propriedades do canal.|
|[Excluir um canal](../api/channel-delete.md) | Nenhum | Exclua um canal.|
|[Lista de mensagens de canal](../api/channel-list-messages.md)  | [chatMessage](../resources/chatmessage.md) | Obter mensagens em um canal |
|[Criar thread de bate-papo](../api/channel-post-chatthreads.md) | coleção [chatThread](chatthread.md)| Crie um segmento de bate-papo no canal especificado.|

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|description|String|Descrição textual opcional para o canal.|
|displayName|String|Nome de canal como ele será exibido ao usuário no Microsoft Teams.|
|id|String|Identificador exclusivo dos canais. Somente leitura.|

## <a name="relationships"></a>Relações
| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
|mensagens|coleção [chatMessage](chatmessage.md)|Uma coleção de todas as mensagens no canal. Uma propriedade de navegação. Anulável. Atualmente, essa API suporta leitura apenas mas eventualmente dará suporte a mensagens de escrita muito.|
|chatThreads|coleção [chatThread](chatthread.md)|(Isso é sendo substituídos gradualmente à propriedade mensagens) chatThreads oferece suporte à criação de novas mensagens, mas não a leitura de mensagens. ChatThreads é uma propriedade de navegação e é Nullable.|
|guias|coleção [teamsTab](../resources/teamstab.md)|Uma coleção de todas as guias no canal. Uma propriedade de navegação.|


## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "chatthreads"
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
<!-- {
  "type": "#page.annotation",
  "description": "channel resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
