---
author: daspek
ms.author: dspektor
ms.date: 09/12/2017
title: ContentTypeInfo
localization_priority: Normal
ms.openlocfilehash: 196a71be06b4e3c02330aba21559341650caa550
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29530059"
---
# <a name="contenttypeinfo-resource-type"></a><span data-ttu-id="44513-102">Tipo de recurso ContentTypeInfo</span><span class="sxs-lookup"><span data-stu-id="44513-102">ContentTypeInfo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="44513-103">O recurso **contentTypeInfo** indica o tipo de conteúdo do SharePoint de um item.</span><span class="sxs-lookup"><span data-stu-id="44513-103">The **contentTypeInfo** resource indicates the SharePoint content type of an item.</span></span>

## <a name="json-representation"></a><span data-ttu-id="44513-104">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="44513-104">JSON representation</span></span>

<span data-ttu-id="44513-105">Aqui está uma representação JSON de um recurso **contentTypeInfo**.</span><span class="sxs-lookup"><span data-stu-id="44513-105">Here is a JSON representation of a **contentTypeInfo** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.contentTypeInfo", "@type.aka": "oneDrive.contentTypeFacet" } -->

```json
{
  "id": "string",
  "name": "string"
}
```

## <a name="properties"></a><span data-ttu-id="44513-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="44513-106">Properties</span></span>

| <span data-ttu-id="44513-107">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="44513-107">Property name</span></span>  | <span data-ttu-id="44513-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="44513-108">Type</span></span>    | <span data-ttu-id="44513-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="44513-109">Description</span></span>
|:---------------|:--------|:--------------------------------------------------
| <span data-ttu-id="44513-110">**id**</span><span class="sxs-lookup"><span data-stu-id="44513-110">**id**</span></span>         | <span data-ttu-id="44513-111">string</span><span class="sxs-lookup"><span data-stu-id="44513-111">string</span></span>  | <span data-ttu-id="44513-112">A id do tipo de conteúdo.</span><span class="sxs-lookup"><span data-stu-id="44513-112">The id of the content type.</span></span>
| <span data-ttu-id="44513-113">**name**</span><span class="sxs-lookup"><span data-stu-id="44513-113">**name**</span></span>       | <span data-ttu-id="44513-114">string</span><span class="sxs-lookup"><span data-stu-id="44513-114">string</span></span>  | <span data-ttu-id="44513-115">O nome do tipo de conteúdo.</span><span class="sxs-lookup"><span data-stu-id="44513-115">The name of the content type.</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ContentTypeInfo",
  "suppressions": [
    "Error: /api-reference/beta/resources/contenttypeinfo.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
