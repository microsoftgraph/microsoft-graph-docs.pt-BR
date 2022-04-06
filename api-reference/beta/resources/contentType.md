---
author: daspek
description: O recurso contentType representa um tipo de conteúdo no SharePoint.
title: contentType
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: sites-and-lists
ms.openlocfilehash: c2136344ff14059cd93f8aa505b9c9f1af204f87
ms.sourcegitcommit: f5382652b6880fab42040df40a08de7cb2d74d35
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/17/2022
ms.locfileid: "63560047"
---
# <a name="contenttype-resource-type"></a>Tipo de recurso contentType

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um tipo de conteúdo SharePoint.
Os tipos de conteúdo permitem definir um conjunto de colunas que devem estar presentes em cada [**listItem**][listItem] em uma [**lista**][list].

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar contentTypes em um site](../api/site-list-contenttypes.md)|[coleção contentType](../resources/contenttype.md)|Obter uma lista dos [objetos contentType](../resources/contenttype.md) e suas propriedades em um [site](../resources/site.md).|
|[Listar contentTypes em uma lista](../api/list-list-contenttypes.md)|[coleção contentType](../resources/contenttype.md)|Obter uma lista dos [objetos contentType](../resources/contenttype.md) e suas propriedades em uma [lista](../resources/list.md).|
|[Criar contentType para um site](../api/site-post-contenttypes.md)|[contentType](../resources/contenttype.md)|Crie um novo [objeto contentType](../resources/contenttype.md) em um [site](../resources/site.md).|
|[Obter contentType](../api/contenttype-get.md)|[contentType](../resources/contenttype.md)|Leia as propriedades e as relações de um [objeto contentType](../resources/contenttype.md) .|
|[Atualizar contentType](../api/contenttype-update.md)|[contentType](../resources/contenttype.md)|Atualize as propriedades de um [objeto contentType](../resources/contenttype.md) .|
|[Excluir contentType](../api/contenttype-delete.md)|Nenhum|Exclui um [objeto contentType](../resources/contenttype.md) .|
|[isPublished](../api/contenttype-ispublished.md)|Booliano| Verifica se [o contentType](../resources/contenttype.md) foi publicado.|
|[publish](../api/contenttype-publish.md)|[contentType](../resources/contenttype.md)| Publicar um [contentType](../resources/contenttype.md).|
|[unpublish](../api/contenttype-unpublish.md)|[contentType](../resources/contenttype.md)|Não publice um [contentType](../resources/contenttype.md).|
|[addCopy](../api/contenttype-addcopy.md)|[contentType](../resources/contenttype.md)|Adicione uma cópia de [um contentType](../resources/contenttype.md) de um [site](../resources/site.md) a uma [lista](../resources/list.md)).|
|[associateWithHubSites](../api/contenttype-associatewithhubsites.md)|[contentType](../resources/contenttype.md)|Associa um [contentType](../resources/contenttype.md) a uma lista de hubsites.|
|[copyToDefaultContentLocation](../api/contenttype-copytodefaultcontentlocation.md)|[contentType](../resources/contenttype.md)| Copie um arquivo para o local de conteúdo padrão em [um contentType](../resources/contenttype.md).|
|[Colunas de lista](../api/contenttype-list-columns.md)|[coleção columnDefinition](../resources/columnDefinition.md)|Obter uma coleção de colunas, representadas como [recursos columnDefinition](../resources/columnDefinition.md) , em um **contentType**.|
|[Criar coluna](../api/contenttype-post-columns.md)|[columnDefinition](../resources/columnDefinition.md)|Adicione uma coluna a **um tipo de conteúdo** em um site ou lista.|
|[getCompatibleHubContentTypes](../api/contenttype-getcompatiblehubcontenttypes.md)|[coleção contentType](../resources/contenttype.md)| Recupere tipos de conteúdo publicados do hub de tipo de conteúdo que pode ser adicionado a um site ou uma lista.|
|[addCopyFromContentTypeHub](../api/contenttype-addcopyfromcontenttypehub.md)|[contentType](../resources/contenttype.md)| Adicione ou sincronize um tipo de conteúdo compatível do hub de tipo de conteúdo para um site ou uma lista.|

