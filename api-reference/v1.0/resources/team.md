---
title: tipo de recurso de equipe
description: 'No Microsoft Teams, uma equipe é um conjunto de canais. '
author: AkJo
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: e1326c63290b36a884d8d61ad5f9b820ab957aca
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/11/2020
ms.locfileid: "49659733"
---
# <a name="team-resource-type"></a>tipo de recurso de equipe

Namespace: microsoft.graph



No Microsoft Teams, uma equipe é um conjunto de objetos de [canal](channel.md).
Um canal representa um tópico e, portanto, um isolamento lógico da discussão em uma equipe.

Cada equipe está associada a um [grupo](../resources/group.md).
O grupo tem a mesma ID da equipe, por exemplo, /groups/{id}/team é igual a /teams/{id}.
Confira mais informações sobre como trabalhar com grupos e membros em equipes, confira [Usar a API REST do Microsoft Graph para trabalhar com o Microsoft Teams](teams-api-overview.md).

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno  |Descrição|
|:---------------|:--------|:----------|
|[Criar equipe](../api/team-post.md) | [teamsAsyncOperation](teamsasyncoperation.md) | Crie uma equipe do zero. |
|[Criar equipe a partir do grupo](../api/team-put-teams.md) | [team](team.md) | Crie uma nova equipe ou adicione uma equipe a um grupo existente.|
|[Obter equipe](../api/team-get.md) | [team](team.md) | Recupere as propriedades e relações da equipe especificada.|
|[Atualizar equipe](../api/team-update.md) | [team](team.md) |Atualize as propriedades da equipe especificada. |
|[Excluir equipe](../api/group-delete.md) | Nenhum |Exclua a equipe e o grupo associado. |
|[Listar membros](../api/team-list-members.md)|coleção [conversationMember](../resources/conversationmember.md)|Obtenha a lista de membros nessa equipe.|
|[Obter membro](../api/team-get-members.md) | [conversationMember](conversationmember.md)coleção | Obtenha um membro na equipe.|
|[Adicionar membro](../api/team-post-members.md)|[conversationMember](../resources/conversationmember.md)|Adicione um novo membro à equipe.|
|[Remover membro](../api/team-delete-members.md)|Nenhum|Remova um membro existente da equipe.|
|[Atualizar a função do membro](../api/team-update-members.md)|[conversationMember](../resources/conversationmember.md)|Alterar um membro para um proprietário ou voltar para um membro regular.|
|[Arquivar equipe](../api/team-archive.md) | [teamsAsyncOperation](../resources/teamsasyncoperation.md) |Coloque a equipe em um estado somente leitura. |
|[Desarquivar equipe](../api/team-unarchive.md) | [teamsAsyncOperation](../resources/teamsasyncoperation.md) |Restaure a equipe com um estado de leitura e gravação. |
|[Clonar equipe](../api/team-clone.md) | [teamsAsyncOperation](../resources/teamsasyncoperation.md) |Copie a equipe e o grupo associado. |
|[Listar suas equipes](../api/user-list-joinedteams.md) | Coleção [team](team.md) | Liste as equipes das quais você é membro. |
|[Listar aplicativos em equipe](../api/team-list-installedapps.md) | Coleção[teamsAppInstallation](teamsappinstallation.md) | Liste os aplicativos instalados em uma equipe.|
|[Instalar o aplicativo na equipe do](../api/team-get-installedapps.md) | [teamsAppInstallation](teamsappinstallation.md) | Obtenha o aplicativo especificado instalado em uma equipe.|
|[Adicionar aplicativo à equipe](../api/team-post-installedapps.md) |Nenhuma | Adicione (instale) um aplicativo a uma equipe.|
|[Atualizar o aplicativo instalado para a equipe](../api/team-teamsappinstallation-upgrade.md) | Nenhuma | Atualize o aplicativo instalado em uma equipe para a versão mais recente.|
|[Remover aplicativo da equipe](../api/team-delete-installedapps.md) | Nenhuma | Remova (desinstale) um aplicativo de uma equipe.|

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
|webUrl|cadeia de caracteres (somente leitura) | Um hiperlink que será enviado à equipe no cliente do Microsoft Teams. Esta é a URL que você recebe ao clicar com o botão direito do mouse em uma equipe no cliente do Microsoft Teams e escolher **Obter o link para a equipe**. Essa URL deve ser tratada como um blob opaco e não analisado. |

## <a name="relationships"></a>Relações

| Relação | Tipo | Descrição |
|:---------------|:--------|:----------|
|channels|Coleção [channel](channel.md)|A coleção de canais e mensagens associadas à equipe.|
|installedApps|Coleção [teamsAppInstallation](teamsappinstallation.md)|Os aplicativos instalados nessa equipe.|
|members|coleção [conversationMember](../resources/conversationmember.md)|Membros e proprietários da equipe.|
|operations|Coleção [teamsAsyncOperation](teamsasyncoperation.md)| As operações assíncronas que foram executadas ou estão em execução nesta equipe. | 
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
  "internalId": "string",
  "isArchived": false,
  "webUrl": "string (URL)",
  "classSettings": {"@odata.type": "microsoft.graph.teamClassSettings"}
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "team resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

## <a name="see-also"></a>Confira também

- [Usar o API do Microsoft Graph para trabalhar com o Microsoft Teams](teams-api-overview.md)
- [Como criar um grupo com uma equipe](/graph/teams-create-group-and-team)
- [Listar todas as equipes](/graph/teams-list-all-teams)

