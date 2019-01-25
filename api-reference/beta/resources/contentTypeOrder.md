---
author: daspek
ms.author: dspektor
ms.date: 09/13/2017
title: ContentTypeOrder
localization_priority: Normal
ms.openlocfilehash: 9b92a8234c493ae9b0f396db7010e7bf717d5959
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29514366"
---
# <a name="contenttypeorder-resource-type"></a><span data-ttu-id="3ba2b-102">Tipo de recurso ContentTypeOrder</span><span class="sxs-lookup"><span data-stu-id="3ba2b-102">ContentTypeOrder resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3ba2b-103">O recurso **contentTypeOrder** especifica a ordem na qual o Content Type será exibido na seleção da interface do usuário.</span><span class="sxs-lookup"><span data-stu-id="3ba2b-103">The **contentTypeOrder** resource specifies in which order the Content Type will appear in the selection UI.</span></span>

## <a name="json-representation"></a><span data-ttu-id="3ba2b-104">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3ba2b-104">JSON representation</span></span>

<span data-ttu-id="3ba2b-105">Aqui está uma representação JSON de um recurso **contentTypeOrder**.</span><span class="sxs-lookup"><span data-stu-id="3ba2b-105">Here is a JSON representation of a **contentTypeOrder** resource.</span></span>
<!-- { "blockType": "resource", "@type": "microsoft.graph.contentTypeOrder", "@type.aka": "oneDrive.contentTypeOrderFacet" } -->

```json
{
  "default": true,
  "position": 2
}
```

## <a name="properties"></a><span data-ttu-id="3ba2b-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3ba2b-106">Properties</span></span>

| <span data-ttu-id="3ba2b-107">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="3ba2b-107">Property name</span></span> | <span data-ttu-id="3ba2b-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="3ba2b-108">Type</span></span>    | <span data-ttu-id="3ba2b-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="3ba2b-109">Description</span></span>
|:--------------|:--------|:----------------------------------------------------
| <span data-ttu-id="3ba2b-110">**default**</span><span class="sxs-lookup"><span data-stu-id="3ba2b-110">**default**</span></span>   | <span data-ttu-id="3ba2b-111">booliano</span><span class="sxs-lookup"><span data-stu-id="3ba2b-111">boolean</span></span> | <span data-ttu-id="3ba2b-112">Se esse é o Content Type padrão</span><span class="sxs-lookup"><span data-stu-id="3ba2b-112">Whether this is the default Content Type</span></span>
| <span data-ttu-id="3ba2b-113">**position**</span><span class="sxs-lookup"><span data-stu-id="3ba2b-113">**position**</span></span>  | <span data-ttu-id="3ba2b-114">Int32</span><span class="sxs-lookup"><span data-stu-id="3ba2b-114">Int32</span></span>   | <span data-ttu-id="3ba2b-115">Especifica a posição em que o tipo de conteúdo aparece na seleção da interface do usuário.</span><span class="sxs-lookup"><span data-stu-id="3ba2b-115">Specifies the position in which the Content Type appears in the selection UI.</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ContentTypeOrder",
  "suppressions": [
    "Error: /api-reference/beta/resources/contentTypeOrder.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
