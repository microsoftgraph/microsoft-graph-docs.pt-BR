---
author: daspek
ms.author: dspektor
ms.date: 09/12/2017
title: ColumnLink
localization_priority: Normal
ms.openlocfilehash: 226666875b9364f33954e7f932227562a9734267
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27888568"
---
# <a name="columnlink-resource-type"></a><span data-ttu-id="5206a-102">Tipo de recurso ColumnLink</span><span class="sxs-lookup"><span data-stu-id="5206a-102">ColumnLink resource type</span></span>

> <span data-ttu-id="5206a-103">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="5206a-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5206a-104">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="5206a-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5206a-105">Um **columnLink** em um [contentType][] anexa um **columnDefinition** de site para esse tipo de conteúdo.</span><span class="sxs-lookup"><span data-stu-id="5206a-105">A **columnLink** on a [contentType][] attaches a site **columnDefinition** to that content type.</span></span>

[contentType]: contenttype.md

## <a name="json-representation"></a><span data-ttu-id="5206a-107">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5206a-107">JSON representation</span></span>

<span data-ttu-id="5206a-108">Aqui está uma representação JSON de um recurso **columnLink**.</span><span class="sxs-lookup"><span data-stu-id="5206a-108">Here is a JSON representation of a **columnLink** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.columnLink" } -->

```json
{
  "id": "string",
  "name": "string"
}
```

## <a name="properties"></a><span data-ttu-id="5206a-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5206a-109">Properties</span></span>

| <span data-ttu-id="5206a-110">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="5206a-110">Property name</span></span> | <span data-ttu-id="5206a-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="5206a-111">Type</span></span>   | <span data-ttu-id="5206a-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="5206a-112">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="5206a-113">**id**</span><span class="sxs-lookup"><span data-stu-id="5206a-113">**id**</span></span>        | <span data-ttu-id="5206a-114">string</span><span class="sxs-lookup"><span data-stu-id="5206a-114">string</span></span> | <span data-ttu-id="5206a-115">O identificador exclusivo da coluna.</span><span class="sxs-lookup"><span data-stu-id="5206a-115">The unique identifier for the column.</span></span>
| <span data-ttu-id="5206a-116">**name**</span><span class="sxs-lookup"><span data-stu-id="5206a-116">**name**</span></span>      | <span data-ttu-id="5206a-117">string</span><span class="sxs-lookup"><span data-stu-id="5206a-117">string</span></span> | <span data-ttu-id="5206a-118">O nome da coluna desse tipo de conteúdo.</span><span class="sxs-lookup"><span data-stu-id="5206a-118">The name of the column  in this content type.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ColumnLink"
} -->
