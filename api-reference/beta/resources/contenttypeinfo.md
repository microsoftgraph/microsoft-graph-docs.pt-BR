---
author: daspek
description: O recurso contentTypeInfo indica o tipo de conteúdo do SharePoint de um item.
ms.date: 09/12/2017
title: ContentTypeInfo
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 0aa9518f2b9597f910586ab49284dfe6f44a17ad
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507426"
---
# <a name="contenttypeinfo-resource-type"></a>Tipo de recurso ContentTypeInfo

Namespace: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

O recurso **contentTypeInfo** indica o tipo de conteúdo do SharePoint de um item.

## <a name="json-representation"></a>Representação JSON

Aqui está uma representação JSON de um recurso **contentTypeInfo**.
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.contentTypeInfo", "@type.aka": "oneDrive.contentTypeFacet" } -->

```json
{
  "id": "string",
  "name": "string"
}
```

## <a name="properties"></a>Propriedades

| Nome da propriedade  | Tipo    | Descrição
|:---------------|:--------|:--------------------------------------------------
| **id**         | cadeia de caracteres  | A id do tipo de conteúdo.
| **name**       | string  | O nome do tipo de conteúdo.

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ContentTypeInfo",
  "suppressions": []
}
-->
