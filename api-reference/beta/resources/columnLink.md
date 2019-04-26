---
author: daspek
ms.author: dspektor
ms.date: 09/12/2017
title: ColumnLink
localization_priority: Normal
ms.openlocfilehash: c6fc12dcfaeffcb3cd4fb08a6863611ae33541d5
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33341400"
---
# <a name="columnlink-resource-type"></a><span data-ttu-id="ae07a-102">Tipo de recurso ColumnLink</span><span class="sxs-lookup"><span data-stu-id="ae07a-102">ColumnLink resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ae07a-103">Um **columnLink** em um [contentType][] anexa um **columnDefinition** de site para esse tipo de conteúdo.</span><span class="sxs-lookup"><span data-stu-id="ae07a-103">A **columnLink** on a [contentType][] attaches a site **columnDefinition** to that content type.</span></span>

[contentType]: contenttype.md

## <a name="json-representation"></a><span data-ttu-id="ae07a-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ae07a-105">JSON representation</span></span>

<span data-ttu-id="ae07a-106">Aqui está uma representação JSON de um recurso **columnLink**.</span><span class="sxs-lookup"><span data-stu-id="ae07a-106">Here is a JSON representation of a **columnLink** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.columnLink" } -->

```json
{
  "id": "string",
  "name": "string"
}
```

## <a name="properties"></a><span data-ttu-id="ae07a-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ae07a-107">Properties</span></span>

| <span data-ttu-id="ae07a-108">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="ae07a-108">Property name</span></span> | <span data-ttu-id="ae07a-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="ae07a-109">Type</span></span>   | <span data-ttu-id="ae07a-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="ae07a-110">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="ae07a-111">**id**</span><span class="sxs-lookup"><span data-stu-id="ae07a-111">**id**</span></span>        | <span data-ttu-id="ae07a-112">string</span><span class="sxs-lookup"><span data-stu-id="ae07a-112">string</span></span> | <span data-ttu-id="ae07a-113">O identificador exclusivo da coluna.</span><span class="sxs-lookup"><span data-stu-id="ae07a-113">The unique identifier for the column.</span></span>
| <span data-ttu-id="ae07a-114">**name**</span><span class="sxs-lookup"><span data-stu-id="ae07a-114">**name**</span></span>      | <span data-ttu-id="ae07a-115">string</span><span class="sxs-lookup"><span data-stu-id="ae07a-115">string</span></span> | <span data-ttu-id="ae07a-116">O nome da coluna desse tipo de conteúdo.</span><span class="sxs-lookup"><span data-stu-id="ae07a-116">The name of the column  in this content type.</span></span>

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
