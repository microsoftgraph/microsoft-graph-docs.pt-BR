# <a name="section-resource-type"></a>Tipo de recurso section

Uma seção em um bloco de anotações do OneNote. As seções podem conter páginas.

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "pages",
    "parentNotebook",
    "parentSectionGroup"
  ],
  "@odata.type": "microsoft.graph.onenoteSection"
}-->

```json
{
  "createdBy": {"@odata.type": "microsoft.graph.identitySet"},
  "createdDateTime": "String (timestamp)",
  "id": "string (identifier)",
  "isDefault": true,
  "lastModifiedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "lastModifiedDateTime": "String (timestamp)",
  "links": {"@odata.type": "microsoft.graph.sectionLinks"},
  "displayName": "string",
  "pagesUrl": "string",
  "self": "string"
}

```
## <a name="properties"></a>Propriedades
| Propriedade       | Tipo    |Descrição|
|:---------------|:--------|:----------|
|createdBy|[identitySet](identityset.md)|Identidade do usuário, dispositivo e aplicativo que criou o item. Somente leitura.|
|createdDateTime|DateTimeOffset|A data e hora da criação da seção. O carimbo de data/hora representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`. Somente leitura.|
|id|String|O identificador exclusivo da seção.  Somente leitura.|
|isDefault|Booliano|Indica se esta é a seção padrão do usuário. Somente leitura.|
|lastModifiedBy|[identitySet](identityset.md)|Identidade do usuário, dispositivo e aplicativo que criou o item. Somente leitura.|
|lastModifiedDateTime|DateTimeOffset|A data e hora da última modificação da seção. O carimbo de data/hora representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`. Somente leitura.|
|links|[SectionLinks](sectionlinks.md)|Links para abrir a seção. O link `oneNoteClientURL` abre a seção no cliente nativo do OneNote se ele estiver instalado. O link `oneNoteWebURL` abre a seção no OneNote Online.|
|displayName|String|O nome da seção. |
|pagesUrl|String|O ponto de extremidade `pages` onde você pode obter detalhes de todas as páginas na seção. Somente leitura.|
|self|String|O ponto de extremidade onde você pode obter detalhes sobre a seção. Somente leitura.|

## <a name="relationships"></a>Relacionamento
| Relação | Tipo    |Descrição|
|:---------------|:--------|:----------|
|páginas|Coleção [Page](page.md)|Obtém o conjunto de páginas da seção.  Somente leitura. Anulável.|
|parentNotebook|[Notebook](notebook.md)|O bloco de anotações que contém a seção.  Somente leitura.|
|parentSectionGroup|[SectionGroup](sectiongroup.md)|O grupo de seção que contém a seção.  Somente leitura.|

## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Get section](../api/section_get.md) | [Section](section.md) |Leia as propriedades e as relações da seção.|
|[Criar página](../api/section_post_pages.md) |[Página](page.md)| Crie uma página postando na coleção pages do grupo de seção especificado.|
|[Listar páginas](../api/section_list_pages.md) |Coleção [Page](page.md)| Obtém uma coleção de páginas na seção especificada.|
|[copyToNotebook](../api/section_copytonotebook.md)|None|Copia a seção para um bloco de anotações específico.|
|[copyToSectionGroup](../api/section_copytosectiongroup.md)|None|Copia uma seção para um grupo de seção específico.|


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "onenoteSection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
