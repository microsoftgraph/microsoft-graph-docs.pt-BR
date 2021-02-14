---
author: daspek
ms.date: 09/12/2017
title: ColumnLink
localization_priority: Normal
description: Um columnLink em um contentType anexa um columnDefinition de site para esse tipo de conteúdo.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 4087d97dfec976560bac7c8949d34fd962308950
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/14/2021
ms.locfileid: "50240574"
---
# <a name="columnlink-resource-type"></a><span data-ttu-id="47cd7-103">Tipo de recurso ColumnLink</span><span class="sxs-lookup"><span data-stu-id="47cd7-103">ColumnLink resource type</span></span>

<span data-ttu-id="47cd7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="47cd7-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="47cd7-105">Um **columnLink** em um [contentType][] anexa um **columnDefinition** de site para esse tipo de conteúdo.</span><span class="sxs-lookup"><span data-stu-id="47cd7-105">A **columnLink** on a [contentType][] attaches a site **columnDefinition** to that content type.</span></span>

[contentType]: contenttype.md

## <a name="json-representation"></a><span data-ttu-id="47cd7-107">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="47cd7-107">JSON representation</span></span>

<span data-ttu-id="47cd7-108">Aqui está uma representação JSON de um recurso **columnLink**.</span><span class="sxs-lookup"><span data-stu-id="47cd7-108">Here is a JSON representation of a **columnLink** resource.</span></span>
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

## <a name="properties"></a><span data-ttu-id="47cd7-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="47cd7-109">Properties</span></span>

| <span data-ttu-id="47cd7-110">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="47cd7-110">Property name</span></span> | <span data-ttu-id="47cd7-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="47cd7-111">Type</span></span>   | <span data-ttu-id="47cd7-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="47cd7-112">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="47cd7-113">**id**</span><span class="sxs-lookup"><span data-stu-id="47cd7-113">**id**</span></span>        | <span data-ttu-id="47cd7-114">string</span><span class="sxs-lookup"><span data-stu-id="47cd7-114">string</span></span> | <span data-ttu-id="47cd7-115">O identificador exclusivo da coluna.</span><span class="sxs-lookup"><span data-stu-id="47cd7-115">The unique identifier for the column.</span></span>
| <span data-ttu-id="47cd7-116">**name**</span><span class="sxs-lookup"><span data-stu-id="47cd7-116">**name**</span></span>      | <span data-ttu-id="47cd7-117">string</span><span class="sxs-lookup"><span data-stu-id="47cd7-117">string</span></span> | <span data-ttu-id="47cd7-118">O nome da coluna desse tipo de conteúdo.</span><span class="sxs-lookup"><span data-stu-id="47cd7-118">The name of the column  in this content type.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ColumnLink"
} -->

