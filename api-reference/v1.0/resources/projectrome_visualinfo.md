# <a name="visualinfo-resource-type"></a>tipo de recurso visualInfo

Um tipo complexo para representar a propriedade **visualElements** no objeto [activity](../resources/projectrome_activity.md).

Cada atividade do usuário será exibida na linha do tempo como um Cartão Adaptável. Desenvolvedores de aplicativos são incentivados a fornecer um Cartão personalizado que captura a essência da atividade que foi realizada no seu aplicativo. É possível fazer isso fornecendo um cartão JSON personalizado na propriedade content.

Além de metadados visuais, com um Cartão Adaptável, o aplicativo pode especificar metadados de conteúdo – dados a serem usados para construir inferências sobre a atividade do usuário a fim de oferecer novas atividades para engajamento futuro. Isso é possível usando a propriedade contentInfo da atividade para fornecer um objeto JSON que aproveita as propriedades de schema.org para descrever o conteúdo.

Se não for fornecido um cartão personalizado, será gerado um cartão simples usando as propriedades displayText e description. Cartões personalizados são recomendados para demonstrar o melhor conteúdo do seu aplicativo.

## <a name="properties"></a>Propriedades

|Nome | Tipo | Descrição|
|:----|:------|:-----------|
|displayText | Cadeia de caracteres | Obrigatório. Uma breve descrição em texto sobre a atividade exclusiva do usuário (por exemplo, nome do documento em casos onde uma atividade refere-se à criação de documentos)|
|descrição | Cadeia de caracteres | Opcional. Descrição de texto mais longa da atividade exclusiva do usuário (exemplo: nome, primeira frase e/ou metadados de documentos)|
|backgroundColor | Cadeia de caracteres | Opcional. Cor do plano de fundo usada para processar a atividade na interface do usuário - cor de marca para a fonte da atividade do aplicativo. Deve ser uma cor hexadecimal válida|
|content | Objeto JSON não tipado | Opcional. Parte personalizada de dados - objeto JSON usado para fornecer conteúdo personalizado para renderizar a atividade na interface de usuário do Shell do Windows|
|attribution | [imageInfo](../resources/projectrome_imageinfo.md) | Opcional. Objeto JSON usado para representar um ícone que representa o aplicativo usado para gerar a atividade|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "attribution",
    "description",
    "backgroundColor",
    "content"
  ],
  "@odata.type": "microsoft.graph.visualInfo"
}-->

```json
{
    "@odata.type": "microsoft.graph.visualInfo",
    "attribution": {
        "@odata.type": "microsoft.graph.imageInfo",
        "iconUrl": "String (URL)",
        "alternateText": "String",
        "addImageQuery": "boolean"
    },
    "description": "String",
    "backgroundColor": "String",
    "displayText": "String",
    "content": {
        "@odata.type": "microsoft.graph.Json"
    }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-07 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "visualinfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
