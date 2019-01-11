---
author: daspek
ms.author: dspektor
ms.date: 09/12/2017
title: ColumnLink
localization_priority: Normal
ms.openlocfilehash: 435696cc596f73830104ea8ec0619bf40a462d62
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27834528"
---
# <a name="columnlink-resource-type"></a><span data-ttu-id="5517d-102">Tipo de recurso ColumnLink</span><span class="sxs-lookup"><span data-stu-id="5517d-102">ColumnLink resource type</span></span>

<span data-ttu-id="5517d-103">Um **columnLink** em um [contentType][] anexa um **columnDefinition** de site para esse tipo de conteúdo.</span><span class="sxs-lookup"><span data-stu-id="5517d-103">A **columnLink** on a [contentType][] attaches a site **columnDefinition** to that content type.</span></span>

[contentType]: contenttype.md

## <a name="json-representation"></a><span data-ttu-id="5517d-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5517d-105">JSON representation</span></span>

<span data-ttu-id="5517d-106">Aqui está uma representação JSON de um recurso **columnLink**.</span><span class="sxs-lookup"><span data-stu-id="5517d-106">Here is a JSON representation of a **columnLink** resource.</span></span>
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

## <a name="properties"></a><span data-ttu-id="5517d-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5517d-107">Properties</span></span>

| <span data-ttu-id="5517d-108">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="5517d-108">Property name</span></span> | <span data-ttu-id="5517d-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="5517d-109">Type</span></span>   | <span data-ttu-id="5517d-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="5517d-110">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="5517d-111">**id**</span><span class="sxs-lookup"><span data-stu-id="5517d-111">**id**</span></span>        | <span data-ttu-id="5517d-112">string</span><span class="sxs-lookup"><span data-stu-id="5517d-112">string</span></span> | <span data-ttu-id="5517d-113">O identificador exclusivo da coluna.</span><span class="sxs-lookup"><span data-stu-id="5517d-113">The unique identifier for the column.</span></span>
| <span data-ttu-id="5517d-114">**name**</span><span class="sxs-lookup"><span data-stu-id="5517d-114">**name**</span></span>      | <span data-ttu-id="5517d-115">string</span><span class="sxs-lookup"><span data-stu-id="5517d-115">string</span></span> | <span data-ttu-id="5517d-116">O nome da coluna desse tipo de conteúdo.</span><span class="sxs-lookup"><span data-stu-id="5517d-116">The name of the column  in this content type.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ColumnLink"
} -->
