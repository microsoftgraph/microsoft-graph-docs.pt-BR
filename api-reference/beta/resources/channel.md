---
title: Tipo de recurso de usuário
description: 'Um canal é uma coleção de chatMessages dentro de uma equipe. '
author: akjo
ms.localizationpriority: high
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: c65d9b0a4b418784af1851f87deb0ecef87cd174
ms.sourcegitcommit: 8253b79a9fdfea723899860492219eaeb9f74e3d
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/18/2022
ms.locfileid: "66160696"
---
# <a name="channel-resource-type"></a>Tipo de recurso de usuário

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[Teams](../resources/team.md) é formado por canais que são as conversas que você tem com seus colegas. Cada canal é dedicado a um tópico específico, departamento ou projeto. Os canais estão onde o trabalho é feito - onde conversas via texto, áudio e vídeo abertas para toda a equipe ocontecem, onde os arquivos são compartilhados e as guias são adicionadas.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno  |Descrição|
|:---------------|:--------|:----------|
|[List channels](../api/channel-list.md) | [channel](channel.md) collection | Obtenha a lista de canais em uma equipe.|
|[Lstar canais de entrada](../api/team-list-incomingchannels.md)|Coleção [channel](../resources/channel.md)|Obtenha a lista de [canais](../resources/channel.md) compartilhados com uma **equipe**.|
|[Listar todos os canais](../api/team-list-allchannels.md)|Coleção [channel](../resources/channel.md)|Obtenha a lista de [canais](../resources/channel.md) em uma **equipe** ou compartilhada com uma **equipe** (canais de entrada).|
|[Create channel](../api/channel-post.md) | [channel](channel.md) | Crie um novo canal ao incluir o nome de exibição e a descrição.|
|[Get channel](../api/channel-get.md) | [channel](channel.md) | Leia as propriedades e as relações do canal.|
|[Update channel](../api/channel-patch.md) | [channel](channel.md) | Atualize as propriedades do canal.|
|[Delete channel](../api/channel-delete.md) | Nenhum | Exclua um canal.|
|[Obter o delta de mensagem](../api/chatmessage-delta.md)  | [chatMessage](../resources/chatmessage.md) | Obtenha mensagens incrementais em um canal. |
|[Listar mensagens do canal](../api/channel-list-messages.md)  | [chatMessage](../resources/chatmessage.md) | Obtenha mensagens em um canal. |
|[Obter todas as mensagens do canal](../api/channel-getallmessages.md)|[channel](channel.md) collection | Obter todas as mensagens de todos os chats nos quais um usuário é um participante. |
|[Criar postagem de mensagem no canal](../api/channel-post-messages.md) | [chatMessage](../resources/chatmessage.md) | Envie uma mensagem para um canal. |
|[Criar resposta à postagem da mensagem do canal](../api/chatmessage-post-replies.md) | [chatMessage](../resources/chatmessage.md) | Responda a uma mensagem em um canal.|
|[Obter pasta de arquivos](../api/channel-get-filesfolder.md).| [driveItem](driveitem.md) | Recupera os detalhes da pasta do SharePoint em que os arquivos do canal estão armazenados. |
|[Listar guias](../api/channel-list-tabs.md) | [teamsTab](teamstab.md) | Listar guias fixadas a um canal.|
|[Listar membros do canal](../api/channel-list-members.md) | coleção [conversationMember](conversationmember.md) | Obtenha uma lista de todas as mensagens raiz em um canal.|
|[Adicionar membro do canal](../api/channel-post-members.md) | [conversationMember](conversationmember.md) | Adicionar um membro a um canal. Só há suporte para canais com um **membershipType** de `private` ou `shared`.|
|[Obter canal do membro](../api/channel-get-members.md) | coleção [conversationMember](conversationmember.md) | Obtenha um membro em um canal.|
|[Atualizar a função do membro do canal](../api/channel-update-members.md) | [conversationMember](conversationmember.md) | Atualize as propriedades de um membro do canal. Só há suporte para canais com um **membershipType** de `private` ou `shared`.|
|[Remover membro do canal](../api/channel-delete-members.md) | Nenhum | Exclua um membro de um canal. Só há suporte para canais com um **membershipType** de `private` ou `shared`.|
|[Migração completa](../api/channel-completemigration.md)|[channel](channel.md)| Remove o modo de migração do canal e torna o canal disponível para os usuários postarem e lerem mensagens.|
|[Listar guias no canal](../api/channel-list-tabs.md) | [teamsTab](teamstab.md) | Listar guias fixadas a um canal.|
|[Adicionar uma guia ao canal](../api/channel-post-tabs.md) | [teamsTab](teamstab.md) | Adicionar (fixar) uma guia a um canal.|
|[Guia obter no canal](../api/channel-get-tabs.md) | [teamsTab](teamstab.md) | Ler uma guia fixada a um canal.|
|[Guia atualizar no canal](../api/channel-patch-tabs.md) | [teamsTab](teamstab.md) | Atualiza as propriedades de uma guia em um canal.|
|[Remover guia do canal](../api/channel-delete-tabs.md) | Nenhum | Remover (Desafixar) uma Tabulação de um canal.|
|[Endereço de email do canal de provisão](../api/channel-provisionemail.md) |[provisionChannelEmailResult](../resources/provisionchannelemailresult.md)| Provisione um endereço de e-mail para o canal.|
|[Remover o endereço de email do canal](../api/channel-removeemail.md) | Nenhum | Remova o endereço de e-mail do canal.|
|[Remover canal de entrada](../api/team-delete-incomingchannels.md) | Nenhum| Remova um canal de entrada.|
|[Listar equipes que compartilham um canal](../api/sharedwithchannelteaminfo-list.md)|coleção [sharedWithChannelTeamInfo](../resources/sharedwithchannelteaminfo.md)|Obtenha a lista de equipes que foram compartilhadas no canal especificado.|
|[Obter equipe compartilhando um canal](../api/sharedwithchannelteaminfo-get.md)|[sharedWithChannelTeamInfo](../resources/sharedwithchannelteaminfo.md)|Obtenha uma equipe que tenha sido compartilhada com o canal especificado.|
|[Descompartilhar canal com a equipe](../api/sharedwithchannelteaminfo-delete.md)|Nenhum|Descompartilhe um canal com uma equipe.|
|[Listar membros permitidos](../api/sharedwithchannelteaminfo-list-allowedmembers.md)|[conversationMember](../resources/conversationmember.md)coleção|Obtenha a lista de membros da equipe que têm acesso ao canal compartilhado.|
|[Verificar o acesso do usuário](../api/channel-doesuserhaveaccess.md)|Boolean|Verifique se um usuário tem acesso a um canal compartilhado ou não.|

