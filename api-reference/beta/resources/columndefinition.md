---
author: JeremyKelley
description: Representa uma coluna em um site, uma lista ou um contentType.
ms.date: 09/11/2017
title: ColumnDefinition
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: sites-and-lists
ms.openlocfilehash: 650b7b9380576762d363c0c764a60d014e8f86b6
ms.sourcegitcommit: e5d5095e26dca6f434354a0970e789e94ee6afb0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/22/2022
ms.locfileid: "63722761"
---
# <a name="columndefinition-resource-type"></a>Tipo de recurso columnDefinition

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma coluna em [um site][], [lista][] ou [contentType][].

## <a name="methods"></a>Methods

| Método                                                                           | Tipo de retorno                                                     | Descrição                                                                                                                                           |
| :------------------------------------------------------------------------------- | :-------------------------------------------------------------- | :---------------------------------------------------------------------------------------------------------------------------------------------------- |
| [Listar colunas em um site](../api/site-list-columns.md)                            | [coleção columnDefinition](../resources/columndefinition.md) | Obter uma lista dos [objetos columnDefinition](../resources/columndefinition.md) e suas propriedades em um [site](../resources/site.md).                |
| [Listar colunas em uma lista](../api/list-list-columns.md)                            | [coleção columnDefinition](../resources/columndefinition.md) | Obter uma lista dos [objetos columnDefinition](../resources/columndefinition.md) e suas propriedades em uma [lista](../resources/list.md).                |
| [Listar colunas em um tipo de conteúdo](../api/contenttype-list-columns.md)             | [coleção columnDefinition](../resources/columndefinition.md) | Obter uma lista dos [objetos columnDefinition](../resources/columndefinition.md) e suas propriedades em um [tipo de conteúdo](../resources/contenttype.md). |
| [Criar columnDefinition para um site](../api/site-post-columns.md)                | [columnDefinition](../resources/columndefinition.md)            | Crie um novo [objeto columnDefinition](../resources/columndefinition.md) em um [site](../resources/site.md).                                           |
| [Criar columnDefinition para uma lista](../api/list-post-columns.md)                | [columnDefinition](../resources/columndefinition.md)            | Crie um novo [objeto columnDefinition](../resources/columndefinition.md) em uma [lista](../resources/list.md).                                           |
| [Criar columnDefinition para um tipo de conteúdo](../api/contenttype-post-columns.md) | [columnDefinition](../resources/columndefinition.md)            | Crie um novo [objeto columnDefinition](../resources/columndefinition.md) em um [tipo de conteúdo](../resources/contenttype.md).                            |
| [Obter columnDefinition](../api/columndefinition-get.md)                           | [columnDefinition](../resources/columndefinition.md)            | Leia as propriedades e as relações de um [objeto columnDefinition](../resources/columndefinition.md) .                                               |
| [Atualizar columnDefinition](../api/columndefinition-update.md)                     | [columnDefinition](../resources/columndefinition.md)            | Atualize as propriedades de um [objeto columnDefinition](../resources/columndefinition.md) .                                                               |
| [Excluir columnDefinition](../api/columndefinition-delete.md)                     | Nenhum                                                            | Exclui um [objeto columnDefinition](../resources/columndefinition.md) .                                                                                |

## <a name="properties"></a>Propriedades

As colunas podem conter dados de vários tipos.
As propriedades a seguir indicam qual tipo de dados uma coluna armazena, bem como configurações adicionais para esses dados.
As propriedades relacionadas ao tipo (boolean, calculated, choice, currency, dateTime, lookup, number, personOrGroup, text) são mutuamente exclusivas. Uma coluna só pode ter uma delas especificada.

