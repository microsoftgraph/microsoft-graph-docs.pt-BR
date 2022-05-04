---
author: daspek
description: O recurso contentType representa um tipo de conteúdo no SharePoint.
title: Tipo de recurso contentType
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: sites-and-lists
ms.openlocfilehash: 6c7c45b74088902f4f1565b52c96577cfcd6e3ca
ms.sourcegitcommit: 089669703041900c4700c5d4f383ed05a7f193f8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/04/2022
ms.locfileid: "65191342"
---
# <a name="contenttype-resource-type"></a>Tipo de recurso contentType

Namespace: microsoft.graph


Representa um tipo de conteúdo SharePoint.
Os tipos de conteúdo permitem definir um conjunto de colunas que devem estar presentes em [**cada listItem**][listItem] em uma [**lista**][list].

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar contentTypes em um site](../api/site-list-contenttypes.md)|[Coleção contentType](../resources/contenttype.md)|Obtenha uma lista dos objetos [contentType](../resources/contenttype.md) e suas propriedades em um [site](../resources/site.md).|
|[Listar contentTypes em uma lista](../api/list-list-contenttypes.md)|[Coleção contentType](../resources/contenttype.md)|Obtenha uma lista dos [objetos contentType](../resources/contenttype.md) e suas propriedades em uma [lista](../resources/list.md).|
|[Criar contentType para um site](../api/site-post-contenttypes.md)|[contentType](../resources/contenttype.md)|Crie um novo [objeto contentType](../resources/contenttype.md) em um [site](../resources/site.md).|
|[Obter contentType](../api/contenttype-get.md)|[contentType](../resources/contenttype.md)|Leia as propriedades e as relações de um [objeto contentType](../resources/contenttype.md) .|
|[Atualizar contentType](../api/contenttype-update.md)|[contentType](../resources/contenttype.md)|Atualize as propriedades de um [objeto contentType](../resources/contenttype.md) .|
|[Excluir contentType](../api/contenttype-delete.md)|Nenhuma|Exclui um [objeto contentType](../resources/contenttype.md) .|
|[isPublished](../api/contenttype-ispublished.md)|Booliano| Verifica se [o contentType](../resources/contenttype.md) foi publicado.|
|[publish](../api/contenttype-publish.md)|[contentType](../resources/contenttype.md)| Publicar um [contentType](../resources/contenttype.md).|
|[unpublish](../api/contenttype-unpublish.md)|[contentType](../resources/contenttype.md)|Cancele a publicação de [um contentType](../resources/contenttype.md).|
|[addCopy](../api/contenttype-addcopy.md)|[contentType](../resources/contenttype.md)|Adicione uma cópia de [um contentType](../resources/contenttype.md) de um [site](../resources/site.md) a uma [lista](../resources/list.md).|
|[associateWithHubSites](../api/contenttype-associatewithhubsites.md)|[contentType](../resources/contenttype.md)|Associa um [contentType](../resources/contenttype.md) a uma lista de sites de hub.|
|[copyToDefaultContentLocation](../api/contenttype-copytodefaultcontentlocation.md)|[contentType](../resources/contenttype.md)| Copie um arquivo para o local de conteúdo padrão em um [contentType](../resources/contenttype.md).|
|[Colunas de lista](../api/contenttype-list-columns.md)|[coleção columnDefinition](../resources/columnDefinition.md)|Obtenha uma coleção de colunas, representadas como [recursos columnDefinition](../resources/columnDefinition.md) , em um **contentType**.|
|[Criar coluna](../api/contenttype-post-columns.md)|[columnDefinition](../resources/columnDefinition.md)|Adicione uma coluna a um **tipo de conteúdo** em um site ou lista.|
|[getCompatibleHubContentTypes](../api/contenttype-getcompatiblehubcontenttypes.md)|[Coleção contentType](../resources/contenttype.md)|Obtenha uma lista de tipos de conteúdo compatíveis do hub de tipo de conteúdo que pode ser adicionado a um [site de destino](../resources/site.md) ou a uma [lista](../resources/list.md).|
|[addCopyFromContentTypeHub](../api/contenttype-addcopyfromcontenttypehub.md)|[contentType](../resources/contenttype.md)|Adicione ou sincronize uma cópia de um tipo de conteúdo publicado do hub de tipo de conteúdo para um [site de destino](../resources/site.md) ou uma [lista](../resources/list.md).|


## <a name="properties"></a>Propriedades

