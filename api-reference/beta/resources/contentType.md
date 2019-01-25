---
author: daspek
ms.author: dspektor
ms.date: 09/12/2017
title: ContentType
localization_priority: Normal
ms.openlocfilehash: c90dd8889d07f903a7d3c79d9e4e5db3b9f2a30b
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29522970"
---
# <a name="contenttype-resource-type"></a>Tipo de recurso ContentType

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

O recurso **contentType** representa um _tipo de conteúdo_ no SharePoint.
Os tipos de conteúdo permitem definir um conjunto de colunas que devem estar presentes em cada [**listItem**][listItem] em uma [**lista**][list].

[list]: list.md
[listItem]: listitem.md

## <a name="json-representation"></a>Representação JSON

Aqui está uma representação JSON de um recurso **contentType**.
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.contentType" } -->

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

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ContentType",
  "suppressions": [
    "Error: /api-reference/beta/resources/contentType.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
