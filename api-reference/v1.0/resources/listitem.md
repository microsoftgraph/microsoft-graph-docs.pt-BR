---
author: JeremyKelley
title: recurso listItem
description: Representa um item em uma lista do sharepoint.
ms.localizationpriority: high
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 851b506b029d05bfac2bcecfcce57d9e3ce8684f
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59021460"
---
# <a name="listitem-resource"></a>recurso listItem

Namespace: microsoft.graph

Representa um item em uma [lista][] do Microsoft Office SharePoint Online.

Todos os itens em uma biblioteca de documentos do Microsoft Office SharePoint Online podem ser representados como um **listItem** ou um r [ecurso driveItem][].

Os valores de coluna na lista estão disponíveis por meio do dicionário `fieldValueSet`.

## <a name="methods"></a>Métodos

Os métodos a seguir estão disponíveis para recursos **listItem**.
Todos os exemplos são relativos a uma **[lista][]**:`https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}`.

| Método                    | Tipo de retorno | Descrição
|:-------------------------------|:-------------------|:------
| [Get][]                   | listItem| Obter um item em uma lista.
| [Obter valores de coluna][Obter]       | listItem | Obter valores de coluna de listItem.
| [Obter análises][]              | [itemAnalytics][]| Obter análises para este recurso. 
| [Obter atividades por intervalo][] | [itemActivityStat][]| Obter uma coleção de itemActivityStats dentro do intervalo de tempo especificado.
| [Criar][]                     | listItem | Criar um novo listItem em uma lista.
| [Excluir][]                     | Sem Conteúdo | Remove um item de uma lista.
| [Atualizar][]                     | [fieldValueSet][]| Atualizar as propriedades de um listItem.
| [Atualizar valores de coluna][Atualizar] | [fieldValueSet][]| Atualizar os valores de coluna de um listItem.

[Obter]: ../api/listitem-get.md
[Obter análises]: ../api/itemanalytics-get.md
[Obter atividades por intervalo]: ../api/itemactivitystat-getactivitybyinterval.md
[Create]: ../api/listitem-create.md
[Delete]: ../api/listitem-delete.md
[Atualizar]: ../api/listitem-update.md

[itemActivityStat]: itemactivitystat.md
[fieldValueSet]: fieldvalueset.md

## <a name="properties"></a>Propriedades

O recurso **listItem** tem as seguintes propriedades.

| Nome da propriedade | Tipo                | Descrição
|:--------------|:--------------------|:-------------------------------
| contentType   | [contentTypeInfo][] | O tipo de conteúdo deste item de lista

As propriedades a seguir são herdadas do **[baseItem][]**.

| Nome da propriedade        | Tipo              | Descrição
|:---------------------|:------------------|:----------------------------------
| id                   | string            | O identificador exclusivo do item. Somente leitura.
| name                 | string            | O nome/título do item.
| createdBy            | [identitySet][]   | Identidade do criador deste item. Somente leitura.
| createdDateTime      | DateTimeOffset    | A data e a hora da criação do item. Somente leitura.
| description          | string            | O texto descritivo do item.
| eTag                 | string            | ETag do item. Somente leitura.                                                          |
| lastModifiedBy       | [identitySet][]   | Identidade do último modificador deste item. Somente leitura.
| lastModifiedDateTime | DateTimeOffset    | A data e a hora que o item foi modificado pela última vez. Somente leitura.
| parentReference      | [itemReference][] | Informações do pai, se o item tiver um pai. Leitura e gravação.
| sharepointIds        | [sharepointIds][] | Retorna os identificadores úteis para fins de compatibilidade do REST do SharePoint. Somente leitura.
| webUrl               | string (url)      | A URL que exibe o item no navegador. Somente leitura.

## <a name="relationships"></a>Relações

 O recurso **listItem** tem as seguintes relações com outros recursos.

| Nome da relação | Tipo                           | Descrição
|:------------------|:-------------------------------|:-------------------------------
| activities        | Conjunto [itemActivity][]    | A lista de atividades recentes que ocorreram neste item.
| análise         | recurso [itemAnalytics][]     | Análise sobre as atividades de visualização que ocorreram neste item.
| driveItem         | [driveItem][]                  | Para bibliotecas de documentos, a relação **driveItem** expõe listItem como um **[driveItem][]**
| campos            | [fieldValueSet][]              | Os valores das colunas definidos neste item de lista.
| versões          | coleção [listItemVersion][]  | A lista de versões anteriores do item de lista.

[baseItem]: baseitem.md
[contentTypeInfo]: contenttypeinfo.md
[driveItem]: driveitem.md
[fieldValueSet]: fieldvalueset.md
[identitySet]: identityset.md
[itemActivity]: itemactivity.md
[itemAnalytics]: itemanalytics.md
[itemReference]: itemreference.md
[list]: list.md
[listItemVersion]: listitemversion.md
[sharepointIds]: sharepointids.md

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON de um recurso **listItem**.

<!--{
  "blockType": "resource",
  "keyProperty": "id",
  "baseType": "microsoft.graph.baseItem",
  "@odata.type&quot;: &quot;microsoft.graph.listItem"
}-->

```json
{
  "contentType": { "@odata.type": "microsoft.graph.contentTypeInfo" },
  "fields": { "@odata.type": "microsoft.graph.fieldValueSet" },
  "sharepointIds": { "@odata.type": "microsoft.graph.sharepointIds" },

  /* relationships */
  "activities": [{"@odata.type": "microsoft.graph.itemActivity"}],
  "analytics": { "@odata.type": "microsoft.graph.itemAnalytics" },
  "driveItem": { "@odata.type": "microsoft.graph.driveItem" },
  "versions": [{"@odata.type": "microsoft.graph.listItemVersion"}],

  /* inherited from baseItem */
  "id": "string",
  "name": "name of resource",
  "createdBy": { "@odata.type": "microsoft.graph.identitySet" },
  "createdDateTime": "timestamp",
  "description": "description of resource",
  "eTag": "string",
  "lastModifiedBy": { "@odata.type": "microsoft.graph.identitySet" },
  "lastModifiedDateTime": "timestamp",
  "parentReference": { "@odata.type": "microsoft.graph.itemReference"},
  "webUrl&quot;: &quot;url"
}
```

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/listItem",
  "tocBookmarks": {
    "ListItem&quot;: &quot;#"
  }
} -->