## <a name="properties"></a>Propriedades

| Propriedade   | Tipo |Descrição|
|:---------------|:--------|:----------|
|description|String|Descrição textual opcional do canal.|
|displayName|String|Nome do canal como ele aparecerá ao usuário no Microsoft Teams.|
|id|Cadeia de caracteres|O identificador exclusivo do canal. Somente leitura.|
|isFavoriteByDefault|Booliano|Indica se o canal deve automaticamente ser marcado como “favorito” para todos os membros da equipe. Só pode ser definida por programação com [Criar equipe](../api/team-post.md). Padrão: `false`.|
|email|Cadeia de caracteres| O endereço de email para enviar mensagens ao canal. Somente leitura.|
|webUrl|String|Um hiperlink que navegará até o canal no Microsoft Teams. Essa é a URL que você recebe ao clicar com o botão direito do mouse em um canal Microsoft Teams e selecionar Obter o link para o canal. Essa URL deve ser tratada como um blob opaco e não analisado. Somente leitura.|
|membershipType|channelMembershipType|O tipo do canal. Pode ser definido durante a criação e não pode ser alterado. Os valores possíveis são: `standard`, `private`, `unknownFutureValue`, `shared`. O valor padrão é `standard`. Observe que você deve usar o cabeçalho de `Prefer: include-unknown-enum-members` solicitação para obter o seguinte valor nessa [enumeração evolutiva](/graph/best-practices-concept#handling-future-members-in-evolvable-enumerations): `shared`.|
|createdDateTime|dateTimeOffset|Somente leitura. Carimbo de data/hora da criação do canal.|
|moderationSettings|[channelModerationSettings](../resources/channelmoderationsettings.md)|Configurações para configurar a moderação do canal para controlar quem pode iniciar novas postagens e responder a postagens no canal.|
|tenantId |cadeia de caracteres | A ID do locatário do Azure Active Directory. |

### <a name="instance-attributes"></a>Atributos de instância

Atributos de instância são propriedades com comportamentos especiais. Essas propriedades são temporárias e a) definem o comportamento que o serviço deve apresentar ou b) fornecem valores de propriedades de curto prazo, como uma URL de download, para um item com data de expiração.

| Nome da propriedade| Tipo   | Descrição
|:-----------------------|:-------|:-------------------------|
|@microsoft.graph.channelCreationMode|string|Indica que o canal está em estado de migração e está sendo usado atualmente para fins de migração. Aceita um valor: `migration`.|

> **Observação**: `channelCreationMode`  é um enum que usa o valor `migration`.

Para obter um exemplo de uma solicitação POST, confira [Solicitação (criar canal no estado de migração)](/microsoftteams/platform/graph-api/import-messages/import-external-messages-to-teams#request-create-a-team-in-migration-state).

## <a name="relationships"></a>Relações

| Relação | Tipo |Descrição|
|:---------------|:--------|:----------|
|messages|[chatMessage](chatmessage.md) collection|Uma coleção de todas as mensagens no canal. Uma propriedade de navegação. Anulável.|
|guias|[teamsTab](../resources/teamstab.md) collection|Uma coleção de todas as guias no canal. Uma propriedade de navegação.|
|members|coleção [conversationMember](conversationmember.md)|Uma coleção de registros de associação ligados ao canal.|
|[filesFolder](../api/channel-get-filesfolder.md)|[driveItem](driveitem.md)|Metadados para o local em que os arquivos do canal estão armazenados.|
|operations|Coleção [teamsAsyncOperation](teamsasyncoperation.md)| As operações assíncronas que foram executadas ou estão em execução nesta equipe. |
|sharedWithTeams|coleção [sharedWithChannelTeamInfo](../resources/sharedwithchannelteaminfo.md)|Uma coleção de equipes com as quais um canal é compartilhado.|

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
  "membershipType": "channelMembershipType",
  "createdDateTime": "string (timestamp)",
  "moderationSettings": { "@odata.type": "microsoft.graph.channelModerationSettings" }
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
