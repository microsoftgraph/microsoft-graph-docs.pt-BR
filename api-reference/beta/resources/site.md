---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Site
localization_priority: Priority
ms.prod: sharepoint
ms.openlocfilehash: 1676a314b7c1283918518655b3180cbc70ca193e
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27952346"
---
# <a name="site-resource-type"></a>tipo de recurso de site

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

O recurso **site** fornece metadados e relações para um site do SharePoint.

## <a name="methods"></a>Métodos

| Método                         | Caminho REST
|:-------------------------------|:--------------------------------------------
| [Obter site raiz][]              | GET /sites/root
| [Obter site][]                   | GET /sites/{site-id}
| [Obter site por caminho][]           | GET /sites/{hostname}:/{site-path}
| [Obter o site para um grupo][]       | GET /groups/{group-id}/sites/root
| [Obtenha a análise][]              | GET /sites/ {site-id} / análise
| [Fazer atividades pelo intervalo][] | GET /sites/ {site-id} / getActivitiesByInterval
| [Listar páginas][]                 | GET /sites/ {site-id} / páginas
| [Lista de sites de raiz][]            | GET /sites? filtro = raiz ne nulo & Selecionar = siteCollection, webUrl
| [Procurar sites][]           | GET /sites?search={query}

[Obter site]: ../api/site-get.md
[Obter site raiz]: ../api/site-get.md
[Obter site por caminho]: ../api/site-getbypath.md
[Obter o site para um grupo]: ../api/site-get.md
[Obtenha a análise]: ../api/itemanalytics-get.md
[Fazer atividades pelo intervalo]: ../api/itemactivity-getbyinterval.md
[Listar páginas]: ../api/sitepage-list.md
[Lista de sites de raiz]: ../api/site-list.md
[Procurar sites]: ../api/site-search.md


## <a name="properties"></a>Propriedades

| Nome da propriedade            | Tipo               | Descrição
|:-------------------------|:-------------------|:-----------------------------
| **id**                   | string             | O identificador exclusivo do item. Somente leitura.
| **createdDateTime**      | DateTimeOffset     | A data e a hora da criação do item. Somente leitura.
| **description**          | string             | O texto descritivo do site.
| **eTag**                 | string             | ETag do item. Somente leitura.                                                                  |
| **displayName**          | string             | O texto completo do site. Somente leitura.
| **lastModifiedDateTime** | DateTimeOffset     | A data e a hora que o item foi modificado pela última vez. Somente leitura.
| **name**                 | string             | O nome/título do item.
| **root**                 | [root][]           | Se estiver presente, indica que este é o site raiz do conjunto de sites. Somente leitura.
| **sharepointIds**        | [sharepointIds][]  | Retorna os identificadores úteis para fins de compatibilidade do REST do SharePoint. Somente leitura.
| **siteCollection**       | [siteCollection][] | Fornece detalhes sobre o conjunto de sites do site. Disponível apenas no site raiz. Somente leitura.
| **webUrl**               | string (url)       | A URL que exibe o item no navegador. Somente leitura.

## <a name="relationships"></a>Relações

| Nome da relação | Tipo                             | Descrição
|:------------------|:---------------------------------|:----------------------
| **análise**     | recurso de [itemAnalytics][]       | Análise sobre as atividades de modo de exibição que foram realizada neste site.
| **columns**       | Collection([columnDefinition][]) | O conjunto de definições de coluna reutilizáveis entre listas nesse site.
| **contentTypes**  | Collection([contentType][])      | O conjunto de tipos de conteúdo definido para esse site.
| **drive**         | [drive][]                        | A unidade padrão (biblioteca de documentos) desse site.
| **drives**        | Collection([drive][])            | O conjunto de unidades (bibliotecas de documentos) nesse site.
| **items**         | Collection([baseItem][])         | Usado para lidar com qualquer item contido neste site. Não é possível enumerar este conjunto.
| **lists**         | Collection([list][])             | O conjunto de listas neste site.
| **páginas**         | Coleção ([sitePage][])         | A coleção de páginas na lista SitePages neste site.
| **sites**         | Collection([site][])             | O conjunto dos subsites neste site.

[columnDefinition]: columndefinition.md
[baseItem]: baseitem.md
[contentType]: contenttype.md
[drive]: drive.md
[identitySet]: identityset.md
[itemAnalytics]: itemanalytics.md
[lista]: list.md
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
  "sites": [ { "@odata.type": "microsoft.graph.site"} ],
  "columns": [ { "@odata.type": "microsoft.graph.columnDefinition" }],

  /* inherited from baseItem */
  "name": "string",
  "createdDateTime": "datetime",
  "description": "string",
  "eTag": "string",
  "lastModifiedDateTime": "datetime",
  "webUrl": "url"
}
```

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Sites",
  "tocBookmarks": { "Resources/Site": "#" }
} -->
