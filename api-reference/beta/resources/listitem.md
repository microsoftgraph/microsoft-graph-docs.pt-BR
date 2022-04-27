---
author: JeremyKelley
description: Esse recurso representa um item em uma SharePoint lista.
title: recurso listItem
ms.localizationpriority: medium
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: bfda041c473da6d5d98c7c6b076ba9be276cd486
ms.sourcegitcommit: 5516b107d72caef6ec042fe74228be4031b32fa5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2022
ms.locfileid: "65060672"
---
# <a name="listitem-resource"></a>recurso listItem

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um item em uma [lista][] do Microsoft Office SharePoint Online.

Todos os itens em uma biblioteca de documentos do Microsoft Office SharePoint Online podem ser representados como um **listItem** ou um r [ecurso driveItem][].

Os valores de coluna na lista estão disponíveis por meio do dicionário `fieldValueSet`.

## <a name="tasks-on-a-listitem"></a>Tarefas em um listItem

As tarefas a seguir estão disponíveis para recursos **listItem**.
Todos os exemplos a seguir referem-se a uma **[list][]**, por exemplo: `https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}`.

| Tarefa comum                    | Método HTTP                                  |
| :----------------------------- | :------------------------------------------- |
| [Get][]                        | GET /items/{item-id}                         |
| [Obter valores de coluna][Get]       | GET /items/{item-id}?expand=fields           |
| [Obter análises][]              | GET /items/{item-id}/analytics               |
| [Obter atividades por intervalo][] | GET /items/{item-id}/getActivitiesByInterval |
| [Create][]                     | POST /items                                  |
| [Delete][]                     | DELETE /items/{item-id}                      |
| [Update][]                     | PATCH /items/{item-id}                       |
| [Atualizar valores de coluna][Update] | PATCH /items/{item-id}/fields                |
| [createLink][CreateLink]       | POST /items/{itemId}/createLink              |
|[Listar documentSetVersions](../api/listitem-list-documentsetversions.md)| GET /items/{item-id}/documentSetVersions |
|[Criar documentSetVersion](../api/listitem-post-documentsetversions.md)| POST /items/{item-id}/documentSetVersions |
|[Restaurar documentSetVersion](../api/documentsetversion-restore.md)| POST /items/{item-id}/documentSetVersions/{documentSetVersion-id}/restore |

[Obter]: ../api/listitem-get.md
[Obter análises]: ../api/itemanalytics-get.md
[Obter atividades por intervalo]: ../api/itemactivity-getbyinterval.md
[Create]: ../api/listitem-create.md
[Delete]: ../api/listitem-delete.md
[Update]: ../api/listitem-update.md
[CreateLink]: ../api/listitem-createlink.md

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
  "documentSetVersions": [{"@odata.type": "microsoft.graph.documentSetVersion"}],
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

## <a name="properties"></a>Propriedades

O recurso **listItem** tem as seguintes propriedades.

| Propriedade    | Tipo                | Descrição                        |
| :---------- | :------------------ | :--------------------------------- |
| contentType | [contentTypeInfo][] | O tipo de conteúdo deste item de lista |

As propriedades a seguir são herdadas do **[baseItem][]**.

| Nome da propriedade        | Tipo              | Descrição                                                              |
| :------------------- | :---------------- | :----------------------------------------------------------------------- |
| id                   | string            | O identificador exclusivo do item. Somente leitura.                            |
| name                 | string            | O nome/título do item.                                            |
| createdBy            | [identitySet][]   | Identidade do criador deste item. Somente leitura.                         |
| createdDateTime      | DateTimeOffset    | A data e a hora da criação do item. Somente leitura.                       |
| description          | string            | O texto descritivo do item.                                       |
| eTag                 | string            | ETag do item. Somente leitura.                                            |
| lastModifiedBy       | [identitySet][]   | Identidade do último modificador deste item. Somente leitura.                   |
| lastModifiedDateTime | DateTimeOffset    | A data e a hora que o item foi modificado pela última vez. Somente leitura.                 |
| parentReference      | [itemReference][] | Informações do pai, se o item tiver um pai. Leitura e gravação.                |
| sharepointIds        | [sharepointIds][] | Retorna os identificadores úteis para fins de compatibilidade do REST do SharePoint. Somente leitura. |
| webUrl               | string (url)      | A URL que exibe o item no navegador. Somente leitura.                    |

## <a name="relationships"></a>Relações

 O recurso **listItem** tem as seguintes relações com outros recursos.

| Relação | Tipo                           | Descrição                                                                                        |
| :----------- | :----------------------------- | :------------------------------------------------------------------------------------------------- |
| activities   | Conjunto [itemActivity][]    | A lista de atividades recentes que ocorreram neste item.                                        |
| análise    | recurso [itemAnalytics][]     | Análise sobre as atividades de visualização que ocorreram neste item.|
|documentSetVersions|[coleção documentSetVersion](../resources/documentsetversion.md)| Informações de versão para uma versão do conjunto de documentos criada por um usuário.|
| driveItem    | [driveItem][]                  | Para bibliotecas de documentos, a relação **driveItem** expõe listItem como um **[driveItem][]** |
| campos       | [fieldValueSet][]              | Os valores das colunas definidos neste item de lista.                                                   |
| versões     | coleção [listItemVersion][]  | A lista de versões anteriores do item de lista.                                                    |

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

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ListItem",
  "tocBookmarks": {
    "ListItem&quot;: &quot;#"
  },
  "suppressions": []
}
-->