## <a name="properties"></a>Propriedades

| Propriedade          | Tipo                 | Descrição|
|:------------------|:---------------------|:----------------------------------|
|   associatedHubsUrls         | Collection(string) | Lista de URLs canônicas para sites de hub aos quais esse tipo de conteúdo está associado. Isso conterá todos os hubsites em que esse tipo de conteúdo está na fila para ser imposto ou já está imposto. Impor um tipo de conteúdo significa que o tipo de conteúdo será aplicado às listas nos sites imposto.|
|   documentSet         | [documentSet][]      | [Metadados do Conjunto](/sharepoint/governance/document-set-planning#about-document-sets) de Documentos.|
|   documentTemplate    | [documentSetContent][] | Metadados do modelo de documento. Para garantir que os documentos tenham conteúdo consistente em um site e seus subsites, você pode associar um modelo do Word, Excel ou PowerPoint a um tipo de conteúdo de site.|
|   description     | string               | O texto descritivo do item.|
|   group           | string               | O nome do grupo ao qual esse tipo de conteúdo pertence. Ajuda a organizar os tipos de conteúdo relacionados.|
|   hidden          | Booliano              | Indica se o tipo de conteúdo está oculto no menu “Novo” da lista.|
|   id              | cadeia de caracteres               | O identificador exclusivo do tipo de conteúdo.|
|   inheritedFrom   | [itemReference][]    | Se esse tipo de conteúdo for herdado de outro escopo (como um site), fornece uma referência para o item no qual o tipo de conteúdo foi definido.|
|   isBuiltIn              | Booliano| Especifica se um tipo de conteúdo é um tipo de conteúdo integrado. |
|   nome            | string               | O nome do tipo de conteúdo.|
|   order           | [contentTypeOrder][] | Especifica a ordem na qual o tipo de conteúdo aparece na seleção da interface do usuário.|
|   parentId        | string               | O identificador exclusivo do tipo de conteúdo.|
|   propagateChanges     | Booliano              | If `true`, any changes made to the content type will be pushed to inherited content types and lists that implement the content type.|
|   readOnly        | Booliano              | Se `true`, o tipo de conteúdo não pode ser modificado, a menos que esse valor seja definido primeiro como `false`.|
|   sealed          | Booliano              | Se `true`, o tipo de conteúdo não pode ser modificado por usuários ou por operações de push-down. Somente administradores de conjunto de sites podem lacrar ou retirar o lacre dos tipos de conteúdo.|


## <a name="relationships"></a>Relações

| Relação    | Tipo                      | Descrição|
|:----------------|:--------------------------|:-------------------------------|
|   base     | [contentType][]  | ContentType pai do qual esse tipo de conteúdo é derivado. |
|   columnLinks   | Conjunto [columnLink][] | O conjunto de colunas necessário para este tipo de conteúdo|
|   baseTypes     | Collection([contentType][])     | A coleção de tipos de conteúdo que são ancestrais desse tipo de conteúdo.|
|   columnPositions         | Collection([columnDefinition][]) | Informações de ordem de coluna em um tipo de conteúdo.|
|   columns       | Collection([columnDefinition][])  | A coleção de definições de coluna para este contentType.|

Para obter mais detalhes, consulte [Introdução a tipos de conteúdo e publicação de tipos de conteúdo][contentTypeIntro].

[columnLink]: columnlink.md
[contentTypeIntro]: https://support.office.com/article/Introduction-to-content-types-and-content-type-publishing-e1277a2e-a1e8-4473-9126-91a0647766e5
[itemReference]: itemreference.md
[contentTypeOrder]: contenttypeorder.md
[columnDefinition]: columnDefinition.md
[contentType]: contentType.md
[documentSet]: documentSet.md
[documentSetContent]: documentSetContent.md

## <a name="json-representation"></a>Representação JSON

A seguir está uma representação JSON de um recurso.

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
