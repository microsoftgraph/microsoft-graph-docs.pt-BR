---
title: tipo de recurso assignmentReviewSettings
description: O tipo assignmentReviewSettings, usado para a propriedade accessReviewSettings de uma política de atribuição de pacote do Access, fornece configurações adicionais para selecionar quem deve revisar as atribuições de pacote de acesso desta política e com que frequência elas devem ser revisadas.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: c673d96ab5bb6dbb6f217d5b36f41520b421f5bf
ms.sourcegitcommit: ec6aa498067c9df6139a469e694a89447b155a1e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/28/2020
ms.locfileid: "42331345"
---
# <a name="assignmentreviewsettings-resource-type"></a><span data-ttu-id="6f550-103">tipo de recurso assignmentReviewSettings</span><span class="sxs-lookup"><span data-stu-id="6f550-103">assignmentReviewSettings resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6f550-104">Usado para a propriedade **accessReviewSettings** de uma [política de atribuição de pacote do Access](accesspackageassignmentpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="6f550-104">Used for the **accessReviewSettings** property of an [access package assignment policy](accesspackageassignmentpolicy.md).</span></span> <span data-ttu-id="6f550-105">Fornece configurações adicionais para selecionar quem deve revisar as atribuições de pacote de acesso desta política e com que frequência elas devem ser revisadas.</span><span class="sxs-lookup"><span data-stu-id="6f550-105">Provides additional settings to select who must review access package assignments from this policy, and how often they must be reviewed.</span></span>  

## <a name="properties"></a><span data-ttu-id="6f550-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6f550-106">Properties</span></span>

<span data-ttu-id="6f550-107">Este tipo tem as seguintes propriedades:</span><span class="sxs-lookup"><span data-stu-id="6f550-107">This type has the following properties:</span></span>

| <span data-ttu-id="6f550-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6f550-108">Property</span></span>                     | <span data-ttu-id="6f550-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="6f550-109">Type</span></span>                      | <span data-ttu-id="6f550-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="6f550-110">Description</span></span> |
| :--------------------------- | :------------------------ | :---------- |
| <span data-ttu-id="6f550-111">isEnabled</span><span class="sxs-lookup"><span data-stu-id="6f550-111">isEnabled</span></span>| <span data-ttu-id="6f550-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f550-112">Boolean</span></span> | <span data-ttu-id="6f550-113">Se verdadeiro, as revisões do Access são necessárias para as atribuições desta política.</span><span class="sxs-lookup"><span data-stu-id="6f550-113">If true, access reviews are required for assignments from this policy.</span></span> |
| <span data-ttu-id="6f550-114">recurrenceType</span><span class="sxs-lookup"><span data-stu-id="6f550-114">recurrenceType</span></span> | <span data-ttu-id="6f550-115">String</span><span class="sxs-lookup"><span data-stu-id="6f550-115">String</span></span> | <span data-ttu-id="6f550-116">O intervalo de recorrência, como `monthly` ou `quarterly`.</span><span class="sxs-lookup"><span data-stu-id="6f550-116">The interval for recurrence, such as `monthly` or `quarterly`.</span></span> |
| <span data-ttu-id="6f550-117">revisor</span><span class="sxs-lookup"><span data-stu-id="6f550-117">reviewerType</span></span> | <span data-ttu-id="6f550-118">String</span><span class="sxs-lookup"><span data-stu-id="6f550-118">String</span></span> | <span data-ttu-id="6f550-119">Quem deve ser solicitado a fazer a revisão, `Self` ou. `Reviewers`</span><span class="sxs-lookup"><span data-stu-id="6f550-119">Who should be asked to do the review, either `Self` or `Reviewers`.</span></span> |
| <span data-ttu-id="6f550-120">startDateTime</span><span class="sxs-lookup"><span data-stu-id="6f550-120">startDateTime</span></span> | <span data-ttu-id="6f550-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6f550-121">DateTimeOffset</span></span> | <span data-ttu-id="6f550-122">Quando a primeira revisão deve iniciar.</span><span class="sxs-lookup"><span data-stu-id="6f550-122">When the first review should start.</span></span> |
| <span data-ttu-id="6f550-123">durationInDays</span><span class="sxs-lookup"><span data-stu-id="6f550-123">durationInDays</span></span> | <span data-ttu-id="6f550-124">Int32</span><span class="sxs-lookup"><span data-stu-id="6f550-124">Int32</span></span> | <span data-ttu-id="6f550-125">O número de dias para permitir a entrada de revisores.</span><span class="sxs-lookup"><span data-stu-id="6f550-125">The number of days to allow input from reviewers.</span></span>|
| <span data-ttu-id="6f550-126">revisores</span><span class="sxs-lookup"><span data-stu-id="6f550-126">reviewers</span></span> | <span data-ttu-id="6f550-127">coleção [userset](userset.md)</span><span class="sxs-lookup"><span data-stu-id="6f550-127">[userSet](userset.md) collection</span></span> | <span data-ttu-id="6f550-128">Se o revisortype for `Reviewers`, essa coleção especifica os usuários que serão revisores, por ID ou como membros de um grupo, usando uma coleção de [únicousuário](singleuser.md) e [groupMembers](groupmembers.md).</span><span class="sxs-lookup"><span data-stu-id="6f550-128">If the reviewerType is `Reviewers`, this collection specifies the users who will be reviewers, either by ID or as members of a group, using a collection of [singleUser](singleuser.md) and [groupMembers](groupmembers.md).</span></span> |

## <a name="json-representation"></a><span data-ttu-id="6f550-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6f550-129">JSON representation</span></span>


<span data-ttu-id="6f550-130">Veja a seguir uma representação JSON da propriedade de configurações de revisão do Access de uma política.</span><span class="sxs-lookup"><span data-stu-id="6f550-130">The following is a JSON representation of the access review settings property of a policy.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.assignmentReviewSettings",
  "baseType": ""
}-->

```json
{
  "isEnabled": true,
  "recurrenceType": "quarterly",
  "reviewerType": "Self",
  "startDateTime": "2020-01-23T07:59:59.998Z",
  "durationInDays": 25,
  "reviewers": []
}
```


<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "assignmentReviewSettings complex type",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
