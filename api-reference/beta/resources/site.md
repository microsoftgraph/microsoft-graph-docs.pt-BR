---
author: JeremyKelley
description: O recurso site fornece metadados e relações para um site do SharePoint.
title: tipo de recurso do site
ms.localizationpriority: high
ms.prod: sites-and-lists
doc_type: resourcePageType
ms.openlocfilehash: 52d5a66533304d2b7df479e2393a7a4a7cf41974
ms.sourcegitcommit: cc9e5b3630cb84c48bbbb2d84a963b9562d1fb78
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/31/2022
ms.locfileid: "64586864"
---
# <a name="site-resource-type"></a>tipo de recurso do site

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

O recurso **site** fornece metadados e relações para um site do SharePoint.

## <a name="methods"></a>Métodos

| Método                                            | Caminho REST                                                   |
| :------------------------------------------------ | :---------------------------------------------------------- |
| [Obter site raiz][]                                 | GET /sites/root                                             |
| [Obter site][]                                      | GET /sites/{site-id}                                        |
| [Obter site por caminho][]                              | GET /sites/{hostname}:/{site-path}                          |
| [Obter o site para um grupo][]                          | GET /groups/{group-id}/sites/root                           |
| [Obter análises][]                                 | GET /sites/{site-id}/analytics                              |
| [Obter atividades por intervalo][]                    | GET /sites/{site-id}/getActivitiesByInterval                |
| [Listar páginas][]                                    | GET /sites/{site-id}/pages                                  |
| [Lista sites raiz][]                               | GET /sites?filter=root ne null&select=siteCollection,webUrl |
| [Procurar sites][]                              | GET /sites?search={query}                                   |
| [Seguir site][]                                   | POST /users/{user-id}/followedSites/add                     |
| [Deixar de seguir site][]                                 | POST /users/{user-id}/followedSites/remove                  |
| [Listar sites seguidos][]                           | GET /me/followedSites                                       |
| [Obter permissão][]                                | GET /sites/{site-id}/permissions/{permission-id}            |
| [Listar permissões][]                              | GET /sites/{site-id}/permissions                            |
| [Criar permissões][]                            | POST /sites/{site-id}/permissions                           |
| [Excluir permissão][]                             | DELETE /sites/{site-id}/permissions/{permission-id}         |
| [Atualizar permissão][]                             | PATCH /sites/{site-id}/permissions/{permission-id}          |
| [Tipos de conteúdo de lista][]                            | Obter /sites/{site-id}/contentTypes                           |
| [Criar contentType][]                            | POSTAR /sites/{site-id}/contentTypes                          |
| [Colunas de lista][]                                  | OBTER /sites/{site-id}/columns                                |
| [Criar coluna][]                                 | POSTAR /sites/{site-id}/columns                               |
| [Listar operações](../api/site-list-operations.md) | OBTER /sites/{site-id}/operações                             |
| [Obter configurações do site][]                             | GET /sites/{site-id}/settings                               |

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
[Tipos de conteúdo de lista]: ../api/site-list-contenttypes.md
[Criar contentType]: ../api/site-post-contenttypes.md
[Colunas de lista]: ../api/site-list-columns.md
[Criar coluna]: ../api/site-post-columns.md
[Obter configurações do site]: ../api/sitesettings-get.md

## <a name="properties"></a>Propriedades

