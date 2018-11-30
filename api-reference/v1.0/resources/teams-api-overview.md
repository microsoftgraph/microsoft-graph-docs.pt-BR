---
title: Usar o Microsoft Graph API para trabalhar com o Microsoft Teams
description: Teams da Microsoft é um espaço de trabalho com base em bate-papo no Office 365 que fornece acesso interno aos calendários específicas para a equipe, arquivos, anotações do OneNote, planos de planejador e muito mais.
ms.openlocfilehash: b42c33a34e0191eae236f675f29762834dfc29da
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27005330"
---
# <a name="use-the-microsoft-graph-api-to-work-with-microsoft-teams"></a>Usar o Microsoft Graph API para trabalhar com o Microsoft Teams



Teams da Microsoft é um espaço de trabalho com base em bate-papo no Office 365 que fornece acesso interno aos calendários específicas para a equipe, arquivos, anotações do OneNote, planos de planejador e muito mais.

## <a name="key-resources-in-microsoft-teams"></a>Principais recursos no Microsoft Teams

| Recurso | Métodos |
|:---------------|:--------|
|[equipe](../resources/team.md)| [Listar suas equipes](../api/user-list-joinedteams.md), [lista todas as equipes](/graph/teams-list-all-teams), [criar](../api/team-put-teams.md), [ler](../api/team-get.md), [Atualizar](../api/team-update.md), [Excluir](/graph/api/group-delete?view=graph-rest-1.0), [clone](../api/team-clone.md), [arquivo morto](../api/team-archive.md), [unarchive](../api/team-unarchive.md) |
|[group](../resources/group.md)| [Adicionar membro](../api/group-post-members.md), [Remover membro](../api/group-delete-members.md), [Adicionar proprietário](../api/group-post-owners.md), [Remover proprietário](../api/group-delete-owners.md), [obter arquivos](drive.md), [fazer anotações](/graph/api/resources/notebook?view=graph-rest-1.0), [fazer planos](plannergroup.md), [Obtenha o calendário](event.md) |
|[canal](../resources/channel.md)|[lista](../api/channel-list.md), [criar](../api/channel-post.md), [ler](../api/channel-get.md), [Atualizar](../api/channel-patch.md), [Excluir](../api/channel-delete.md)|
|[teamsTab](../resources/teamstab.md) |[lista](../api/teamstab-list.md), [criar](../api/teamstab-add.md), [ler](../api/teamstab-get.md), [Atualizar](../api/teamstab-update.md), [Excluir](../api/teamstab-delete.md) |
|[teamsApp](../resources/teamsapp.md)|[lista](../api/teamsapp-list.md), [Publicar](../api/teamsapp-publish.md), [Atualizar](../api/teamsapp-update.md), [Remover](../api/teamsapp-delete.md)|
|[teamsAppInstallation](../resources/teamsappinstallation.md)| [lista](../api/teamsappinstallation-list.md), [instalar](../api/teamsappinstallation-add.md), [Atualizar](../api/teamsappinstallation-delete.md), [Remover](../api/teamsappinstallation-delete.md) |
| (Preview) [chatMessage](/graph/api/resources/chatmessage?view=graph-rest-beta) e [chatThread](/graph/api/resources/chatthread?view=graph-rest-beta) | [lista](/graph/api/channel-list-messages?view=graph-rest-beta), [criar](/graph/api/channel-post-chatthreads?view=graph-rest-beta), [ler](/graph/api/channel-get-message?view=graph-rest-beta) |
| (Preview) [chamada](/graph/api/resources/call?view=graph-rest-beta) | [resposta](/graph/api/call-answer?view=graph-rest-beta), [Rejeitar](/graph/api/call-reject?view=graph-rest-beta), [Redirecionar](/graph/api/call-redirect?view=graph-rest-beta), [Ativar Mudo](/graph/api/call-mute?view=graph-rest-beta), [desativar o mudo](/graph/api/call-unmute?view=graph-rest-beta), [atualizar os metadados](/graph/api/call-updatemetadata?view=graph-rest-beta), [alterar a função de compartilhamento de tela](/graph/api/call-changescreensharingrole?view=graph-rest-beta), [participantes de lista](/graph/api/call-list-participants?view=graph-rest-beta), [Convidar participantes](/graph/api/participant-invite?view=graph-rest-beta), [Ativar Mudo de todos os participantes](/graph/api/participant-muteall?view=graph-rest-beta) |

## <a name="teams-and-groups"></a>Equipes e grupos

No Microsoft Graph, Microsoft Teams é representada por um recurso de [grupo](../resources/group.md) . Grupos de Teams da Microsoft e o Office 365 abordar as necessidades de vários de colaboração de grupo. Quase todos os recursos baseados no grupo se aplicam ao Microsoft Teams e grupos do Office 365, como calendário de grupo, arquivos, observações, foto, planos e assim por diante. A principal diferença entre uma [equipe](team.md) e um grupo do Office 365 é o modo de comunicação entre membros. Os membros da equipe se comunicar por chat persistente no contexto de uma equipe específico. Membros do Office 365 grupo se comunicar por conversas do grupo, que são as conversas de email que ocorrem no contexto de um grupo no Outlook.

