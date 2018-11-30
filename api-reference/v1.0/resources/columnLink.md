---
author: daspek
ms.author: dspektor
ms.date: 09/12/2017
title: ColumnLink
ms.openlocfilehash: a3eae28dcd9fef3ddfba9b39103bec31ff71c9da
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27003494"
---
# <a name="columnlink-resource-type"></a><span data-ttu-id="ac408-102">Tipo de recurso ColumnLink</span><span class="sxs-lookup"><span data-stu-id="ac408-102">ColumnLink resource type</span></span>

<span data-ttu-id="ac408-103">Um **columnLink** em um [contentType][] anexa um **columnDefinition** de site para esse tipo de conteúdo.</span><span class="sxs-lookup"><span data-stu-id="ac408-103">A **columnLink** on a [contentType][] attaches a site **columnDefinition** to that content type.</span></span>

[contentType]: contenttype.md

## <a name="json-representation"></a><span data-ttu-id="ac408-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ac408-105">JSON representation</span></span>

<span data-ttu-id="ac408-106">Aqui está uma representação JSON de um recurso **columnLink**.</span><span class="sxs-lookup"><span data-stu-id="ac408-106">Here is a JSON representation of a **columnLink** resource.</span></span>
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

## <a name="properties"></a><span data-ttu-id="ac408-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ac408-107">Properties</span></span>

| <span data-ttu-id="ac408-108">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="ac408-108">Property name</span></span> | <span data-ttu-id="ac408-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="ac408-109">Type</span></span>   | <span data-ttu-id="ac408-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="ac408-110">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="ac408-111">**id**</span><span class="sxs-lookup"><span data-stu-id="ac408-111">**id**</span></span>        | <span data-ttu-id="ac408-112">string</span><span class="sxs-lookup"><span data-stu-id="ac408-112">string</span></span> | <span data-ttu-id="ac408-113">O identificador exclusivo da coluna.</span><span class="sxs-lookup"><span data-stu-id="ac408-113">The unique identifier for the column.</span></span>
| <span data-ttu-id="ac408-114">**name**</span><span class="sxs-lookup"><span data-stu-id="ac408-114">**name**</span></span>      | <span data-ttu-id="ac408-115">string</span><span class="sxs-lookup"><span data-stu-id="ac408-115">string</span></span> | <span data-ttu-id="ac408-116">O nome da coluna desse tipo de conteúdo.</span><span class="sxs-lookup"><span data-stu-id="ac408-116">The name of the column  in this content type.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ColumnLink"
} -->
