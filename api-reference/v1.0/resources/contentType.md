---
author: daspek
ms.author: dspektor
ms.date: 09/12/2017
title: ContentType
ms.openlocfilehash: cb16559aa9da3a885be1977bbd1466265d0a72f0
ms.sourcegitcommit: abf4b739257e3ffd9d045f783ec595d846172590
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/21/2018
ms.locfileid: "23268330"
---
# <a name="contenttype-resource-type"></a>Tipo de recurso ContentType

O recurso **contentType** representa um _tipo de conteúdo_ no SharePoint.
Os tipos de conteúdo permitem definir um conjunto de colunas que devem estar presentes em cada [**listItem**][listItem] em uma [**lista**][list].

[list]: list.md
[listItem]: listItem.md

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
| **description**   | sequência de caracteres               | O texto descritivo do item.
| **group**         | sequência de caracteres               | O nome do grupo ao qual esse tipo de conteúdo pertence. Ajuda a organizar os tipos de conteúdo relacionados.
| **hidden**        | booliano              | Indica se o tipo de conteúdo está oculto no menu “Novo” da lista.
| **id**            | sequência de caracteres               | O identificador exclusivo do tipo de conteúdo.
| **inheritedFrom** | [itemReference][]    | Se esse tipo de conteúdo for herdado de outro escopo (como um site), fornece uma referência para o item no qual o tipo de conteúdo foi definido.
| **name**          | sequência de caracteres               | O nome do tipo de conteúdo.
| **order**         | [contentTypeOrder][] | Especifica a ordem na qual o tipo de conteúdo aparece na seleção da interface do usuário.
| **parentId**      | sequência de caracteres               | O identificador exclusivo do tipo de conteúdo.
| **readOnly**      | booliano              | Se `true`, o tipo de conteúdo não pode ser modificado, a menos que esse valor seja definido primeiro como `false`.
| **sealed**        | booliano              | Se `true`, o tipo de conteúdo não pode ser modificado por usuários ou por operações de push-down. Somente administradores de conjunto de sites podem lacrar ou retirar o lacre dos tipos de conteúdo.

## <a name="relationships"></a>Relações

| Nome da propriedade   | Tipo                      | Descrição
|:----------------|:--------------------------|:-------------------------------
| **columnLinks** | Conjunto [columnLink][] | O conjunto de colunas necessário para este tipo de conteúdo

Consulte [Introdução a tipos de conteúdo e publicação de tipo de conteúdo][contentTypeIntro] para obter mais informações.

[columnLink]: columnLink.md
[contentTypeIntro]: https://support.office.com/en-us/article/Introduction-to-content-types-and-content-type-publishing-e1277a2e-a1e8-4473-9126-91a0647766e5
[itemReference]: itemReference.md
[contentTypeOrder]: contentTypeOrder.md

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ContentType"
} -->
