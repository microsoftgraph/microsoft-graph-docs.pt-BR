---
title: tipo de recurso personDataSource
description: Representa as fontes das quais os dados do usuário vêm, como contatos do Active Directory e do Outlook.
localization_priority: Normal
author: simonhult
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 80c7ec18094af2cd84671e095515566bfc52a10e
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35966109"
---
# <a name="persondatasource-resource-type"></a>tipo de recurso personDataSource

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa as fontes das quais os dados do usuário vêm, como contatos do Active Directory e do Outlook.

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.personDataSource"
}-->

```json
{
  "type": "string"
}

```
## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|type|String|O tipo de fonte de dados.|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "personDataSource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
