---
author: daspek
description: Um columnLink em um contentType anexa um columnDefinition de site para esse tipo de conteúdo.
ms.date: 09/12/2017
title: ColumnLink
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: f60392954cb1a214327edd4ffcc65449c6d976f0
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48034060"
---
# <a name="columnlink-resource-type"></a><span data-ttu-id="3e637-103">Tipo de recurso ColumnLink</span><span class="sxs-lookup"><span data-stu-id="3e637-103">ColumnLink resource type</span></span>

<span data-ttu-id="3e637-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3e637-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3e637-105">Um **columnLink** em um [contentType][] anexa um **columnDefinition** de site para esse tipo de conteúdo.</span><span class="sxs-lookup"><span data-stu-id="3e637-105">A **columnLink** on a [contentType][] attaches a site **columnDefinition** to that content type.</span></span>

[contentType]: contenttype.md

## <a name="json-representation"></a><span data-ttu-id="3e637-107">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3e637-107">JSON representation</span></span>

<span data-ttu-id="3e637-108">Aqui está uma representação JSON de um recurso **columnLink**.</span><span class="sxs-lookup"><span data-stu-id="3e637-108">Here is a JSON representation of a **columnLink** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.columnLink" } -->

```json
{
  "id": "string",
  "name": "string"
}
```

## <a name="properties"></a><span data-ttu-id="3e637-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3e637-109">Properties</span></span>

| <span data-ttu-id="3e637-110">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="3e637-110">Property name</span></span> | <span data-ttu-id="3e637-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="3e637-111">Type</span></span>   | <span data-ttu-id="3e637-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="3e637-112">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="3e637-113">**id**</span><span class="sxs-lookup"><span data-stu-id="3e637-113">**id**</span></span>        | <span data-ttu-id="3e637-114">string</span><span class="sxs-lookup"><span data-stu-id="3e637-114">string</span></span> | <span data-ttu-id="3e637-115">O identificador exclusivo da coluna.</span><span class="sxs-lookup"><span data-stu-id="3e637-115">The unique identifier for the column.</span></span>
| <span data-ttu-id="3e637-116">**name**</span><span class="sxs-lookup"><span data-stu-id="3e637-116">**name**</span></span>      | <span data-ttu-id="3e637-117">string</span><span class="sxs-lookup"><span data-stu-id="3e637-117">string</span></span> | <span data-ttu-id="3e637-118">O nome da coluna desse tipo de conteúdo.</span><span class="sxs-lookup"><span data-stu-id="3e637-118">The name of the column  in this content type.</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ColumnLink",
  "suppressions": []
}
-->