| Propriedade                 | Tipo               | Descrição                                                                                    |
| :----------------------- | :----------------- | :--------------------------------------------------------------------------------------------- |
| **id**                   | cadeia de caracteres             | O [identificador exclusivo](#id-property) do item. Somente leitura.                                  |
| **createdDateTime**      | DateTimeOffset     | A data e a hora da criação do item. Somente leitura.                                             |
| **description**          | string             | O texto descritivo do site.                                                             |
| **eTag**                 | string             | ETag do item. Somente leitura.                                                                  |
| **displayName**          | cadeia de caracteres             | O texto completo do site. Somente leitura.                                                        |
| **lastModifiedDateTime** | DateTimeOffset     | A data e a hora que o item foi modificado pela última vez. Somente leitura.                                       |
| **name**                 | string             | O nome/título do item.                                                                  |
| **root**                 | [root][]           | Se estiver presente, indica que este é o site raiz do conjunto de sites. Somente leitura.            |
| **configurações**             | [siteSettings]     | As configurações neste site. Retornado apenas em $select. Somente leitura.                                |
| **sharepointIds**        | [sharepointIds][]  | Retorna os identificadores úteis para fins de compatibilidade do REST do SharePoint. Somente leitura.                       |
| **siteCollection**       | [siteCollection][] | Fornece detalhes sobre o conjunto de sites do site. Disponível apenas no site raiz. Somente leitura. |
| **webUrl**               | string (url)       | A URL que exibe o item no navegador. Somente leitura.                                          |

### <a name="id-property"></a>propriedade do id

Um **site** é identificado por um ID exclusivo que é composto pelos seguintes valores:
* Hostname do conjunto de sites (contoso.sharepoint.com)
* ID exclusiva do conjunto de sites (GUID)
* ID exclusiva do site (GUID)

O identificador `root` sempre faz referência ao site raiz de um determinado destino, como a seguir:

* `/sites/root`: O site raiz do locatário.
* `/groups/{group-id}/sites/root`: O site da equipe do grupo.

## <a name="relationships"></a>Relações

| Relação        | Tipo                                                                            | Descrição                                                                                                                                |
| :------------------ | :------------------------------------------------------------------------------ | :----------------------------------------------------------------------------------------------------------------------------------------- |
| **analytics**       | [itemAnalytics][] resource                                                      | Análise sobre as atividades de modo de exibição que ocorreram no site.                                                                          |
| **columns**         | Collection([columnDefinition][])                                                | O conjunto de definições de coluna reutilizáveis entre listas nesse site.                                                                |
| **contentTypes**    | Collection([contentType][])                                                     | O conjunto de tipos de conteúdo definido para esse site.                                                                                     |
| **drive**           | [drive][]                                                                       | A unidade padrão (biblioteca de documentos) desse site.                                                                                        |
| **drives**          | Collection([drive][])                                                           | O conjunto de unidades (bibliotecas de documentos) nesse site.                                                                             |
| **items**           | Collection([baseItem][])                                                        | Usado para lidar com qualquer item contido neste site. Não é possível enumerar este conjunto.                                                     |
| **lists**           | Collection([list][])                                                            | O conjunto de listas neste site.                                                                                                   |
| **operations**      | Coleção [richLongRunningOperation](../resources/richlongrunningoperation.md) | A coleção de operações de execução prolongada para o site.                                                                                    |
| **pages**           | Collection([sitePage][])                                                        | O conjunto de páginas na lista SitePages no site.                                                                                |
| **permissões**     | Coleção ([permissão][])                                                      | As permissões associadas ao site. Nulas.                                                                                        |
| **sites**           | Collection([site][])                                                            | O conjunto dos subsites neste site.                                                                                           |
| **LojaDeTermos**       | [microsoft.graph.termStore.store]                                               | A LojaDeTermos sob este site.                                                                                                             |
| **externalColumns** | Collection([columnDefinition][])                                                | A coleção de definições de coluna disponíveis no site que são referenciadas nos sites na hierarquia pai do site atual. |

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
[siteSettings]: sitesettings.md
[sharepointIds]: sharepointids.md
[siteCollection]: sitecollection.md
[microsoft.graph.termStore.store]: termstore-store.md

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

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
  "displayName": "string",
  "id": "string",
  "root": { "@odata.type": "microsoft.graph.root" },
  "settings": { "@odata.type": "microsoft.graph.sitesettings" },
  "sharepointIds": { "@odata.type": "microsoft.graph.sharepointIds" },
  "siteCollection": {"@odata.type": "microsoft.graph.siteCollection"},

  /* relationships */
  "analytics": { "@odata.type": "microsoft.graph.itemAnalytics" },
  "columns": [ { "@odata.type": "microsoft.graph.columnDefinition" }],
  "contentTypes": [ { "@odata.type": "microsoft.graph.contentType" }],
  "externalColumns": [ { "@odata.type": "microsoft.graph.columnDefinition" }],
  "drive": { "@odata.type": "microsoft.graph.drive" },
  "drives": [ { "@odata.type": "microsoft.graph.drive" }],
  "items": [ { "@odata.type": "microsoft.graph.baseItem" }],
  "lists": [ { "@odata.type": "microsoft.graph.list" }],
  "permissions": [ { "@odata.type": "microsoft.graph.permission" }],
  "sites": [ { "@odata.type": "microsoft.graph.site"} ],
  "termStore": { "@odata.type": "microsoft.graph.termStore.store" },

  /* inherited from baseItem */
  "createdDateTime": "datetime",
  "description": "string",
  "eTag": "string",
  "lastModifiedDateTime": "datetime",
  "name": "string",
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
