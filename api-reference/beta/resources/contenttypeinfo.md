---
author: daspek
ms.author: dspektor
ms.date: 09/12/2017
title: ContentTypeInfo
localization_priority: Normal
ms.openlocfilehash: 107dfb3577489521d2e10e0c8fd2fe52c4f90b10
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33341219"
---
# <a name="contenttypeinfo-resource-type"></a><span data-ttu-id="f3bf8-102">Tipo de recurso ContentTypeInfo</span><span class="sxs-lookup"><span data-stu-id="f3bf8-102">ContentTypeInfo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f3bf8-103">O recurso **contentTypeInfo** indica o tipo de conteúdo do SharePoint de um item.</span><span class="sxs-lookup"><span data-stu-id="f3bf8-103">The **contentTypeInfo** resource indicates the SharePoint content type of an item.</span></span>

## <a name="json-representation"></a><span data-ttu-id="f3bf8-104">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f3bf8-104">JSON representation</span></span>

<span data-ttu-id="f3bf8-105">Aqui está uma representação JSON de um recurso **contentTypeInfo**.</span><span class="sxs-lookup"><span data-stu-id="f3bf8-105">Here is a JSON representation of a **contentTypeInfo** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.contentTypeInfo", "@type.aka": "oneDrive.contentTypeFacet" } -->

```json
{
  "id": "string",
  "name": "string"
}
```

## <a name="properties"></a><span data-ttu-id="f3bf8-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f3bf8-106">Properties</span></span>

| <span data-ttu-id="f3bf8-107">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="f3bf8-107">Property name</span></span>  | <span data-ttu-id="f3bf8-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="f3bf8-108">Type</span></span>    | <span data-ttu-id="f3bf8-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="f3bf8-109">Description</span></span>
|:---------------|:--------|:--------------------------------------------------
| <span data-ttu-id="f3bf8-110">**id**</span><span class="sxs-lookup"><span data-stu-id="f3bf8-110">**id**</span></span>         | <span data-ttu-id="f3bf8-111">string</span><span class="sxs-lookup"><span data-stu-id="f3bf8-111">string</span></span>  | <span data-ttu-id="f3bf8-112">A id do tipo de conteúdo.</span><span class="sxs-lookup"><span data-stu-id="f3bf8-112">The id of the content type.</span></span>
| <span data-ttu-id="f3bf8-113">**name**</span><span class="sxs-lookup"><span data-stu-id="f3bf8-113">**name**</span></span>       | <span data-ttu-id="f3bf8-114">string</span><span class="sxs-lookup"><span data-stu-id="f3bf8-114">string</span></span>  | <span data-ttu-id="f3bf8-115">O nome do tipo de conteúdo.</span><span class="sxs-lookup"><span data-stu-id="f3bf8-115">The name of the content type.</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ContentTypeInfo",
  "suppressions": []
}
-->