| Propriedade                  | Tipo                            | Descrição                                                                                                                         |
| :------------------------ | :------------------------------ | :---------------------------------------------------------------------------------------------------------------------------------- |
| **columnGroup**           | string                          | Para colunas de site, o nome do grupo ao qual esta coluna pertence. Ajuda a organizar as colunas relacionadas.                                     |
| **description**           | string                          | A descrição voltado para o usuário da coluna.                                                                                          |
| **displayName**           | string                          | O nome voltado para o usuário da coluna.                                                                                                 |
| **enforceUniqueValues**   | Booliano                         | If `true`, no two list items may have the same value for this column.                                                               |
| **hidden**                | Booliano                         | Especifica se a coluna é exibida na interface do usuário.                                                                    |
| **id**                    | string                          | O identificador exclusivo da coluna.                                                                                               |
| **indexed**               | Booliano                         | Especifica se os valores da coluna podem ser usados para classificação e pesquisa.                                                             |
| **name**                  | string                          | O nome voltado para a API da coluna, conforme ele aparece nos [campos][] em uma [listItem][]. Para o nome voltado ao usuário, consulte **displayName**. |
| **readOnly**              | Booliano                         | Especifica se os valores da coluna podem ser modificados.                                                                                |
| **required**              | Boolean                         | Especifica se o valor da coluna não é opcional.                                                                                  |
| **boolean**               | [booleanColumn][]               | Esta coluna armazena valores boolianos.                                                                                                  |
| **calculated**            | [calculatedColumn][]            | Os dados dessa coluna são calculados com base em outras colunas.                                                                            |
| **choice**                | [choiceColumn][]                | Esta coluna armazena dados de uma lista de opções.                                                                                     |
| **currency**              | [currencyColumn][]              | Esta coluna armazena valores monetários.                                                                                                 |
| **dateTime**              | [dateTimeColumn][]              | Esta coluna armazena valores de datetime.                                                                                                 |
| **defaultValue**          | [defaultColumnValue][]          | O valor padrão dessa coluna.                                                                                                  |
| **geolocalização**           | [geolocationColumn][]           | Esta coluna armazena uma localização geográfica.                                                                                                   |
| **lookup**                | [lookupColumn][]                | Os dados dessa coluna são procurados por outra fonte no site.                                                                    |
| **number**                | [numberColumn][]                | Esta coluna armazena valores numéricos.                                                                                                   |
| **personOrGroup**         | [personOrGroupColumn][]         | Esta coluna armazena valores de Pessoa ou Grupo.                                                                                          |
| **text**                  | [textColumn][]                  | Esta coluna armazena valores de texto.                                                                                                     |
| **isDeletable**           | Booliano                         | Indica se essa coluna pode ser excluída.                                                                                       |
| **propagateChanges**      | Booliano                         | Se `true`, as alterações nesta coluna serão propagadas para listas que implementam a coluna.                                            |
| **isReorderable**         | Booliano                         | Indica se os valores na coluna podem ser reordenados. Somente leitura.                                                                 |
| **isSealed**              | Booliano                         | Especifica se a coluna pode ser alterada.                                                                                        |
| **validation**            | [columnValidation][]            | Esta coluna armazena a fórmula e a mensagem de validação da coluna.                                                                   |
| **hyperlinkOrPicture**    | [hyperlinkOrPictureColumn][]    | Esta coluna armazena valores de hiperlink ou imagem.                                                                                     |
| **term**                  | [termColumn][]                  | Esta coluna armazena termos de taxonomia.                                                                                                  |
| **sourceContentType**     | [contentTypeInfo][]             | ContentType do qual esta coluna é herdada. Usado apenas para buscar colunas contentTypes.                                      |
| **thumbnail**             | [thumbnailColumn][]             | Esta coluna armazena valores de miniatura.                                                                                                |
| **tipo**                  | columnTypes                     | Para colunas de site, o tipo de coluna. Somente leitura.                                                                                    |
| **contentApprovalStatus** | [contentApprovalStatusColumn][] | Esta coluna armazena o status de aprovação de conteúdo.                                                                                         |

## <a name="relationships"></a>Relações

| Relação     | Tipo                 | Descrição                                |
| :--------------- | :------------------- | :----------------------------------------- |
| **sourceColumn** | [columnDefinition][] | A coluna de origem para a coluna de tipo de conteúdo. |

>**Observação:** Essas propriedades correspondem à enumeração SharePoint [SPFieldType][].
Observe que os tipos de campo mais comuns são representados na tabela anterior. No entanto, essa API beta ainda está faltando algumas.
nestes casos, nenhuma das facetas do tipo de coluna serão preenchidas, e a coluna só terá as propriedades básicas.

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
