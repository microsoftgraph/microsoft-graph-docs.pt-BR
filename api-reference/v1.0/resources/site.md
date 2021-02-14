---
author: JeremyKelley
title: Recurso do site
description: O recurso do site fornece metadados e relações para um site do SharePoint.
localization_priority: Priority
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: d9015326d4a1f6ea49abbbd6b14731ebbdc78b56
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/14/2021
ms.locfileid: "50239328"
---
# <a name="site-resource"></a>Recurso do site

Namespace: microsoft.graph

O recurso **site** fornece metadados e relações para um site do SharePoint.

## <a name="methods"></a>Métodos

| Método                | Tipo de retorno | Descrição
|:-------------------------|:-------------|:----------
| [Obter site raiz][]        | site | Acessar o site raiz do SharePoint dentro de um locatário.
| [Obter site][]             | site | Acessar um site do sharePoint usando o siteId.
| [Obter site por caminho][]     | site | Acessar o site raiz do SharePoint com um caminho relativo.
| [Obter site para um grupo][] | site | Acessar o site de equipe de um grupo.
| [Obter análises][]              | [itemAnalytics][] | Obter análises para este recurso. 
| [Obter atividades por intervalo][] | [itemActivityStat][] | Obter uma coleção de **itemActivityStats** dentro do intervalo de tempo especificado.
| [Pesquisar sites][]     | coleção de sites | Pesquise num locatário do SharePoint por sites que correspondam a palavras-chave fornecidas.
| [Seguir site][]          | coleção de sites | Seguir um ou vários sites de usuário.
| [Deixar de seguir site][]        | coleção de sites | Seguir um ou vários sites de usuário.
| [Listar sites seguidos][]  | coleção de sites | Liste os sites que foram seguidos pelo usuário conectado.
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
[Obter atividades por intervalo]: ../api/itemactivitystat-getactivitybyinterval.md
[Pesquisar sites]: ../api/site-search.md
[itemActivityStat]: itemactivitystat.md
[Seguir site]: ../api/site-follow.md
[Deixar de seguir site]: ../api/site-unfollow.md
[Listar sites seguidos]: ../api/sites-list-followed.md
[Obter permissão]: ../api/site-get-permission.md
[Listar permissões]: ../api/site-list-permissions.md
[Criar permissões]: ../api/site-post-permissions.md
[Excluir permissão]: ../api/site-delete-permission.md
[Atualizar permissão]: ../api/site-update-permission.md

## <a name="properties"></a>Propriedades

| Propriedade            | Tipo                                | Descrição                                                                                    |
| :----------------------- | :---------------------------------- | :--------------------------------------------------------------------------------------------- |
| **id**                   | string                              | O identificador exclusivo do item. Somente leitura.                                                  |
| **createdDateTime**      | DateTimeOffset                      | A data e a hora da criação do item. Somente leitura.                                             |
| **description**          | string                              | O texto descritivo do site.                                                             |
| **displayName**          | cadeia de caracteres                              | O texto completo do site. Somente leitura.                                                        |
| **eTag**                 | string                              | ETag do item. Somente leitura.                                                                  |
| **lastModifiedDateTime** | DateTimeOffset                      | A data e a hora que o item foi modificado pela última vez. Somente leitura.                                       |
| **name**                 | string                              | O nome/título do item.                                                                  |
| **root**                 | [root](root.md)                     | Se estiver presente, indica que este é o site raiz do conjunto de sites. Somente leitura.            |
| **sharepointIds**        | [sharepointIds](sharepointids.md)   | Retorna os identificadores úteis para fins de compatibilidade do REST do SharePoint. Somente leitura.                       |
| **siteCollection**       | [siteCollection](sitecollection.md) | Fornece detalhes sobre o conjunto de sites do site. Disponível apenas no site raiz. Somente leitura. |
| **webUrl**               | string (url)                        | A URL que exibe o item no navegador. Somente leitura.                                          |

### <a name="id-property"></a>propriedade do id
Um **site** é identificado por um ID exclusivo que é composto pelos seguintes valores:
* Hostname do conjunto de sites (contoso.sharepoint.com)
* ID exclusiva do conjunto de sites (GUID)
* ID exclusiva do site (GUID)
  
O identificador `root` sempre faz referência ao site raiz de um determinado destino, como a seguir:

* `/sites/root`: O site raiz do locatário.
* `/groups/{group-id}/sites/root`: O site da equipe do grupo.
  
## <a name="relationships"></a>Relações

| Relação      | Tipo                             | Descrição
|:------------------|:---------------------------------|:----------------------
| **analytics**     | [itemAnalytics][] resource       | Análise sobre as atividades de modo de exibição que ocorreram no site.
| **columns**       | Collection([columnDefinition][]) | O conjunto de definições de coluna reutilizáveis entre listas nesse site.
| **contentTypes**  | Collection([contentType][])      | O conjunto de tipos de conteúdo definido para esse site.
| **drive**         | [drive][]                        | A unidade padrão (biblioteca de documentos) desse site.
| **drives**        | Collection([drive][])            | O conjunto de unidades (bibliotecas de documentos) nesse site.
| **items**         | Collection([baseItem][])         | Usado para lidar com qualquer item contido neste site. Não é possível enumerar este conjunto.
| **lists**         | Collection([list][])             | O conjunto de listas neste site.
| **permissions**   | Coleção ([permissão][])         | As permissões associadas ao site. Anulável.
| **sites**         | Collection([site][])             | O conjunto dos subsites neste site.
| **onenote**       | [onenote][]                      | Chama o serviço OneNote para operações relacionadas ao bloco de anotações.

[columnDefinition]: columndefinition.md
[baseItem]: baseitem.md
[contentType]: contenttype.md
[drive]: drive.md
[identitySet]: identityset.md
[itemAnalytics]: itemanalytics.md
[list]: list.md
[permission]: permission.md
[site]: site.md
[onenote]: onenote.md

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
  "onenote": { "@odata.type": "microsoft.graph.onenote"},

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
