---
title: tipo de recurso de equipe
description: 'No Microsoft Teams, uma equipe é um conjunto de canais. '
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 48cc5a44ffca20b435d9095d7f25fd5bfa65b4e8
ms.sourcegitcommit: 7ceec757fd82ef3fd80aa3089ef46d3807aa3aa2
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/09/2020
ms.locfileid: "48405537"
---
# <a name="team-resource-type"></a>tipo de recurso de equipe

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

No Microsoft Teams, uma equipe é um conjunto de objetos de [canal](channel.md). Um canal representa um tópico e, portanto, um isolamento lógico da discussão em uma equipe.

Cada equipe está associada a um [grupo](../resources/group.md). O grupo tem a mesma ID da equipe, por exemplo, `/groups/{id}/team` é o mesmo `/teams/{id}`. Confira mais informações sobre como trabalhar com grupos e membros em equipes, confira [Usar a API REST do Microsoft Graph para trabalhar com o Microsoft Teams](teams-api-overview.md).

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno  |Descrição|
|:---------------|:--------|:----------|
|[Criar equipe](../api/team-post.md) | [teamsAsyncOperation](teamsasyncoperation.md) | Crie uma equipe do zero. |
|[Criar equipe a partir do grupo](../api/team-put-teams.md) | [team](team.md) | Crie uma nova equipe ou adicione uma equipe a um grupo existente.|
|[Obter equipe](../api/team-get.md) | [team](team.md) | Recupere as propriedades e relações da equipe especificada.|
|[Atualizar equipe](../api/team-update.md) | [team](team.md) |Atualize as propriedades da equipe especificada. |
|[Excluir equipe](../api/group-delete.md) | Nenhum |Exclua a equipe e o grupo associado. |
|[Listar membros](../api/team-list-members.md)|coleção [conversationMember](../resources/conversationmember.md)|Obtenha o conversationMembers da propriedade de navegação dos membros.|
|[Adicionar membros](../api/team-post-members.md)|[conversationMember](../resources/conversationmember.md)|Adicionar um novo membro.|
|[Remover membros](../api/team-delete-members.md)|Nenhum|Excluir um objeto [conversationMember](../resources/conversationmember.md).|
|[Alterar a função do membro](../api/conversationmember-update.md)|[conversationMember](../resources/conversationmember.md)|Alterar um membro para um proprietário ou voltar para um membro regular.|
|[Arquivar equipe](../api/team-archive.md) | [teamsAsyncOperation](../resources/teamsasyncoperation.md) |Coloque a equipe em um estado somente leitura. |
|[Desarquivar equipe](../api/team-unarchive.md) | [teamsAsyncOperation](../resources/teamsasyncoperation.md) |Restaure a equipe com um estado de leitura e gravação. |
|[Clonar equipe](../api/team-clone.md) | [teamsAsyncOperation](../resources/teamsasyncoperation.md) |Copie a equipe e o grupo associado. |
|[Listar suas equipes](../api/user-list-joinedteams.md) | Coleção [team](team.md) | Liste as equipes das quais você é membro. |
|[Obter foto da equipe](../api/team-get-photo.md) | Dados Binários | Obter a foto (imagem) de uma equipe. |

## <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição |
|:---------------|:--------|:----------|
|displayName|string| O nome da equipe. |
|description|string| Uma descrição opcional para a equipe. |
|classificação|string| Um rótulo opcional. Normalmente descreve a confidencialidade da empresa ou dos dados da equipe. Deve coincidir com um dos conjuntos predefinidos no diretório do locatário. |
|specialization|[teamSpecialization](teamspecialization.md)| Opcional. Indica se a equipe destina-se a um caso de uso específico.  Cada especialização de equipe tem acesso a comportamentos e experiências exclusivos direcionados ao seu caso de uso. |
|visibility|[teamVisibilityType](teamvisibilitytype.md)| A visibilidade de um grupo e equipe. O padrão é Público. |
|funSettings|[teamFunSettings](teamfunsettings.md) |Configurações que definem o uso de Giphy, memes e figurinhas na equipe.|
|guestSettings|[teamGuestSettings](teamguestsettings.md) |Configurações que definem se os convidados podem criar, atualizar ou excluir canais na equipe.|
|internalId | string | Uma ID exclusiva da equipe, que foi usada em alguns locais, como o log de auditoria da [API da Atividade de Gestão do Office 365](/office/office-365-management-api/office-365-management-activity-api-reference). |
|isArchived|Booliano|Se essa equipe está no modo somente leitura. |
|memberSettings|[teamMemberSettings](teammembersettings.md) |Configurações para configurar se os membros podem executar determinadas ações, por exemplo, criar canais e adicionar bots na equipe.|
|messagingSettings|[teamMessagingSettings](teammessagingsettings.md) |Configurações para definir a mensagens e menções na equipe.|
|discoverySettings|[teamDiscoverySettings](teamdiscoverysettings.md) |Configurações de capacidade de descoberta da equipe por outras pessoas.|
|webUrl|cadeia de caracteres (somente leitura) | Um hiperlink que será enviado à equipe no cliente do Microsoft Teams. Esta é a URL que você recebe ao clicar com o botão direito do mouse em uma equipe no cliente do Microsoft Teams e escolher **Obter o link para a equipe**. Essa URL deve ser tratada como um blob opaco e não analisado. |
|classSettings|[teamClassSettings](teamclasssettings.md) |Definir configurações de uma classe. Disponível apenas quando a equipe representa uma classe.|
|isMembershipLimitedToOwners|Booliano|Se definido para `true`, a equipe está atualmente no estado de membro da equipe apenas para o proprietário e não é acessível a outros membros da equipe, tais como estudantes.|
|createdDateTime|dateTimeOffset|Somente leitura. Carimbo de data/hora de criação da equipe.|

