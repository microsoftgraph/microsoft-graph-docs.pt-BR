---
author: daspek
ms.author: dspektor
ms.date: 09/12/2017
title: ColumnLink
localization_priority: Normal
description: Um columnLink em um contentType anexa um columnDefinition de site para esse tipo de conteúdo.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: fe17c5baf13e24800f28af1895561d55f3bf66cd
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42531810"
---
# <a name="columnlink-resource-type"></a><span data-ttu-id="49f66-103">Tipo de recurso ColumnLink</span><span class="sxs-lookup"><span data-stu-id="49f66-103">ColumnLink resource type</span></span>

<span data-ttu-id="49f66-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="49f66-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="49f66-105">Um **columnLink** em um [contentType][] anexa um **columnDefinition** de site para esse tipo de conteúdo.</span><span class="sxs-lookup"><span data-stu-id="49f66-105">A **columnLink** on a [contentType][] attaches a site **columnDefinition** to that content type.</span></span>

[contentType]: contenttype.md

## <a name="json-representation"></a><span data-ttu-id="49f66-107">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="49f66-107">JSON representation</span></span>

<span data-ttu-id="49f66-108">Aqui está uma representação JSON de um recurso **columnLink**.</span><span class="sxs-lookup"><span data-stu-id="49f66-108">Here is a JSON representation of a **columnLink** resource.</span></span>
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

## <a name="properties"></a><span data-ttu-id="49f66-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="49f66-109">Properties</span></span>

| <span data-ttu-id="49f66-110">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="49f66-110">Property name</span></span> | <span data-ttu-id="49f66-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="49f66-111">Type</span></span>   | <span data-ttu-id="49f66-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="49f66-112">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="49f66-113">**id**</span><span class="sxs-lookup"><span data-stu-id="49f66-113">**id**</span></span>        | <span data-ttu-id="49f66-114">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="49f66-114">string</span></span> | <span data-ttu-id="49f66-115">O identificador exclusivo da coluna.</span><span class="sxs-lookup"><span data-stu-id="49f66-115">The unique identifier for the column.</span></span>
| <span data-ttu-id="49f66-116">**name**</span><span class="sxs-lookup"><span data-stu-id="49f66-116">**name**</span></span>      | <span data-ttu-id="49f66-117">string</span><span class="sxs-lookup"><span data-stu-id="49f66-117">string</span></span> | <span data-ttu-id="49f66-118">O nome da coluna desse tipo de conteúdo.</span><span class="sxs-lookup"><span data-stu-id="49f66-118">The name of the column  in this content type.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ColumnLink"
} -->
