# <a name="teamsappinstallation-resource-type"></a>tipo de recurso de teamsAppInstallation



Um [teamsApp](teamsapp.md) instalado em uma [equipe](team.md). Qualquer bots que fazem parte do aplicativo se tornará parte de qualquer aplicativo é adicionado de equipe.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno  |Descrição|
|:---------------|:--------|:----------|
|[Lista de aplicativos](../api/teamsappinstallation_list.md) | [teamsAppInstallation](teamsapp.md) | Lista os aplicativos instalados em uma equipe.|
|[Adicionar aplicativo](../api/teamsappinstallation_add.md) | [teamsAppInstallation](teamsapp.md) | Adiciona (instala) um aplicativo para uma equipe.|
|[Remover aplicativo](../api/teamsappinstallation_delete.md) | Nenhum | Remove (desinstala) um aplicativo da equipe.|
|[Atualizar o aplicativo](../api/teamsappinstallation_delete.md) | Nenhum | Atualizações para a versão mais recente do aplicativo.|

## <a name="properties"></a>Propriedades

| Propriedade            | Tipo     | Descrição |
|:------------------- |:-------- |:----------- |
| id                  | string   | Uma identificação exclusiva (não o appid equipes). |

## <a name="relationships"></a>Relações

| Relação   | Tipo    | Descrição |
|:---------------|:--------|:----------|
|teamsApp|[teamsApp](teamsapp.md)| O aplicativo que está instalado. |
|teamsAppDefinition|[teamsAppDefinition](teamsapp.md)| Os detalhes desta versão do aplicativo. |

## <a name="json-representation"></a>Representação JSON

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsAppInstallation",
  "baseType": "microsoft.graph.entity"
}-->

```json
{
  "id": "string",
}
```

# <a name="see-also"></a>Confira também

- [teamsApp](teamsapp.md)
- [teamsAppDefinition](teamsappdefinition.md)
- [teamsTab](../resources/teamstab.md)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "teamsApp resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

