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
# <a name="persondatasource-resource-type"></a><span data-ttu-id="293d3-103">tipo de recurso personDataSource</span><span class="sxs-lookup"><span data-stu-id="293d3-103">personDataSource resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="293d3-104">Representa as fontes das quais os dados do usuário vêm, como contatos do Active Directory e do Outlook.</span><span class="sxs-lookup"><span data-stu-id="293d3-104">Represents the sources the user data comes from, such as Directory and Outlook Contacts.</span></span>

## <a name="json-representation"></a><span data-ttu-id="293d3-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="293d3-105">JSON representation</span></span>

<span data-ttu-id="293d3-106">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="293d3-106">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="293d3-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="293d3-107">Properties</span></span>
| <span data-ttu-id="293d3-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="293d3-108">Property</span></span>     | <span data-ttu-id="293d3-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="293d3-109">Type</span></span>   |<span data-ttu-id="293d3-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="293d3-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="293d3-111">type</span><span class="sxs-lookup"><span data-stu-id="293d3-111">type</span></span>|<span data-ttu-id="293d3-112">String</span><span class="sxs-lookup"><span data-stu-id="293d3-112">String</span></span>|<span data-ttu-id="293d3-113">O tipo de fonte de dados.</span><span class="sxs-lookup"><span data-stu-id="293d3-113">The type of data source.</span></span>|

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
