# <a name="onenote-resource-type"></a>tipo de recurso do onenote

O ponto de entrada para os recursos do OneNote.

Todas as chamadas para o serviço do OneNote pela API do Microsoft Graph usam essa URL raiz de serviço:

```
https://graph.microsoft.com/{version}/{location}/onenote/ 
```

A localização pode ser blocos de anotações do usuário no Office 365 ou OneDrive do consumidor, blocos de anotações de grupo ou blocos de anotações hospedado no site de equipe do SharePoint no Office 365. 

**Blocos de anotações do usuário** Para acessar blocos de anotações pessoais no OneDrive do consumidor ou no OneDrive for Business, use uma das seguintes URLs:

```
https://graph.microsoft.com/{version}/me/onenote/{notebooks | sections | sectionGroups | pages} 
https://graph.microsoft.com/{version}/users/{userPrincipalName}/onenote/{notebooks | sections | sectionGroups | pages} 
https://graph.microsoft.com/{version}/users/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```

**Blocos de anotações de grupo** para acessar blocos de anotações que pertencem a um grupo, use a seguinte URL raiz de serviço:

```
https://graph.microsoft.com/{version}/groups/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```
**Blocos de anotações do site do SharePoint** para acessar blocos de anotações que pertencem a um site de equipe do SharePoint, use a seguinte URL raiz de serviço:

```
https://graph.microsoft.com/{version}/sites/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```
## <a name="authorization"></a>Autorização

Para obter informações sobre as permissões necessárias para trabalhar com o APIs do OneNote, confira [Permissões de anotações](../../../concepts/permissions_reference.md#notes-permissions).


## <a name="relationships"></a>Relações
| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
|notebooks|Coleção [Notebook](notebook.md)|A coleção de blocos de anotações do OneNote que pertencem ao usuário ou ao grupo. Somente leitura. Anulável.|
|operations|Coleção [Operation](onenoteoperation.md) |O status das operações do OneNote. Não há suporte para a obtenção de uma coleção de operações, mas você pode obter o status das operações longas se o cabeçalho `Operation-Location` for retornado na resposta. Somente leitura. Anulável.|
|páginas|Coleção [Page](page.md)|As páginas em todos os blocos de anotações do OneNote que pertencem ao usuário ou ao grupo.  Somente leitura. Anulável.|
|recursos|Coleção [Resource](resource.md) |A imagem e outros recursos de arquivos nas páginas do OneNote. Não há suporte para a obtenção de uma coleção de recursos, mas você pode [obter o conteúdo de um recurso binário específico](resource.md). Somente leitura. Anulável.|
|sectionGroups|Coleção [SectionGroup](sectiongroup.md)|Os grupos de seção em todos os blocos de anotações do OneNote que pertencem ao usuário ou ao grupo.  Somente leitura. Anulável.|
|seções|Coleção [Section](section.md)|As seções em todos os blocos de anotações do OneNote que pertencem ao usuário ou ao grupo.  Somente leitura. Anulável.|

## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Create notebook](../api/onenote_post_notebooks.md) |[Notebook](notebook.md)| Crie um bloco de anotações postando na coleção notebooks.|
|[List notebooks](../api/onenote_list_notebooks.md) |Coleção [Notebook](notebook.md)| Obter uma coleção de blocos de anotações.|
|[Create page](../api/onenote_post_pages.md) |[Page](page.md)| Crie uma página postando na coleção pages.|
|[List pages](../api/onenote_list_pages.md) |Coleção [Page](page.md)| Obter uma coleção de páginas.|
|[List section groups](../api/onenote_list_sectiongroups.md) |Coleção [SectionGroup](sectiongroup.md)| Obter uma coleção de grupos de seção.|
|[List sections](../api/onenote_list_sections.md) |Coleção [Section](section.md)| Obter uma coleção de seções.|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "onenote resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
