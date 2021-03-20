---
author: JeremyKelley
description: Aqui está uma representação JSON de um recurso columnDefinition.
ms.date: 09/11/2017
title: ColumnDefinition
localization_priority: Normal
doc_type: resourcePageType
ms.prod: sites-and-lists
ms.openlocfilehash: cddab6ee01cea34902ee892e593e0e81b3cde8af
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50961297"
---
# <a name="columndefinition-resource-type"></a>Tipo de recurso columnDefinition

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma coluna em um [site,][] [lista][] ou [contentType][].

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar colunas em um site](../api/site-list-columns.md)|[coleção columnDefinition](../resources/columndefinition.md)|Obter uma lista dos [objetos columnDefinition](../resources/columndefinition.md) e suas propriedades em um [site](../resources/site.md).|
|[Listar colunas em uma lista](../api/list-list-columns.md)|[coleção columnDefinition](../resources/columndefinition.md)|Obter uma lista dos [objetos columnDefinition](../resources/columndefinition.md) e suas propriedades em uma [lista](../resources/list.md).|
|[Listar colunas em um tipo de conteúdo](../api/contenttype-list-columns.md)|[coleção columnDefinition](../resources/columndefinition.md)|Obter uma lista dos [objetos columnDefinition](../resources/columndefinition.md) e suas propriedades em um [tipo de conteúdo](../resources/contenttype.md).|
|[Criar columnDefinition para um site](../api/site-post-columns.md)|[columnDefinition](../resources/columndefinition.md)|Criar um novo [objeto columnDefinition](../resources/columndefinition.md) em um [site](../resources/site.md).|
|[Criar columnDefinition para uma lista](../api/list-post-columns.md)|[columnDefinition](../resources/columndefinition.md)|Criar um novo [objeto columnDefinition](../resources/columndefinition.md) em uma [lista](../resources/list.md).|
|[Criar columnDefinition para um tipo de conteúdo](../api/contenttype-post-columns.md)|[columnDefinition](../resources/columndefinition.md)|Criar um novo [objeto columnDefinition](../resources/columndefinition.md) em um [tipo de conteúdo](../resources/contenttype.md).|
|[Obter columnDefinition](../api/columndefinition-get.md)|[columnDefinition](../resources/columndefinition.md)|Leia as propriedades e as relações de um [objeto columnDefinition.](../resources/columndefinition.md)|
|[Atualizar columnDefinition](../api/columndefinition-update.md)|[columnDefinition](../resources/columndefinition.md)|Atualize as propriedades de um [objeto columnDefinition.](../resources/columndefinition.md)|
|[Excluir columnDefinition](../api/columndefinition-delete.md)|Nenhum|Exclui um [objeto columnDefinition.](../resources/columndefinition.md)|

## <a name="json-representation"></a>Representação JSON

Aqui está uma representação JSON de um recurso columnDefinition.

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.columnDefinition"
}-->

```json
{
  "columnGroup": "string",
  "description": "description",
  "displayName": "friendly name",
  "enforceUniqueValues": true,
  "hidden": false,
  "id": "string",
  "indexed": true,
  "name": "staticNameForApi",
  "readOnly": false,
  "required": false,
  "boolean": { "@odata.type": "microsoft.graph.booleanColumn" },
  "calculated": { "@odata.type": "microsoft.graph.calculatedColumn" },
  "choice": { "@odata.type": "microsoft.graph.choiceColumn" },
  "currency": { "@odata.type": "microsoft.graph.currencyColumn" },
  "dateTime": { "@odata.type": "microsoft.graph.dateTimeColumn" },
  "defaultValue": { "@odata.type": "microsoft.graph.defaultColumnValue" },
  "geolocation": { "@odata.type": "microsoft.graph.geolocationColumn" },
  "lookup": { "@odata.type": "microsoft.graph.lookupColumn" },
  "number": { "@odata.type": "microsoft.graph.numberColumn" },
  "personOrGroup": { "@odata.type": "microsoft.graph.personOrGroupColumn" },
  "text": { "@odata.type": "microsoft.graph.textColumn" },
  "isDeletable" : false,
  "propagateChanges": false,
  "isReorderable": false,
  "isSealed": false,
  "validation": { "@odata.type": "microsoft.graph.columnValidation" },
  "hyperlinkOrPicture": { "@odata.type": "microsoft.graph.hyperlinkOrPictureColumn" },
  "term": { "@odata.type": "microsoft.graph.termColumn" },
  "sourceContentType": { "@odata.type": "microsoft.graph.contentTypeInfo" },
  "thumbnail": { "@odata.type": "microsoft.graph.thumbnailColumn" },
  "type": { "@odata.type": "microsoft.graph.columnTypes" },
  "contentApprovalStatus": { "@odata.type": "microsoft.graph.contentApprovalStatusColumn" }
}
```

## <a name="properties"></a>Propriedades

As colunas podem conter dados de vários tipos.
As propriedades a seguir indicam qual tipo de dados uma coluna armazena, bem como configurações adicionais para esses dados.
As propriedades relacionadas ao tipo (boolean, calculated, choice, currency, dateTime, lookup, number, personOrGroup, text) são mutuamente exclusivas. Uma coluna só pode ter uma delas especificada.

