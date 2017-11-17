---
author: daspek
ms.author: dspektor
ms.date: 09/12/2017
title: ColumnLink
ms.openlocfilehash: ef7fef6fb6ca35f1117433b452de0841691282a0
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/28/2017
---
# <a name="columnlink-resource-type"></a><span data-ttu-id="55a9c-102">Tipo de recurso ColumnLink</span><span class="sxs-lookup"><span data-stu-id="55a9c-102">ColumnLink resource type</span></span>

<span data-ttu-id="55a9c-103">Um **columnLink** em um [contentType][] anexa um **columnDefinition** de site para esse tipo de conteúdo.</span><span class="sxs-lookup"><span data-stu-id="55a9c-103">A **columnLink** on a [contentType][] attaches a site **columnDefinition** to that content type.</span></span>

[contentType]: contentType.md

## <a name="json-representation"></a><span data-ttu-id="55a9c-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="55a9c-105">JSON representation</span></span>

<span data-ttu-id="55a9c-106">Aqui está uma representação JSON de um recurso **columnLink**.</span><span class="sxs-lookup"><span data-stu-id="55a9c-106">Here is a JSON representation of a **baseItem** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.columnLink" } -->

```json
{
  "id": "string",
  "name": "string"
}
```

## <a name="properties"></a><span data-ttu-id="55a9c-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="55a9c-107">Properties</span></span>

| <span data-ttu-id="55a9c-108">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="55a9c-108">Property name</span></span> | <span data-ttu-id="55a9c-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="55a9c-109">Type</span></span>   | <span data-ttu-id="55a9c-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="55a9c-110">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="55a9c-111">**id**</span><span class="sxs-lookup"><span data-stu-id="55a9c-111">**id**</span></span>        | <span data-ttu-id="55a9c-112">string</span><span class="sxs-lookup"><span data-stu-id="55a9c-112">string</span></span> | <span data-ttu-id="55a9c-113">O identificador exclusivo da coluna.</span><span class="sxs-lookup"><span data-stu-id="55a9c-113">The unique identifier for the column.</span></span>
| <span data-ttu-id="55a9c-114">**name**</span><span class="sxs-lookup"><span data-stu-id="55a9c-114">**name**</span></span>      | <span data-ttu-id="55a9c-115">string</span><span class="sxs-lookup"><span data-stu-id="55a9c-115">string</span></span> | <span data-ttu-id="55a9c-116">O nome da coluna desse tipo de conteúdo.</span><span class="sxs-lookup"><span data-stu-id="55a9c-116">The name of the column  in this content type.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ColumnLink"
} -->
