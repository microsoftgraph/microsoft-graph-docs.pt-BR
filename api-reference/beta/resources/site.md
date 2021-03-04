---
author: JeremyKelley
description: O recurso site fornece metadados e relações para um site do SharePoint.
ms.date: 09/10/2017
title: Site
localization_priority: Priority
ms.prod: sites-and-lists
doc_type: resourcePageType
ms.openlocfilehash: 587014aa0c9dbe4c05c0e3b946c3f6e44b7cb821
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50442784"
---
# <a name="site-resource-type"></a>tipo de recurso do site

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

O recurso **site** fornece metadados e relações para um site do SharePoint.

## <a name="methods"></a>Métodos

| Método                         | Caminho REST
|:-------------------------------|:--------------------------------------------
| [Obter site raiz][]              | GET /sites/root
| [Obter site][]                   | GET /sites/{site-id}
| [Obter site por caminho][]           | GET /sites/{hostname}:/{site-path}
| [Obter o site para um grupo][]       | GET /groups/{group-id}/sites/root
| [Obter análises][]              | GET /sites/{site-id}/analytics
| [Obter atividades por intervalo][] | GET /sites/{site-id}/getActivitiesByInterval
| [Listar páginas][]                 | GET /sites/{site-id}/pages
| [Lista sites raiz][]            | GET /sites?filter=root ne null&select=siteCollection,webUrl
| [Procurar sites][]           | GET /sites?search={query}
| [Seguir site][]                | POST /users/{user-id}/followedSites/add
| [Deixar de seguir site][]              | POST /users/{user-id}/followedSites/remove
| [Listar sites seguidos][]        | GET /me/followedSites
| [Obter permissão][]             | GET /sites/{site-id}/permissions/{permission-id}
| [Listar permissões][]           | GET /sites/{site-id}/permissions
| [Criar permissões][]         | POST /sites/{site-id}/permissions
| [Excluir permissão][]         | DELETE /sites/{site-id}/permissions/{permission-id}
| [Atualizar permissão][]         | PATCH /sites/{site-id}/permissions/{permission-id}

[Obter site]: ../api/site-get.md
[Obter site raiz]: ../api/site-get.md
[Obter site por caminho]: ../api/site-getbypath.md
[Obter o site para um grupo]: ../api/site-get.md
[Obter análises]: ../api/itemanalytics-get.md
[Obter atividades por intervalo]: ../api/itemactivity-getbyinterval.md
[Listar páginas]: ../api/sitepage-list.md
[Lista sites raiz]: ../api/site-list.md
[Procurar sites]: ../api/site-search.md
[Seguir site]: ../api/site-follow.md
[Deixar de seguir site]: ../api/site-unfollow.md
[Listar sites seguidos]: ../api/sites-list-followed.md
[Obter permissão]: ../api/site-get-permission.md
[Listar permissões]: ../api/site-list-permissions.md
[Criar permissões]: ../api/site-post-permissions.md
[Excluir permissão]: ../api/site-delete-permission.md
[Atualizar permissão]: ../api/site-update-permission.md


## <a name="properties"></a>Propriedades

