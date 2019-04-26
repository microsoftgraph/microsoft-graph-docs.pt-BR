---
title: insightIdentity
description: Tipo complexo contendo propriedades de itens compartilhados.
author: simonhult
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: 45ac8874a30ebb4f3196f03a675229bf1fab750c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32549563"
---
# <a name="insightidentity"></a><span data-ttu-id="1ddfe-103">insightIdentity</span><span class="sxs-lookup"><span data-stu-id="1ddfe-103">insightIdentity</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1ddfe-104">Tipo complexo contendo propriedades de itens [compartilhados](insights-shared.md) .</span><span class="sxs-lookup"><span data-stu-id="1ddfe-104">Complex type containing properties of [Shared](insights-shared.md) items.</span></span> 

## <a name="json-representation"></a><span data-ttu-id="1ddfe-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1ddfe-105">JSON representation</span></span>
<span data-ttu-id="1ddfe-106">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="1ddfe-106">Here is a JSON representation of the resource</span></span>

```json
{
  "displayName": "string",
  "id": "string",
  "address": "string"
}
```

## <a name="properties"></a><span data-ttu-id="1ddfe-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1ddfe-107">Properties</span></span>

| <span data-ttu-id="1ddfe-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1ddfe-108">Property</span></span>              | <span data-ttu-id="1ddfe-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="1ddfe-109">Type</span></span>          | <span data-ttu-id="1ddfe-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="1ddfe-110">Description</span></span>  |
| -------------         |-----------    | -------------|
| <span data-ttu-id="1ddfe-111">displayName</span><span class="sxs-lookup"><span data-stu-id="1ddfe-111">displayName</span></span>       | <span data-ttu-id="1ddfe-112">String</span><span class="sxs-lookup"><span data-stu-id="1ddfe-112">String</span></span>          | <span data-ttu-id="1ddfe-113">O nome de exibição do usuário que compartilhou o item.</span><span class="sxs-lookup"><span data-stu-id="1ddfe-113">The display name of the user who shared the item.</span></span> |
| <span data-ttu-id="1ddfe-114">id</span><span class="sxs-lookup"><span data-stu-id="1ddfe-114">id</span></span>              | <span data-ttu-id="1ddfe-115">String</span><span class="sxs-lookup"><span data-stu-id="1ddfe-115">String</span></span>        | <span data-ttu-id="1ddfe-116">A ID do usuário que compartilhou o item.</span><span class="sxs-lookup"><span data-stu-id="1ddfe-116">The id of the user who shared the item.</span></span>     |
| <span data-ttu-id="1ddfe-117">address</span><span class="sxs-lookup"><span data-stu-id="1ddfe-117">address</span></span>             | <span data-ttu-id="1ddfe-118">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1ddfe-118">String</span></span>      | <span data-ttu-id="1ddfe-119">O endereço de email do usuário que compartilhou o item.</span><span class="sxs-lookup"><span data-stu-id="1ddfe-119">The email address of the user who shared the item.</span></span>  |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/insights-insightidentity.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
