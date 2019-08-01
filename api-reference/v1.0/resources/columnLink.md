---
author: daspek
ms.author: dspektor
ms.date: 09/12/2017
title: ColumnLink
localization_priority: Normal
description: Um columnLink em um contentType anexa um columnDefinition de site para esse tipo de conteúdo.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: d3914c4b3cfe18d2dead778116b86134caaf6caa
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36029691"
---
# <a name="columnlink-resource-type"></a><span data-ttu-id="5abe6-103">Tipo de recurso ColumnLink</span><span class="sxs-lookup"><span data-stu-id="5abe6-103">ColumnLink resource type</span></span>

<span data-ttu-id="5abe6-104">Um **columnLink** em um [contentType][] anexa um **columnDefinition** de site para esse tipo de conteúdo.</span><span class="sxs-lookup"><span data-stu-id="5abe6-104">A **columnLink** on a [contentType][] attaches a site **columnDefinition** to that content type.</span></span>

[contentType]: contenttype.md

## <a name="json-representation"></a><span data-ttu-id="5abe6-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5abe6-106">JSON representation</span></span>

<span data-ttu-id="5abe6-107">Aqui está uma representação JSON de um recurso **columnLink**.</span><span class="sxs-lookup"><span data-stu-id="5abe6-107">Here is a JSON representation of a **columnLink** resource.</span></span>
<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.columnLink" } -->

```json
{
  "id": "string",
  "name": "string"
}
```

## <a name="properties"></a><span data-ttu-id="5abe6-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5abe6-108">Properties</span></span>

| <span data-ttu-id="5abe6-109">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="5abe6-109">Property name</span></span> | <span data-ttu-id="5abe6-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="5abe6-110">Type</span></span>   | <span data-ttu-id="5abe6-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="5abe6-111">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="5abe6-112">**id**</span><span class="sxs-lookup"><span data-stu-id="5abe6-112">**id**</span></span>        | <span data-ttu-id="5abe6-113">string</span><span class="sxs-lookup"><span data-stu-id="5abe6-113">string</span></span> | <span data-ttu-id="5abe6-114">O identificador exclusivo da coluna.</span><span class="sxs-lookup"><span data-stu-id="5abe6-114">The unique identifier for the column.</span></span>
| <span data-ttu-id="5abe6-115">**name**</span><span class="sxs-lookup"><span data-stu-id="5abe6-115">**name**</span></span>      | <span data-ttu-id="5abe6-116">string</span><span class="sxs-lookup"><span data-stu-id="5abe6-116">string</span></span> | <span data-ttu-id="5abe6-117">O nome da coluna desse tipo de conteúdo.</span><span class="sxs-lookup"><span data-stu-id="5abe6-117">The name of the column  in this content type.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ColumnLink"
} -->
