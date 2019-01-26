---
title: insightIdentity
description: Tipo complexo que contém as propriedades de itens compartilhados.
author: simonhult
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: 47283a82260d4f03a271a16660d58aca60da94e1
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2019
ms.locfileid: "29577219"
---
# <a name="insightidentity"></a><span data-ttu-id="bea2a-103">insightIdentity</span><span class="sxs-lookup"><span data-stu-id="bea2a-103">insightIdentity</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bea2a-104">Tipo complexo que contém as propriedades de itens [compartilhados](insights-shared.md) .</span><span class="sxs-lookup"><span data-stu-id="bea2a-104">Complex type containing properties of [Shared](insights-shared.md) items.</span></span> 

## <a name="json-representation"></a><span data-ttu-id="bea2a-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="bea2a-105">JSON representation</span></span>
<span data-ttu-id="bea2a-106">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="bea2a-106">Here is a JSON representation of the resource</span></span>
<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "attachments",
    "singleValueLegacyExtendedProperty",
    "multiValueLegacyExtendedProperty"
  ],
  "@odata.type": "microsoft.graph.insightIdentity"
}-->
```json
{
  "displayName": "string",
  "id": "string",
  "address": "string"
}
```

## <a name="properties"></a><span data-ttu-id="bea2a-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="bea2a-107">Properties</span></span>

| <span data-ttu-id="bea2a-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bea2a-108">Property</span></span>              | <span data-ttu-id="bea2a-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="bea2a-109">Type</span></span>          | <span data-ttu-id="bea2a-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="bea2a-110">Description</span></span>  |
| -------------         |-----------    | -------------|
| <span data-ttu-id="bea2a-111">displayName</span><span class="sxs-lookup"><span data-stu-id="bea2a-111">displayName</span></span>       | <span data-ttu-id="bea2a-112">String</span><span class="sxs-lookup"><span data-stu-id="bea2a-112">String</span></span>          | <span data-ttu-id="bea2a-113">O nome de exibição do usuário que shared o item.</span><span class="sxs-lookup"><span data-stu-id="bea2a-113">The display name of the user who shared the item.</span></span> |
| <span data-ttu-id="bea2a-114">id</span><span class="sxs-lookup"><span data-stu-id="bea2a-114">id</span></span>              | <span data-ttu-id="bea2a-115">String</span><span class="sxs-lookup"><span data-stu-id="bea2a-115">String</span></span>        | <span data-ttu-id="bea2a-116">A identificação do usuário que shared o item.</span><span class="sxs-lookup"><span data-stu-id="bea2a-116">The id of the user who shared the item.</span></span>     |
| <span data-ttu-id="bea2a-117">address</span><span class="sxs-lookup"><span data-stu-id="bea2a-117">address</span></span>             | <span data-ttu-id="bea2a-118">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bea2a-118">String</span></span>      | <span data-ttu-id="bea2a-119">O endereço de email do usuário que shared o item.</span><span class="sxs-lookup"><span data-stu-id="bea2a-119">The email address of the user who shared the item.</span></span>  |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/insights-insightidentity.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
