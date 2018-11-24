# <a name="team-resource-type"></a>tipo de recurso de equipe



Uma equipe Teams da Microsoft é uma coleção de [canais](channel.md). Um canal representa um tópico e, portanto, um isolamento lógico discussão, dentro de uma equipe.

Cada equipe é associado um [grupo](../resources/group.md).
O grupo tem a mesma identificação que a equipe - por exemplo, /groups/ {id} / equipe é igual ao /teams/ {id}.
Para obter mais informações sobre como trabalhar com grupos e membros de equipes, consulte [Use a API do Microsoft Graph REST para trabalhar com as equipes da Microsoft](teams_api_overview.md).

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno  |Descrição|
|:---------------|:--------|:----------|
|[Criar equipe](../api/team_put_teams.md) | [equipe](team.md) | Criar um novo equipe ou adicione uma equipe a um grupo existente.|
|[Obtenha a equipe](../api/team_get.md) | [equipe](team.md) | Recupere as propriedades e relacionamentos da equipe especificado.|
|[Equipe de atualização](../api/team_update.md) | [equipe](team.md) |Atualize as propriedades da equipe especificado. |
|[Excluir equipe](../../v1.0/api/group_delete.md) | Nenhum |Exclua a equipe e seu grupo associado. |
|[Equipe de clone](../api/team_clone.md) | [teamsAsyncOperation](../resources/teamsasyncoperation.md) |Copie a equipe e seu grupo associado. |
|[Equipe de arquivo morto](../api/team_archive.md) | [teamsAsyncOperation](../resources/teamsasyncoperation.md) |Colocar a equipe em um estado somente leitura. |
|[Equipe de unarchive](../api/team_unarchive.md) | [teamsAsyncOperation](../resources/teamsasyncoperation.md) |Restaure a equipe em um estado de leitura / gravação. |
|[Listar suas equipes](../api/user_list_joinedteams.md) | coleção de [equipe](team.md) | Liste as equipes que você é um membro de. |
|[Liste todas as equipes](../../../concepts/teams_list_all_teams.md) | Coleção [group](group.md) | Liste todos os grupos que possuem equipes. |
|[Publicar aplicativos à sua organização](../resources/teamsapp.md)| [teamsApp](../resources/teamsapp.md) | Crie aplicativos de equipes visível somente para sua organização. |
|[Adicionar o aplicativo à equipe](../api/teamsappinstallation_add.md) | [teamsappinstallation](teamsappinstallation.md) | Adiciona (instala) um aplicativo para uma equipe.|
|[Adicionar guia ao canal](../api/teamstab_add.md) | [teamsTab](../resources/teamstab.md) | Adiciona (instala) uma guia ao canal da equipe.|

## <a name="properties"></a>Propriedades

| Propriedade | Tipo   | Descrição |
|:---------------|:--------|:----------|
|funSettings|[teamFunSettings](teamfunsettings.md) |Configurações para configurar o uso de Giphy, memes e adesivos na equipe de.|
|guestSettings|[teamGuestSettings](teamguestsettings.md) |Configurações para configurar se os convidados podem criar, atualizar ou excluir canais na equipe de.|
|isArchived|Booliano|Se essa equipe está em modo somente leitura. |
|memberSettings|[teamMemberSettings](teammembersettings.md) |Configurações para configurar se os membros podem realizar determinadas ações, por exemplo, criam canais e adicionar bots, na equipe de.|
|messagingSettings|[teamMessagingSettings](teammessagingsettings.md) |Configurações para configurar mensagens e menções na equipe de.|
|webUrl|cadeia de caracteres (somente leitura) | Um hiperlink que irão para a equipe no cliente do Microsoft Teams. Esta é a URL que você obtém quando você uma equipe no cliente do Microsoft Teams do mouse em e selecione o **link para a equipe de obter**. Essa URL deve ser tratado como um blob opaco e não analisado. |

## <a name="relationships"></a>Relações

| Relação | Tipo   | Descrição |
|:---------------|:--------|:----------|
|canais|coleção de [canal](channel.md)|A coleção de canais & associadas à equipe de mensagens.|
|installedApps|coleção [teamsAppInstallation](teamsappinstallation.md)|Os aplicativos instalados nesse conjunto.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

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
  "isArchived": false,
  "webUrl": "https://...longUrl..."
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
- [Criando um grupo com uma equipe](../../../concepts/teams-create-group-and-team.md)
- [Usando as APIs de equipes](teams_api_overview.md)