Qualquer grupo que tenha uma equipe tem uma propriedade **resourceProvisioningOptions** que contém "Equipe". 

>**Observação:** A propriedade **Group.resourceProvisioningOptions** pode ser alterada.
Não adicione ou remova "Equipe" dessa coleção; Caso contrário, você obterá resultados incorretos quando você lista todas as equipes.

A seguir estão as diferenças no nível de API entre equipes e grupos:

- O método [lista ingressou equipes](../api/user-list-joinedteams.md) só se aplica a Teams da Microsoft.
- Consulte também os [problemas conhecidos](/graph/known-issues) para essas APIs.

>**Observação:** Se você usar os API de grupos em um [aplicativo de equipes da Microsoft](https://docs.microsoft.com/en-us/microsoftteams/platform/#apps-in-microsoft-teams) em vez de um aplicativo autônomo - por exemplo, como parte de uma guia ou bot executando no Microsoft Teams - siga as orientações no artigo [Usando o Microsoft Graph em suas páginas de equipes da Microsoft](https://docs.microsoft.com/en-us/microsoftteams/platform/resources/microsoft-graph).

## <a name="membership-changes-in-microsoft-teams"></a>Alterações de associação no Microsoft Teams

Para adicionar membros e proprietários para uma equipe, alterar a associação do [grupo](../resources/group.md) com a mesma identificação.

| Caso de uso      | Verb      | URL |
| ------------------------------------- | ------------------------------------------------------------ | ------------------------------------------------------------ |
| [Adicionar membro](../api/group-post-members.md)    | POST      | ref de $/members/ /Groups/ {id}  |
| [Remover membro](../api/group-delete-members.md)   | DELETE    | /members/ /Groups/ {id} {userId} / $ref |
| [Adicionar proprietário](../api/group-post-owners.md)     | POST       | ref de $/owners/ /Groups/ {id} |
| [Remover proprietário](../api/group-delete-owners.md) | DELETE    | /owners/ /Groups/ {id} {userId} / $ref |
| [Equipe de atualização](../api/team-update.md)  | PATCH     | /Teams/ {id} |

Recomendamos que quando você adiciona um proprietário, você também adicionar esse usuário como um membro. Se uma equipe possui um proprietário que também não é um membro, alterações de propriedade e a associação talvez não mostrada imediatamente no Microsoft Teams. Além disso, diferentes aplicativos e APIs vai tratar de que forma diferente. Por exemplo, o Microsoft Teams mostrará equipes que o usuário é um membro ou um proprietário do, enquanto os cmdlets do PowerShell de equipes da Microsoft e joinedTeams/me/API serão exibidas apenas as equipes que o usuário é membro do. Para evitar confusão, adicione todos os proprietários à lista de membros. 

Problema conhecido: excluir quando /groups/ {id} / proprietários é chamado, o usuário também é removido do /groups/ {id} / lista de membros. Para contornar esse problema, recomendamos que você remova o usuário de proprietários e membros, e depois Aguarde 10 segundos e adicioná-los de volta aos membros.

Quando adicionando e removendo membros e proprietários, não coloque chaves {} ao redor a ID.

| Speed | Sintaxe | 
| ------ | ----- |
| Rápida | https://graph.microsoft.com/v1.0/groups/02bd9fd6-8f93-4758-87c3-1fb73740a315/members/48d31887-5fad-4d73-a9f5-3c356e68a038/$ref | 
| Lenta | https://graph.microsoft.com/v1.0/groups/{02bd9fd6-8f93-4758-87c3-1fb73740a315}/members/{48d31887-5fad-4d73-a9f5-3c356e68a038}/$ref | 

Da mesma forma, se o `userId` na URL ou carga é expresso como um UPN em vez de como um GUID, o desempenho será mais lento.

| Speed | Sintaxe | 
| ------ | ----- |
| Rápida | 48d31887-5fad-4d73-a9f5-3c356e68a038 | 
| Lenta | John@example.com | 

Quando o caminho mais lento é executado, se um membro da equipe atual ou proprietário do site da aplicativo Microsoft Teams tiver entrado no, a alteração será refletida dentro de uma hora.
Se nenhum desses usuários estiver conectado ao site/aplicativo Teams da Microsoft, a alteração não será refletida até uma hora após um deles entra no.

## <a name="see-also"></a>Confira também

- [Visão geral da API de equipes da Microsoft](/graph/teams-concept-overview)
- Código de exemplo: [Contoso Airlines](https://github.com/microsoftgraph/contoso-airlines-teams-sample), [miniamostras do c#](https://github.com/microsoftgraph/csharp-teams-sample-graph)
