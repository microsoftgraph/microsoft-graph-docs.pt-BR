---
title: tipo de recurso de equipe
description: No Microsoft Teams, uma equipe é um conjunto de canais.
author: AkJo
ms.localizationpriority: high
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: fa6da0486972982566b6785a8f2aa62fef408b30
ms.sourcegitcommit: af7a33e92d0e84e6108dd5d9466f869061ac0c97
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/19/2022
ms.locfileid: "66856278"
---
# <a name="team-resource-type"></a>tipo de recurso de equipe

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

No Microsoft Teams, uma equipe é um conjunto de objetos de [canal](channel.md). Um canal representa um tópico e, portanto, um isolamento lógico da discussão em uma equipe.

Cada equipe está associada a um [grupo Microsoft 365](../resources/group.md). O grupo tem a mesma ID da equipe, por exemplo, `/groups/{id}/team` é o mesmo `/teams/{id}`. Confira mais informações sobre como trabalhar com grupos e membros em equipes, confira [Usar a API REST do Microsoft Graph para trabalhar com o Microsoft Teams](teams-api-overview.md).

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno  |Descrição|
|:---------------|:--------|:----------|
|[Criar equipe](../api/team-post.md) | [teamsAsyncOperation](teamsasyncoperation.md) | Crie uma equipe do zero. |
|[Criar equipe a partir do grupo](../api/team-put-teams.md) | [team](team.md) | Crie uma nova equipe ou adicione uma equipe a um grupo Microsoft 365 existente.|
|[Obter equipe](../api/team-get.md) | [team](team.md) | Recupere as propriedades e relações da equipe especificada.|
|[Atualizar equipe](../api/team-update.md) | [team](team.md) |Atualize as propriedades da equipe especificada. |
|[Excluir equipe](../api/group-delete.md) | Nenhum |Exclua a equipe e o grupo associado. |
|[Listar membros](../api/team-list-members.md)|coleção [conversationMember](../resources/conversationmember.md)|Obtenha a lista de membros nessa equipe.|
|[Adicionar membro](../api/team-post-members.md)|[conversationMember](../resources/conversationmember.md)|Adicione um novo membro à equipe.|
|[Adicionar membros em massa](../api/conversationmembers-add.md)|coleção[actionResultPart](../resources/actionresultpart.md)|Adicione vários membros à equipe em uma única solicitação.|
|[Obter membro](../api/team-get-members.md) | [conversationMember](conversationmember.md)coleção | Obtenha um membro na equipe.|
|[Atualizar a função do membro](../api/team-update-members.md)|[conversationMember](../resources/conversationmember.md)|Alterar um membro para um proprietário ou voltar para um membro regular.|
|[Remover membro](../api/team-delete-members.md)|Nenhum|Remova um membro existente da equipe.|
|[Arquivar equipe](../api/team-archive.md) | [teamsAsyncOperation](../resources/teamsasyncoperation.md) |Coloque a equipe em um estado somente leitura. |
|[Desarquivar equipe](../api/team-unarchive.md) | [teamsAsyncOperation](../resources/teamsasyncoperation.md) |Restaure a equipe com um estado de leitura e gravação. |
|[Clonar equipe](../api/team-clone.md) | [teamsAsyncOperation](../resources/teamsasyncoperation.md) |Copie a equipe e o grupo associado. |
|[Listar suas equipes](../api/user-list-joinedteams.md) | Coleção [team](team.md) | Liste as equipes das quais você é membro. |
|[Listar equipes associadas](../api/associatedteaminfo-list.md) | Coleção [associatedTeamInfo](associatedteaminfo.md) | Obtenha a lista de objetos [associatedTeamInfo](associatedteaminfo.md) no Microsoft Teams as quais um [usuário](user.md) está associado. |
|[Listar todas as equipes em uma organização](../api/teams-list.md) | Coleção [team](team.md) | Listar todas as equipes em uma organização. |
|[Obter foto da equipe](../api/profilephoto-get.md) | Dados Binários | Obter a foto (imagem) de uma equipe. |
|[Migração completa](../api/team-completemigration.md)|[equipe](team.md)| Remove o modo de migração da equipe e disponibiliza a equipe aos usuários para postar e ler mensagens.|
|[Listar todos os canais](../api/team-list-allchannels.md)|Coleção [channel](../resources/channel.md)|Obtenha a lista de [canais](../resources/channel.md) desta **equipe** ou compartilhados com esta **equipe** (canais de entrada).|
|[List channels](../api/channel-list.md)|[channel](../resources/channel.md) collection|Obtenha a lista de [canais](../resources/channel.md) em uma **equipe**.|
|[Lstar canais de entrada](../api/team-list-incomingchannels.md)|Coleção [channel](../resources/channel.md)|Obtenha a lista de [canais](../resources/channel.md) compartilhados com esta **equipe**.|
|[Remover canal de entrada](../api/team-delete-incomingchannels.md) | Nenhum| Remova um canal de entrada.|
|[Listar aplicativos em equipe](../api/team-list-installedapps.md) | Coleção [teamsAppInstallation](teamsappinstallation.md) | Liste os aplicativos instalados em uma equipe.|
|[Adicionar aplicativo à equipe](../api/team-post-installedapps.md) |Nenhuma | Adicione (instale) um aplicativo a uma equipe.|
|[Instalar o aplicativo na equipe do](../api/team-get-installedapps.md) | [teamsAppInstallation](teamsappinstallation.md) | Obtenha o aplicativo especificado instalado em uma equipe.|
|[Atualizar o aplicativo instalado para a equipe](../api/team-teamsappinstallation-upgrade.md) | Nenhuma | Atualize o aplicativo instalado em uma equipe para a versão mais recente.|
|[Remover aplicativo da equipe](../api/team-delete-installedapps.md) | Nenhuma | Remova (desinstale) um aplicativo de uma equipe.|
|[Listar as concessões de permissões](../api/team-list-permissiongrants.md) | Coleção [resourceSpecificPermissionGrant](resourcespecificpermissiongrant.md) | Liste as permissões que foram concedidas aos aplicativos para acessar a equipe.|