| Propriedade     | Tipo                 | Descrição|
|:------------------|:---------------------|:----------------------------------|
| associatedHubsUrls         | Collection(string) | Lista de URLs canônicas para sites de hub aos quais esse tipo de conteúdo está associado. Isso conterá todos os sites de hub em que esse tipo de conteúdo está na fila para ser imposto ou já está imposto. Impor um tipo de conteúdo significa que o tipo de conteúdo será aplicado às listas nos sites impostos.|
| description       | string               | O texto descritivo do item.|
| documentSet         | [documentSet][]      | [Metadados do Conjunto](/sharepoint/governance/document-set-planning#about-document-sets) de Documentos.|
| documentTemplate    | [documentSetContent][] | Metadados do modelo de documento. Para garantir que os documentos tenham conteúdo consistente em um site e em seus subsites, você pode associar um word, Excel ou PowerPoint a um tipo de conteúdo de site.|
| group             | string               | O nome do grupo ao qual esse tipo de conteúdo pertence. Ajuda a organizar os tipos de conteúdo relacionados.|
| hidden            | Booliano              | Indica se o tipo de conteúdo está oculto no menu “Novo” da lista.|
| id                | cadeia de caracteres               | O identificador exclusivo do tipo de conteúdo.|
| inheritedFrom   | [itemReference][]    | Se esse tipo de conteúdo for herdado de outro escopo (como um site), fornece uma referência para o item no qual o tipo de conteúdo foi definido.|
| isBuiltIn            | Booliano| Especifica se um tipo de conteúdo é um tipo de conteúdo interno. |
| nome              | string               | O nome do tipo de conteúdo.|
| Ordem             | [contentTypeOrder][] | Especifica a ordem na qual o tipo de conteúdo aparece na seleção da interface do usuário.|
| Parentid          | string               | O identificador exclusivo do tipo de conteúdo.|
| propagateChanges     | Booliano              | Se `true`, quaisquer alterações feitas no tipo de conteúdo serão enviadas por push para tipos de conteúdo herdados e listas que implementam o tipo de conteúdo.|
| Readonly          | Booliano              | Se `true`, o tipo de conteúdo não pode ser modificado, a menos que esse valor seja definido pela primeira vez como `false`.|
| sealed            | Booliano              | Se `true`, o tipo de conteúdo não pode ser modificado por usuários ou por meio de operações de push down. Somente administradores de conjunto de sites podem lacrar ou retirar o lacre dos tipos de conteúdo.|


## <a name="relationships"></a>Relações

| Relação    | Tipo                      | Descrição|
|:----------------|:--------------------------|:-------------------------------|
| Base     | [contentType][]  | ContentType pai do qual esse tipo de conteúdo é derivado. |
| columnLinks   | Conjunto [columnLink][] | A coleção de colunas que são exigidas por esse tipo de conteúdo.|
| Basetypes     | Collection([contentType][])     | A coleção de tipos de conteúdo que são ancestrais desse tipo de conteúdo.|
| columnPositions         | Collection([columnDefinition][]) | Informações de ordem de coluna em um tipo de conteúdo.|
| columns       | Collection([columnDefinition][])  | A coleção de definições de coluna para este contentType.|

Para mais informações, confira [Introdução a tipos de conteúdo e publicação de tipo de conteúdo][contentTypeIntro].

[columnLink]: columnlink.md
[contentTypeIntro]: https://support.office.com/en-us/article/Introduction-to-content-types-and-content-type-publishing-e1277a2e-a1e8-4473-9126-91a0647766e5
[itemReference]: itemreference.md
[contentTypeOrder]: contenttypeorder.md
[columnDefinition]: columnDefinition.md
[contentType]: contentType.md
[documentSet]: documentSet.md
[documentSetContent]: documentSetContent.md

## <a name="json-representation"></a>Representação JSON

A seguir está uma representação JSON de um **recurso contentType** .

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.contentType","keyProperty":"id" } -->

```json
{
  "associatedHubsUrls" : ["string"],
  "base": { "@type": "microsoft.graph.contentType" },
  "baseTypes" : [{ "@type": "microsoft.graph.contentType" }],
  "columns" : [{ "@type": "microsoft.graph.columnDefinition" }],
  "columnLinks": [{ "@type": "microsoft.graph.columnLink" }],
  "columnPositions" : [{ "@type": "microsoft.graph.columnDefinition" }],
  "description": "string",
  "documentSet" : { "@type": "microsoft.graph.documentSet" },
  "documentTemplate" : { "@type": "microsoft.graph.documentSetContent" },
  "group": "string",
  "hidden": false,
  "id": "string",
  "inheritedFrom": { "@type": "microsoft.graph.itemReference" },
  "isBuiltIn" : false,
  "name": "string",
  "order": { "@type": "microsoft.graph.contentTypeOrder" },
  "parentId": "string",
  "propagateChanges" : false,
  "readOnly": false,
  "sealed": false
}
```

[list]: list.md
[listItem]: listitem.md
<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ContentType",
  "suppressions": []
}
-->


