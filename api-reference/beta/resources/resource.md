# <a name="resource-resource-type"></a>Tipo de recurso resource

Uma imagem ou outro recurso de arquivo em uma página do OneNote. 

É possível obter os dados binários de um recurso, mas não há suporte para obter uma representação JSON de um objeto de recurso ou uma coleção de recursos.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onenoteResource"
}-->

Obtenha os dados binários de um recurso específico enviando uma solicitação GET para o ponto de extremidade `content` do recurso:

```
GET ../onenote/resources/{id}/content
```

O URI de recurso do arquivo é retornado quando você recebe um conteúdo HTML da página usando a seguinte solicitação:

```
GET ../onenote/pages/{id}/content
```

Na página HTML, uma marca `img` inclui os pontos de extremidade do recurso de imagem original no atributo `data-fullres-src` e a imagem otimizada no atributo `src`:
```
<img 
    src="image-resource-url"  
    data-src-type="media-type"
    data-fullres-src="image-resource-url"  
    data-fullres-src-type="media-type" ... />
```

Uma marca `object` (que representa arquivos como PDF, DOCX e PNG) inclui o ponto de extremidade para o recurso do arquivo no atributo `data`:

```
<object
    data="file-resource-url"
    data-attachment="file-name.file-type" 
    type="media-type" ... />
```

## <a name="properties"></a>Propriedades
Nenhum.

## <a name="relationships"></a>Relações
Nenhum


## <a name="methods"></a>Métodos
| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Get resource binary data](../api/resource_get.md) | Fluxo |Recupere os dados binários de um recurso de arquivo ou imagem.|


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "resource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->