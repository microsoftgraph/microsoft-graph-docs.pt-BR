---
author: daspek
ms.author: dspektor
ms.date: 09/12/2017
title: ColumnLink
localization_priority: Normal
ms.openlocfilehash: d5b1d068202057bc6a07982d04ff77b6bf07f028
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29511860"
---
# <a name="columnlink-resource-type"></a><span data-ttu-id="777cc-102">Tipo de recurso ColumnLink</span><span class="sxs-lookup"><span data-stu-id="777cc-102">ColumnLink resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="777cc-103">Um **columnLink** em um [contentType][] anexa um **columnDefinition** de site para esse tipo de conteúdo.</span><span class="sxs-lookup"><span data-stu-id="777cc-103">A **columnLink** on a [contentType][] attaches a site **columnDefinition** to that content type.</span></span>

[contentType]: contenttype.md

## <a name="json-representation"></a><span data-ttu-id="777cc-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="777cc-105">JSON representation</span></span>

<span data-ttu-id="777cc-106">Aqui está uma representação JSON de um recurso **columnLink**.</span><span class="sxs-lookup"><span data-stu-id="777cc-106">Here is a JSON representation of a **columnLink** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.columnLink" } -->

```json
{
  "id": "string",
  "name": "string"
}
```

## <a name="properties"></a><span data-ttu-id="777cc-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="777cc-107">Properties</span></span>

| <span data-ttu-id="777cc-108">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="777cc-108">Property name</span></span> | <span data-ttu-id="777cc-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="777cc-109">Type</span></span>   | <span data-ttu-id="777cc-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="777cc-110">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="777cc-111">**id**</span><span class="sxs-lookup"><span data-stu-id="777cc-111">**id**</span></span>        | <span data-ttu-id="777cc-112">string</span><span class="sxs-lookup"><span data-stu-id="777cc-112">string</span></span> | <span data-ttu-id="777cc-113">O identificador exclusivo da coluna.</span><span class="sxs-lookup"><span data-stu-id="777cc-113">The unique identifier for the column.</span></span>
| <span data-ttu-id="777cc-114">**name**</span><span class="sxs-lookup"><span data-stu-id="777cc-114">**name**</span></span>      | <span data-ttu-id="777cc-115">string</span><span class="sxs-lookup"><span data-stu-id="777cc-115">string</span></span> | <span data-ttu-id="777cc-116">O nome da coluna desse tipo de conteúdo.</span><span class="sxs-lookup"><span data-stu-id="777cc-116">The name of the column  in this content type.</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ColumnLink",
  "suppressions": [
    "Error: /api-reference/beta/resources/columnLink.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