| Nome da propriedade            | Tipo               | Descrição
|:-------------------------|:-------------------|:-----------------------------
| **id**                   | cadeia de caracteres             | O [identificador exclusivo](#id-property) do item. Somente leitura.
| **createdDateTime**      | DateTimeOffset     | A data e a hora da criação do item. Somente leitura.
| **description**          | string             | O texto descritivo do site.
| **eTag**                 | string             | ETag do item. Somente leitura.                                                                  |
| **displayName**          | cadeia de caracteres             | O texto completo do site. Somente leitura.
| **lastModifiedDateTime** | DateTimeOffset     | A data e a hora que o item foi modificado pela última vez. Somente leitura.
| **name**                 | string             | O nome/título do item.
| **root**                 | [root][]           | Se estiver presente, indica que este é o site raiz do conjunto de sites. Somente leitura.
| **sharepointIds**        | [sharepointIds][]  | Retorna os identificadores úteis para fins de compatibilidade do REST do SharePoint. Somente leitura.
| **siteCollection**       | [siteCollection][] | Fornece detalhes sobre o conjunto de sites do site. Disponível apenas no site raiz. Somente leitura.
| **webUrl**               | string (url)       | A URL que exibe o item no navegador. Somente leitura.

### <a name="id-property"></a>propriedade do id
Um **site** é identificado por um ID exclusivo que é composto pelos seguintes valores:
* Hostname do conjunto de sites (contoso.sharepoint.com)
* ID exclusiva do conjunto de sites (GUID)
* ID exclusiva do site (GUID)
  
O identificador `root` sempre faz referência ao site raiz de um determinado destino, como a seguir:

* `/sites/root`: O site raiz do locatário.
* `/groups/{group-id}/sites/root`: O site da equipe do grupo.

## <a name="relationships"></a>Relações

| Nome da relação | Tipo                             | Descrição
|:------------------|:---------------------------------|:----------------------
| **analytics**     | [itemAnalytics][] resource       | Análise sobre as atividades de modo de exibição que ocorreram no site.
| **columns**       | Collection([columnDefinition][]) | O conjunto de definições de coluna reutilizáveis entre listas nesse site.
| **contentTypes**  | Collection([contentType][])      | O conjunto de tipos de conteúdo definido para esse site.
| **drive**         | [drive][]                        | A unidade padrão (biblioteca de documentos) desse site.
| **drives**        | Collection([drive][])            | O conjunto de unidades (bibliotecas de documentos) nesse site.
| **items**         | Collection([baseItem][])         | Usado para lidar com qualquer item contido neste site. Não é possível enumerar este conjunto.
| **lists**         | Collection([list][])             | O conjunto de listas neste site.
| **pages**         | Collection([sitePage][])         | O conjunto de páginas na lista SitePages no site.
| **permissões**   | Coleção ([permissão][])         | As permissões associadas ao site. Anulável.
| **sites**         | Collection([site][])             | O conjunto dos subsites neste site.
| **externalColumns**     | Collection([columnDefinition][])  | A coleção de definições de coluna disponíveis no site que são referenciadas nos sites na hierarquia pai do site atual.

[columnDefinition]: columndefinition.md
[baseItem]: baseitem.md
[contentType]: contenttype.md
[drive]: drive.md
[identitySet]: identityset.md
[itemAnalytics]: itemanalytics.md
[list]: list.md
[permissão]: permission.md
[sitePage]: sitepage.md
[root]: root.md
[site]: site.md
[sharepointIds]: sharepointids.md
[siteCollection]: sitecollection.md

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON de um recurso **site**.

O recurso **site** é derivado de [**baseItem**](baseitem.md) e herda propriedades desse recurso.

<!--{
  "blockType": "resource",
  "optionalProperties": [
    "root",
    "sharepointIds",
    "siteCollection",
    "drive",
    "drives",
    "permissions",
    "sites"
  ],
  "keyProperty": "id",
  "baseType": "microsoft.graph.baseItem",
  "@odata.type": "microsoft.graph.site"
}-->

```json
{
  "id": "string",
  "root": { "@odata.type": "microsoft.graph.root" },
  "sharepointIds": { "@odata.type": "microsoft.graph.sharepointIds" },
  "siteCollection": {"@odata.type": "microsoft.graph.siteCollection"},
  "displayName": "string",

  /* relationships */
  "analytics": { "@odata.type": "microsoft.graph.itemAnalytics" },
  "contentTypes": [ { "@odata.type": "microsoft.graph.contentType" }],
  "drive": { "@odata.type": "microsoft.graph.drive" },
  "drives": [ { "@odata.type": "microsoft.graph.drive" }],
  "items": [ { "@odata.type": "microsoft.graph.baseItem" }],
  "lists": [ { "@odata.type": "microsoft.graph.list" }],
  "permissions": [ { "@odata.type": "microsoft.graph.permission" }],
  "sites": [ { "@odata.type": "microsoft.graph.site"} ],
  "columns": [ { "@odata.type": "microsoft.graph.columnDefinition" }],
  "externalColumns": [ { "@odata.type": "microsoft.graph.columnDefinition" }],
  /* inherited from baseItem */
  "name": "string",
  "createdDateTime": "datetime",
  "description": "string",
  "eTag": "string",
  "lastModifiedDateTime": "datetime",
  "webUrl": "url"
}
```

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Sites",
  "tocBookmarks": {
    "Resources/Site": "#"
  },
  "suppressions": []
}
-->
