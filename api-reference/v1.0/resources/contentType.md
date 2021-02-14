---
author: daspek
ms.date: 09/12/2017
title: ContentType
localization_priority: Normal
description: O recurso contentType representa um tipo de conteúdo no SharePoint.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: f49ce9d1c656975ee02e6c1056015f7e033d57f9
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/14/2021
ms.locfileid: "50238558"
---
# <a name="contenttype-resource-type"></a>Tipo de recurso ContentType

Namespace: microsoft.graph

O recurso **contentType** representa um _tipo de conteúdo_ no SharePoint.
Tipos de conteúdo permitem definir um conjunto de colunas que devem estar presentes em cada [**listItem**][listItem] em uma [**lista.**][list]

[list]: list.md
[listItem]: listitem.md

## <a name="json-representation"></a>Representação JSON

Aqui está uma representação JSON de um recurso **contentType**.
<!-- {
  "blockType": "resource",
 "baseType": "microsoft.graph.entity",
 "@odata.type": "microsoft.graph.contentType" } -->

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

  "columnLinks": [{ "@type": "microsoft.graph.columnLink" }]
}
```

## <a name="properties"></a>Propriedades

| Nome da propriedade     | Tipo                 | Descrição
|:------------------|:---------------------|:----------------------------------
| **description**   | string               | O texto descritivo do item.
| **group**         | string               | O nome do grupo ao qual esse tipo de conteúdo pertence. Ajuda a organizar os tipos de conteúdo relacionados.
| **hidden**        | booliano              | Indica se o tipo de conteúdo está oculto no menu “Novo” da lista.
| **id**            | string               | O identificador exclusivo do tipo de conteúdo.
| **inheritedFrom** | [itemReference][]    | Se esse tipo de conteúdo for herdado de outro escopo (como um site), fornece uma referência para o item no qual o tipo de conteúdo foi definido.
| **name**          | string               | O nome do tipo de conteúdo.
| **order**         | [contentTypeOrder][] | Especifica a ordem na qual o tipo de conteúdo aparece na seleção da interface do usuário.
| **parentId**      | string               | O identificador exclusivo do tipo de conteúdo.
| **readOnly**      | booliano              | Se `true`, o tipo de conteúdo não pode ser modificado, a menos que esse valor seja definido primeiro como `false`.
| **sealed**        | booliano              | Se `true`, o tipo de conteúdo não pode ser modificado por usuários ou por operações de push-down. Somente administradores de conjunto de sites podem lacrar ou retirar o lacre dos tipos de conteúdo.

## <a name="relationships"></a>Relações

| Nome da propriedade   | Tipo                      | Descrição
|:----------------|:--------------------------|:-------------------------------
| **columnLinks** | Conjunto [columnLink][] | O conjunto de colunas necessário para este tipo de conteúdo

Consulte [Introdução a tipos de conteúdo e publicação de tipo de conteúdo][contentTypeIntro] para obter mais informações.

[columnLink]: columnlink.md
[contentTypeIntro]: https://support.office.com/en-us/article/Introduction-to-content-types-and-content-type-publishing-e1277a2e-a1e8-4473-9126-91a0647766e5
[itemReference]: itemreference.md
[contentTypeOrder]: contenttypeorder.md

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ContentType"
} -->

