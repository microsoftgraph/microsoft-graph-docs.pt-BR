---
author: JeremyKelley
ms.date: 09/10/2017
title: SiteCollection
localization_priority: Normal
ms.prod: sharepoint
description: O recurso siteCollection fornece mais informações sobre um conjunto de sites.
doc_type: resourcePageType
ms.openlocfilehash: 196958674462095b8b47f82d07ac4fa7a885243b240473444c30b24014578c18
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54251740"
---
# <a name="sitecollection-resource"></a>Recurso SiteCollection

Namespace: microsoft.graph

O recurso **siteCollection** fornece mais informações sobre um conjunto de sites.

Se um recurso [**site**](site.md) tem uma propriedade **siteCollection** não nula e, em seguida, o site é um site raiz do conjunto de sites.

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
  ],
  "@odata.type": "microsoft.graph.siteCollection"
}-->

```json
{
  "hostname": "contoso.sharepoint.com",
  "dataLocationCode": "EUR",
  "root": { "@odata.type": "microsoft.graph.root" }
}
```

## <a name="properties"></a>Propriedades

| Nome da propriedade        | Tipo     | Descrição
|:---------------------|:---------|:---------------------------------------------------
| **hostname**         | string   | O nome do host do conjunto de sites. Somente leitura.
| **dataLocationCode** | string   | O código de região geográfica para onde esse conjunto de sites reside. Somente leitura.
| **root**             | [root][] | Se presente, indica que esse é um conjunto de sites raiz no SharePoint. Somente leitura.

[root]: root.md

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath&quot;: &quot;Facets/SiteCollection"
}-->

