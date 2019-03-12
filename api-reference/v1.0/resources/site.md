---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Site
localization_priority: Priority
ms.prod: sharepoint
ms.openlocfilehash: d4dfb3f340a2b2b7ff5ad5a3c9279cb2a03c63be
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2019
ms.locfileid: "30482088"
---
# <a name="site-resource"></a>Recurso site

O recurso **site** fornece metadados e relações para um site do SharePoint.

## <a name="tasks"></a>Tarefas

Todos os exemplos a seguir referem-se ao endereço `https://graph.microsoft.com/v1.0`.

| Nome da tarefa                | Exemplo de Solicitação
|:-------------------------|:--------------------------------------------------
| [Obter site raiz][]        | GET /sites/root
| [Obter site][]             | GET /sites/{site-id}
| [Obter site por caminho][]     | GET /sites/{hostname}:/{site-path}
| [Obter o site para um grupo][] | GET /groups/{group-id}/sites/root
| [Procurar sites][]     | GET /sites?search={query}

[Obter site]: ../api/site-get.md
[Obter site raiz]: ../api/site-get.md
[Obter site por caminho]: ../api/site-getbypath.md
[Obter o site para um grupo]: ../api/site-get.md
[Procurar sites]: ../api/site-search.md

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
  "contentTypes": [ { "@odata.type": "microsoft.graph.contentType" }],
  "drive": { "@odata.type": "microsoft.graph.drive" },
  "drives": [ { "@odata.type": "microsoft.graph.drive" }],
  "items": [ { "@odata.type": "microsoft.graph.baseItem" }],
  "lists": [ { "@odata.type": "microsoft.graph.list" }],
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

## <a name="properties"></a>Propriedades

| Nome da propriedade            | Tipo                                | Descrição                                                                                    |
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

## <a name="relationships"></a>Relações

| Nome da relação | Tipo                             | Descrição
|:------------------|:---------------------------------|:----------------------
| **columns**       | Collection([columnDefinition][]) | O conjunto de definições de coluna reutilizáveis entre listas nesse site.
| **contentTypes**  | Collection([contentType][])      | O conjunto de tipos de conteúdo definido para esse site.
| **drive**         | [drive][]                        | A unidade padrão (biblioteca de documentos) desse site.
| **drives**        | Collection([drive][])            | O conjunto de unidades (bibliotecas de documentos) nesse site.
| **items**         | Collection([baseItem][])         | Usado para lidar com qualquer item contido neste site. Não é possível enumerar este conjunto.
| **lists**         | Collection([list][])             | O conjunto de listas neste site.
| **sites**         | Collection([site][])             | O conjunto dos subsites neste site.
| **onenote**       | [onenote][]                      | Chama o serviço OneNote para operações relacionadas ao bloco de anotações.

[columnDefinition]: columndefinition.md
[baseItem]: baseitem.md
[contentType]: contenttype.md
[drive]: drive.md
[identitySet]: identityset.md
[list]: list.md
[site]: site.md
[onenote]: onenote.md

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Sites",
  "tocBookmarks": { "Resources/Site": "#" }
} -->