| Nome da propriedade           | Tipo    | Descrição
|:------------------------|:--------|:-----------------------------------------
| **columnGroup**         | string  | Para colunas de site, o nome do grupo ao qual esta coluna pertence. Ajuda a organizar as colunas relacionadas.
| **description**         | string  | A descrição voltado para o usuário da coluna.
| **displayName**         | cadeia de caracteres  | O nome voltado para o usuário da coluna.
| **enforceUniqueValues** | Booliano | Se for verdadeiro, esse mesmo valor não constará em dois itens de lista nessa coluna.
| **hidden**              | Booliano | Especifica se a coluna é exibida na interface do usuário.
| **id**                  | cadeia de caracteres  | O identificador exclusivo da coluna.
| **indexed**             | Booliano | Especifica se os valores da coluna podem ser usados para classificação e pesquisa.
| **name**                | string  | O nome voltado para a API da coluna, conforme ele aparece nos [campos][] em uma [listItem][]. Para o nome voltado ao usuário, consulte **displayName**.
| **readOnly**            | Booliano    | Especifica se os valores da coluna podem ser modificados.
| **required**            | Booliano | Especifica se o valor da coluna não é opcional.
| **boolean**       | [booleanColumn][]       | Esta coluna armazena valores boolianos.
| **calculated**    | [calculatedColumn][]    | Os dados dessa coluna são calculados com base em outras colunas.
| **choice**        | [choiceColumn][]        | Esta coluna armazena dados de uma lista de opções.
| **currency**      | [currencyColumn][]      | Esta coluna armazena valores monetários.
| **dateTime**      | [dateTimeColumn][]      | Esta coluna armazena valores de datetime.
| **defaultValue**  | [defaultColumnValue][]  | O valor padrão dessa coluna.
| **geolocalização**   | [geolocationColumn][]   | Esta coluna armazena uma localização geográfica.
| **lookup**        | [lookupColumn][]        | Os dados dessa coluna são procurados por outra fonte no site.
| **number**        | [numberColumn][]        | Esta coluna armazena valores numéricos.
| **personOrGroup** | [personOrGroupColumn][] | Esta coluna armazena valores de Pessoa ou Grupo.
| **text**          | [textColumn][]          | Esta coluna armazena valores de texto.
| **isDeletable**       | Booliano | Indica se essa coluna pode ser excluída.
| **propagateChanges**     | Booliano | Se as alterações 'True' nesta coluna serão propagadas para listas que implementam a coluna. 
| **isReorderable**         | Booliano | Indica se os valores na coluna podem ser reordenados. Somente leitura.
| **isSealed**              | Booliano | Especifica se a coluna pode ser alterada.
| **validation**   |  [columnValidation][]    | Esta coluna armazena a fórmula e a mensagem de validação da coluna. 
| **hyperlinkOrPicture**  | [hyperlinkOrPictureColumn][] | Esta coluna armazena valores de hiperlink ou imagem. 
| **term**     | [termColumn][] | Esta coluna armazena termos de taxonomia.
| **sourceContentType**   |[contentTypeInfo][]  | ContentType do qual esta coluna é herdada. Usado apenas ao buscar colunas contentTypes.
| **thumbnail**           |[thumbnailColumn][]      | Esta coluna armazena valores de miniatura.
| **type**         | columnTypes  | Para colunas de site, o tipo de coluna. Somente leitura
| **contentApprovalStatus**| [contentApprovalStatusColumn][]     | Esta coluna armazena o status de aprovação de conteúdo.

## <a name="relationships"></a>Relações

| Nome da propriedade   | Tipo                      | Descrição
|:----------------|:--------------------------|:-------------------------------
| **sourceColumn** | [columnDefinition][] | A coluna de origem para a coluna de tipo de conteúdo.

>**Observação:** Essas propriedades correspondem à enumeração [SPFieldType][] do SharePoint.
Embora os tipos de campo mais comuns sejam representados na tabela anterior, essa API beta ainda não tem alguns.
nestes casos, nenhuma das facetas do tipo de coluna serão preenchidas, e a coluna só terá as propriedades básicas.

## <a name="remarks"></a>Comentários

Os valores ColumnDefinitions e valores de campo para colunas `hidden` não são mostrados por padrão.
Para vê-los ao listar **columnDefinitions**, inclua `hidden` na instrução `$select`.
Para vê-los ao exibir valores **field** em [listItems][listItem], inclua as colunas desejadas por nome na instrução `$select`.

[booleanColumn]: booleancolumn.md
[calculatedColumn]: calculatedcolumn.md
[choiceColumn]: choicecolumn.md
[columnDefinition]: columnDefinition.md
[contentType]: contenttype.md
[currencyColumn]: currencycolumn.md
[dateTimeColumn]: datetimecolumn.md
[defaultColumnValue]: defaultcolumnvalue.md
[geolocationColumn]: geolocationcolumn.md
[list]: list.md
[lookupColumn]: lookupcolumn.md
[numberColumn]: numbercolumn.md
[personOrGroupColumn]: personorgroupcolumn.md
[site]: site.md
[textColumn]: textcolumn.md
[fieldValueSet]: fieldvalueset.md
[campos]: fieldvalueset.md
[listItem]: listitem.md
[termColumn]: termColumn.md
[contentApprovalStatusColumn]: contentApprovalStatusColumn.md
[thumbnailColumn]: thumbnailColumn.md
[hyperlinkOrPictureColumn]: hyperlinkOrPictureColumn.md
[columnValidation]: columnValidation.md
[contentTypeInfo]: contentTypeInfo.md


  [SPFieldType]: /previous-versions/office/sharepoint-server/ms428806(v=office.15)

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ColumnDefinition",
  "suppressions": []
}
-->