## <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição |
|:---------------|:--------|:----------|
|displayName|string| O nome da equipe. |
|description|string| Uma descrição opcional para a equipe. O comprimento máximo é de 1024 caracteres. |
|classificação|string| Um rótulo opcional. Normalmente descreve a confidencialidade da empresa ou dos dados da equipe. Deve coincidir com um dos conjuntos predefinidos no diretório do locatário. |
|specialization|[teamSpecialization](teamspecialization.md)| Opcional. Indica se a equipe destina-se a um caso de uso específico.  Cada especialização de equipe tem acesso a comportamentos e experiências exclusivos direcionados ao seu caso de uso. |
|visibility|[teamVisibilityType](teamvisibilitytype.md)| A visibilidade de um grupo e equipe. Padrão é Público. |
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
|createdDateTime|dateTimeOffset|Carimbo de data/hora de criação da equipe.|
|summary|[teamSummary](teamsummary.md)| Contém informações resumidas sobre a equipe, incluindo o número de proprietários, membros e convidados. |
|tenantId |cadeia de caracteres | A ID do locatário do Azure Active Directory. |

### <a name="instance-attributes"></a>Atributos de instância

Atributos de instância são propriedades com comportamentos especiais. Essas propriedades são temporárias e a) definem o comportamento que o serviço deve apresentar ou b) fornecem valores de propriedades de curto prazo, como uma URL de download, para um item com data de expiração.

| Nome da propriedade| Tipo   | Descrição
|:-----------------------|:-------|:-------------------------|
|@microsoft.graph.teamCreationMode|cadeia de caracteres|Indica que a equipe está em estado de migração e atualmente está sendo usada para fins de migração. Ele aceita um valor: `migration`. **Observação**: no futuro, a Microsoft pode exigir que você ou seus clientes paguem taxas adicionais com base na quantidade de dados importados.|

Para um exemplo de solicitação POST, confira [Solicitação (criar equipe no estado de migração)](/microsoftteams/platform/graph-api/import-messages/import-external-messages-to-teams).

## <a name="relationships"></a>Relações

| Relação | Tipo | Descrição |
|:---------------|:--------|:----------|
|allChannels|Coleção [channel](channel.md)|Lista de canais hospedados ou compartilhados com a equipe (canais de entrada).|
|channels|Coleção [channel](channel.md)|A coleção de canais e mensagens associadas à equipe.|
|incomingChannels|Coleção [channel](channel.md)|Lista de [canais](../resources/channel.md) compartilhados com a equipe.|
|installedApps|Coleção [teamsAppInstallation](teamsappinstallation.md)|Os aplicativos instalados nessa equipe.|
|members|coleção [conversationMember](../resources/conversationmember.md)|Membros e proprietários da equipe.|
|owners|[user](user.md)| A lista de proprietários desta equipe. Atualmente, ao criar uma equipe usando permissões de aplicativo, exatamente um proprietário deve ser especificado. Ao usar permissões delegadas pelo usuário, nenhum proprietário pode ser especificado (o usuário atual é o proprietário). O proprietário deve ser especificado como um objeto ID (GUID), não um UPN. |
|operations|Coleção [teamsAsyncOperation](teamsasyncoperation.md)| As operações assíncronas que foram executadas ou estão em execução nesta equipe. |
|photo|[profilePhoto](../resources/profilephoto.md)|Foto da equipe.|
|[primaryChannel](../api/team-get-primarychannel.md)|[channel](channel.md)| O canal geral da equipe. |
|Cronograma|[Cronograma](schedule.md)| Cronograma de turno para essa equipe.|
|template|[teamsTemplate](teamstemplate.md)| O modelo a partir do qual essa equipe foi criada. Consulte [modelos disponíveis](/MicrosoftTeams/get-started-with-teams-templates). |
|permissionGrants|Coleção [resourceSpecificPermissionGrant](resourcespecificpermissiongrant.md)| Uma coleção de permissões concedidas a aplicativos para acessar a equipe.|
|tags|Coleção [teamworkTag](../resources/teamworktag.md)|Os rótulos associados com a equipe.|

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
  "createdDateTime": "dateTimeOffset",
  "summary":  {"@odata.type": "microsoft.graph.teamSummary"}
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


