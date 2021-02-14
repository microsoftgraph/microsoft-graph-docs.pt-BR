---
author: JeremyKelley
ms.date: 09/11/2017
title: ColumnDefinition
localization_priority: Normal
description: Aqui está uma representação JSON de um recurso ColumnDefinition.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 83f278123a8153629593c54604ce1285a48439a7
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/14/2021
ms.locfileid: "50239237"
---
# <a name="columndefinition-resource"></a>Recurso ColumnDefinition

Namespace: microsoft.graph

## <a name="json-representation"></a>Representação JSON

Aqui está uma representação JSON de um recurso ColumnDefinition.

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
  "enforceUniqueValues": "true",
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
  "text": { "@odata.type": "microsoft.graph.textColumn" }
}
```

## <a name="properties"></a>Propriedades

O recurso **columnDefinition** tem as seguintes propriedades.

| Nome da propriedade           | Tipo    | Descrição
|:------------------------|:--------|:-----------------------------------------
| **columnGroup**         | string  | Para colunas de site, o nome do grupo ao qual esta coluna pertence. Ajuda a organizar as colunas relacionadas.
| **description**         | string  | A descrição voltado para o usuário da coluna.
| **displayName**         | string  | O nome voltado para o usuário da coluna.
| **enforceUniqueValues** | booliano | Se for verdadeiro, esse mesmo valor não constará em dois itens de lista nessa coluna.
| **hidden**              | booliano | Especifica se a coluna é exibida na interface do usuário.
| **id**                  | string  | O identificador exclusivo da coluna.
| **indexed**             | booliano | Especifica se os valores da coluna podem ser usados para classificação e pesquisa.
| **name**                | string  | O nome voltado para a API da coluna, conforme ele aparece nos [campos][] em uma [listItem][]. Para o nome voltado ao usuário, consulte **displayName**.
| **readOnly**            | bool    | Especifica se os valores da coluna podem ser modificados.
| **required**            | booliano | Especifica se o valor da coluna não é opcional.

As colunas podem conter dados de vários tipos.
As propriedades a seguir indicam qual tipo de dados uma coluna armazena, bem como configurações adicionais para esses dados.
Essas propriedades são mutuamente exclusivas: uma coluna só pode ter uma delas especificada.

| Nome da propriedade     | Tipo                    | Descrição
|:------------------|:------------------------|:-------------------------------
| **boolean**       | [booleanColumn][]       | Esta coluna armazena valores boolianos.
| **calculated**    | [calculatedColumn][]    | Os dados dessa coluna são calculados com base em outras colunas.
| **choice**        | [choiceColumn][]        | Esta coluna armazena dados de uma lista de opções.
| **currency**      | [currencyColumn][]      | Esta coluna armazena valores monetários.
| **dateTime**      | [dateTimeColumn][]      | Esta coluna armazena valores de datetime.
| **defaultValue**  | [defaultColumnValue][]  | O valor padrão dessa coluna.
| **geolocalização**   | [geolocationColumn][]   | Essa coluna armazena uma localização geográfica.
| **lookup**        | [lookupColumn][]        | Os dados dessa coluna são procurados por outra fonte no site.
| **number**        | [numberColumn][]        | Esta coluna armazena valores numéricos.
| **personOrGroup** | [personOrGroupColumn][] | Esta coluna armazena valores de Pessoa ou Grupo.
| **text**          | [textColumn][]          | Esta coluna armazena valores de texto.

Observação: essas propriedades correspondem à enumeração [SPFieldType][] do SharePoint.
Embora os tipos de campo mais comuns sejam representados acima, essa API ainda não tem alguns.
nestes casos, nenhuma das facetas do tipo de coluna serão preenchidas, e a coluna só terá as propriedades básicas.

## <a name="remarks"></a>Comentários

Os valores ColumnDefinitions e valores de campo para colunas `hidden` não são mostrados por padrão.
Para vê-los ao listar **columnDefinitions**, inclua `hidden` na instrução `$select`.
Para vê-los ao exibir valores **field** em [listItems][listItem], inclua as colunas desejadas por nome na instrução `$select`.

[booleanColumn]: booleancolumn.md
[calculatedColumn]: calculatedcolumn.md
[choiceColumn]: choicecolumn.md
[currencyColumn]: currencycolumn.md
[dateTimeColumn]: datetimecolumn.md
[defaultColumnValue]: defaultcolumnvalue.md
[geolocationColumn]: geolocationcolumn.md
[lookupColumn]: lookupcolumn.md
[numberColumn]: numbercolumn.md
[personOrGroupColumn]: personorgroupcolumn.md
[textColumn]: textcolumn.md
[fieldValueSet]: fieldvalueset.md
[campos]: fieldvalueset.md
[listItem]: listitem.md


  [SPFieldType]: /previous-versions/office/sharepoint-server/ms428806(v=office.15)

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ColumnDefinition"
} -->