### <a name="instance-attributes"></a>Atributos de instância

Atributos de instância são propriedades com comportamentos especiais. Essas propriedades são temporárias e a) definem o comportamento que o serviço deve apresentar ou b) fornecem valores de propriedades de curto prazo, como uma URL de download, para um item com data de expiração.

| Nome da propriedade| Tipo   | Descrição
|:-----------------------|:-------|:-------------------------|
|@microsoft.graph.teamCreationMode|cadeia de caracteres|Indica que a equipe está no estado de migração e está sendo usada no momento para fins de migração. Aceita um valor: `migration`.|

Para obter um exemplo de uma solicitação POST, confira [Solicitação (criar equipe no estado de migração)](https://github.com/MicrosoftDocs/msteams-docs/blob/add-import-messages/msteams-platform/graph-api/import-messages/import-external-messages-to-teams.md#request-create-team-in-migration-state).

## <a name="relationships"></a>Relações

| Relação | Tipo | Descrição |
|:---------------|:--------|:----------|
|channels|Coleção [channel](channel.md)|A coleção de canais e mensagens associadas à equipe.|
|installedApps|Coleção [teamsAppInstallation](teamsappinstallation.md)|Os aplicativos instalados nessa equipe.|
|members|coleção [conversationMember](../resources/conversationmember.md)|Membros e proprietários da equipe.|
|owners|[user](user.md)| A lista de proprietários desta equipe. Atualmente, ao criar uma equipe usando permissões de aplicativo, exatamente um proprietário deve ser especificado. Ao usar permissões delegadas pelo usuário, nenhum proprietário pode ser especificado (o usuário atual é o proprietário). O proprietário deve ser especificado como um objeto ID (GUID), não um UPN. |
|operations|Coleção [teamsAsyncOperation](teamsasyncoperation.md)| As operações assíncronas que foram executadas ou estão em execução nesta equipe. | 
|photo|[profilePhoto](../resources/profilephoto.md)|Foto da equipe.|
|[primaryChannel](../api/team-get-primarychannel.md)|[channel](channel.md)| O canal geral da equipe. | 
|Cronograma|[Cronograma](schedule.md)| Cronograma de turno para essa equipe.|
|template|[teamsTemplate](teamstemplate.md)| O modelo usado para criar essa equipe. Confira os [modelos disponíveis](/MicrosoftTeams/get-started-with-teams-templates). |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

>**Observação:** se a equipe for do tipo classe, uma propriedade **classSettings** será aplicada à equipe.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.team",
  "baseType": "microsoft.graph.entity"
}-->

```json
{
  "guestSettings": {"@odata.type": "microsoft.graph.teamGuestSettings"},
  "memberSettings": {"@odata.type": "microsoft.graph.teamMemberSettings"},
  "messagingSettings": {"@odata.type": "microsoft.graph.teamMessagingSettings"},
  "funSettings": {"@odata.type": "microsoft.graph.teamFunSettings"},
  "discoverySettings": {"@odata.type": "microsoft.graph.teamDiscoverySettings"},
  "internalId": "string",
  "isArchived": false,
  "webUrl": "string (URL)",
  "displayName": "string",
  "description": "string",
  "classification": "string",
  "specialization": "string",
  "visibility": "string",
  "classSettings": {"@odata.type": "microsoft.graph.teamClassSettings"},
  "isMembershipLimitedToOwners":"boolean",
  "createdDateTime": "string (timestamp)"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "team resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->

## <a name="see-also"></a>Confira também

- [Usar o API do Microsoft Graph para trabalhar com o Microsoft Teams](teams-api-overview.md)
- [Como criar um grupo com uma equipe](/graph/teams-create-group-and-team)
- [Listar todas as equipes](/graph/teams-list-all-teams)


