---
author: daspek
description: O recurso contentType representa um tipo de conteúdo no SharePoint.
title: contentType
localization_priority: Normal
doc_type: resourcePageType
ms.prod: sites-and-lists
ms.openlocfilehash: 2af8291f33f62517e33349fb66408131f576e89a
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50444291"
---
# <a name="contenttype-resource-type"></a>Tipo de recurso contentType

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um _tipo de conteúdo_ no SharePoint.
Os tipos de conteúdo permitem definir um conjunto de colunas que devem estar presentes em cada [**listItem**][listItem] em uma [**lista**][list].

## <a name="properties"></a>Propriedades

| Nome da propriedade     | Tipo                 | Descrição
|:------------------|:---------------------|:----------------------------------
| **description**   | string               | O texto descritivo do item.
| **group**         | string               | O nome do grupo ao qual esse tipo de conteúdo pertence. Ajuda a organizar os tipos de conteúdo relacionados.
| **hidden**        | Booliano              | Indica se o tipo de conteúdo está oculto no menu “Novo” da lista.
| **id**            | string               | O identificador exclusivo do tipo de conteúdo.
| **inheritedFrom** | [itemReference][]    | Se esse tipo de conteúdo for herdado de outro escopo (como um site), fornece uma referência para o item no qual o tipo de conteúdo foi definido.
| **name**          | string               | O nome do tipo de conteúdo.
| **order**         | [contentTypeOrder][] | Especifica a ordem na qual o tipo de conteúdo aparece na seleção da interface do usuário.
| **parentId**      | string               | O identificador exclusivo do tipo de conteúdo.
| **readOnly**      | Booliano              | Se `true`, o tipo de conteúdo não pode ser modificado, a menos que esse valor seja definido primeiro como `false`.
| **sealed**        | Booliano              | Se `true`, o tipo de conteúdo não pode ser modificado por usuários ou por operações de push-down. Somente administradores de conjunto de sites podem lacrar ou retirar o lacre dos tipos de conteúdo.
| **isBuiltIn**            | Booliano| Especifica se um tipo de conteúdo é um tipo de conteúdo integrado. 
| **documentSet**       | [documentSet][]      | [Metadados do Conjunto](https://docs.microsoft.com/sharepoint/governance/document-set-planning#about-document-sets) de Documentos.
| **documentTemplate**  | [documentSetContent][] | Metadados do modelo de documento. Para garantir que os documentos tenham conteúdo consistente em um site e seus subsites, você pode associar um modelo do Word, Excel ou PowerPoint a um tipo de conteúdo de site.
| **associatedHubsUrls**       | Collection(string) | Lista de URLs canônicas para sites de hub aos quais esse tipo de conteúdo está associado. Isso conterá todos os hubsites em que esse tipo de conteúdo está na fila para ser imposto ou já está imposto. Impor um tipo de conteúdo significa que o tipo de conteúdo será aplicado às listas nos sites imposto.
| **propagateChanges**   | Booliano              | If `true` , any changes made to the content type will be pushed to inherited content types and lists that implement the content type.



## <a name="relationships"></a>Relações

| Nome da propriedade   | Tipo                      | Descrição
|:----------------|:--------------------------|:-------------------------------
| **base**   | [contentType][]  | ContentType pai do qual esse tipo de conteúdo é derivado. 
| **columnLinks** | Conjunto [columnLink][] | O conjunto de colunas necessário para este tipo de conteúdo
| **baseTypes**   | Collection([contentType][])     | A coleção de tipos de conteúdo que são ancestrais desse tipo de conteúdo.
| **columnPositions**       | Collection([columnDefinition][]) | Informações de ordem de coluna em um tipo de conteúdo.
| **columns**     | Collection([columnDefinition][])  | A coleção de definições de coluna para este contentType.

Consulte [Introdução a tipos de conteúdo e publicação de tipo de conteúdo][contentTypeIntro] para obter mais informações.

[columnLink]: columnlink.md
[contentTypeIntro]: https://support.office.com/en-us/article/Introduction-to-content-types-and-content-type-publishing-e1277a2e-a1e8-4473-9126-91a0647766e5
[itemReference]: itemreference.md
[contentTypeOrder]: contenttypeorder.md
[columnDefinition]: columnDefinition.md
[contentType]: contentType.md
[documentSet]: documentSet.md
[documentSetContent]: documentSetContent.md

## <a name="json-representation"></a>Representação JSON

A seguir está uma representação JSON de um **recurso contentType.**

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.contentType","keyProperty":"id" } -->

```json
{
  "description": "string",
  "group": "string",
  "hidden": false,
  "id": "string",
  "inheritedFrom": { "@type": "microsoft.graph.itemReference" },
  "name": "string",
  "order": { "@type": "microsoft.graph.contentTypeOrder" },
  "parentId": "string",
  "readOnly": false,
  "sealed": false,
  "columnLinks": [{ "@type": "microsoft.graph.columnLink" }],
  "base": { "@type": "microsoft.graph.contentType" },
  "columnPositions" : [{ "@type": "microsoft.graph.columnDefinition" }],
  "isBuiltIn" : false,
  "documentSet" : { "@type": "microsoft.graph.documentSet" },
  "documentTemplate" : { "@type": "microsoft.graph.documentSetContent" },
  "associatedHubsUrls" : ["string"],
  "propagateChanges" : false,
  "baseTypes" : [{ "@type": "microsoft.graph.contentType" }],
  "columns" : [{ "@type": "microsoft.graph.columnDefinition" }]
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


