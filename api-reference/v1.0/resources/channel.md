---
title: Tipo de recurso de usuário
description: 'Um canal é um conjunto de mensagens dentro de uma equipe. '
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: 6c1f73746081e5b1e4f78acb91d43e33c1c9bf73
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32569456"
---
# <a name="channel-resource-type"></a>Tipo de recurso de usuário

[Teams](../resources/team.md) é formado por canais que são as conversas que você tem com seus colegas. Cada canal é dedicado a um tópico específico, departamento ou projeto.
Os canais estão onde o trabalho é feito - onde conversas via texto, áudio e vídeo abertas para toda a equipe ocontecem, onde os arquivos são compartilhados e as guias são adicionadas.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno  |Descrição|
|:---------------|:--------|:----------|
|[List channels](../api/channel-list.md) | [channel](channel.md) collection | Obtenha a lista de canais nessa equipe.|
|[Create channel](../api/channel-post.md) | [channel](channel.md) | Crie um novo canal ao incluir o nome de exibição e a descrição.|
|[Get channel](../api/channel-get.md) | [channel](channel.md) | Leia as propriedades e as relações do canal.|
|[Update channel](../api/channel-patch.md) | [channel](channel.md) | Atualize as propriedades do canal.|
|[Delete channel](../api/channel-delete.md) | Nenhum | Exclua um canal.|
|[Listar guias](../api/teamstab-list.md) | [teamsTab](teamstab.md) | Listar guias fixadas a um canal.|
|[Obter guia](../api/teamstab-get.md) | [teamsTab](teamstab.md) | Ler uma guia fixada a um canal.|
|[Adicionar guia](../api/teamstab-add.md) | [teamsTab](teamstab.md) | Adicionar (fixar) uma guia em um canal.|
|[Remover guia](../api/teamstab-delete.md) | Nenhum | Remover (desafixar) uma guia de um canal.|
|[Guia de atualização](../api/teamstab-update.md) | [teamsTab](teamstab.md) | Atualizar as propriedades da guia.|

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|description|String|Descrição textual opcional do canal.|
|displayName|String|Nome do canal como ele aparecerá ao usuário no Microsoft Teams.|
|email|Cadeia de caracteres| O endereço de email para enviar mensagens ao canal. Somente leitura.|
|id|String|O identificador exclusivo do canal. Somente leitura.|
|webUrl|String|Um hiperlink que navegará até o canal no Microsoft Teams. Essa é a URL que você recebe ao clicar com o botão direito do mouse em um canal Microsoft Teams e selecionar Obter o link para o canal. Essa URL deve ser tratada como um blob opaco e não analisado. Somente leitura.|

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
  "email": "string (identifier)",
  "id": "string",
  "webUrl": "string"
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
