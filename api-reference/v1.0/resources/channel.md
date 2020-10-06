---
title: Tipo de recurso de usuário
description: 'Um canal é uma coleção de chatMessages dentro de uma equipe. '
author: clearab
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: f9860f6d1385374258eeed11dd8db4db21ba895c
ms.sourcegitcommit: 39e48ed2d95b142ccf3f40ecc52441458f2745bf
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/06/2020
ms.locfileid: "48364394"
---
# <a name="channel-resource-type"></a>Tipo de recurso de usuário

Namespace: microsoft.graph

[Teams](../resources/team.md) é formado por canais que são as conversas que você tem com seus colegas. Cada canal é dedicado a um tópico específico, departamento ou projeto. Os canais estão onde o trabalho é feito - onde conversas via texto, áudio e vídeo abertas para toda a equipe ocontecem, onde os arquivos são compartilhados e as guias são adicionadas.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno  |Descrição|
|:---------------|:--------|:----------|
|[List channels](../api/channel-list.md) | [channel](channel.md) collection | Obtenha a lista de canais nessa equipe.|
|[Create channel](../api/channel-post.md) | [channel](channel.md) | Crie um novo canal ao incluir o nome de exibição e a descrição.|
|[Get channel](../api/channel-get.md) | [channel](channel.md) | Leia as propriedades e as relações do canal.|
|[Update channel](../api/channel-patch.md) | [channel](channel.md) | Atualize as propriedades do canal.|
|[Delete channel](../api/channel-delete.md) | Nenhum | Exclua um canal.|
|[Listar guias](../api/teamstab-list.md) | [teamsTab](teamstab.md) | Listar guias fixadas a um canal.|

## <a name="properties"></a>Propriedades

| Propriedade   | Tipo |Descrição|
|:---------------|:--------|:----------|
|description|String|Descrição textual opcional do canal.|
|displayName|String|Nome do canal como ele aparecerá ao usuário no Microsoft Teams.|
|id|String|O identificador exclusivo do canal. Somente leitura.|
|isFavoriteByDefault|Booliano|Indica se o canal deve automaticamente ser marcado como “favorito” para todos os membros da equipe. Só pode ser definida por programação com [Criar equipe](../api/team-post.md). Padrão: `false`.|
|email|Cadeia de caracteres| O endereço de email para enviar mensagens ao canal. Somente leitura.|
|webUrl|String|Um hiperlink que navegará até o canal no Microsoft Teams. Essa é a URL que você recebe ao clicar com o botão direito do mouse em um canal Microsoft Teams e selecionar Obter o link para o canal. Essa URL deve ser tratada como um blob opaco e não analisado. Somente leitura.|
|createdDateTime|dateTimeOffset|Somente leitura. Carimbo de data/hora de criação do canal.|

## <a name="relationships"></a>Relações

| Relação | Tipo |Descrição|
|:---------------|:--------|:----------|
|messages|[chatMessage](chatmessage.md) collection|Uma coleção de todas as mensagens do canal. Uma propriedade de navegação. Anulável.|
|guias|[teamsTab](../resources/teamstab.md) collection|Uma coleção de todas as guias do canal. Uma propriedade de navegação.|
|[filesFolder](../api/channel-get-filesfolder.md)|[driveItem](driveitem.md)|Metadados para o local em que os arquivos do canal estão armazenados.|
|operations|Coleção [teamsAsyncOperation](teamsasyncoperation.md)| As operações assíncronas que foram executadas ou estão em execução nesta equipe. |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

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
  "isFavoriteByDefault": true,
  "email": "string",
  "webUrl": "string",
  "createdDateTime": "string (timestamp)"
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
  "suppressions": []
}
-->
