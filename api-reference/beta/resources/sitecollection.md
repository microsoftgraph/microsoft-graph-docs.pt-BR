---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: SiteCollection
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 7fb11fc9dc2f55b853ec512255ffa06f8a53cef6
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27933670"
---
# <a name="sitecollection-resource"></a>Recurso SiteCollection

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

O recurso **siteCollection** fornece mais informações sobre um conjunto de sites.

Se um recurso [**site**](site.md) tem uma propriedade **siteCollection** não nula e, em seguida, o site é um site raiz do conjunto de sites.

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "dataLocationCode", "root"
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
| **root**             | [root][] | Se presente, indica que este é um conjunto de sites raiz no SharePoint. Somente leitura.

[root]: root.md

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
