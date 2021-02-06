---
title: Tipo de recurso assignmentReviewSettings
description: O tipo assignmentReviewSettings, usado para a propriedade accessReviewSettings de uma política de atribuição de pacote de acesso, fornece configurações adicionais para selecionar quem deve revisar as atribuições de pacote de acesso dessa política e com que frequência elas devem ser revisadas.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: bde8c6d330eda7e100071edbf2190e170ca913ea
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50131318"
---
# <a name="assignmentreviewsettings-resource-type"></a><span data-ttu-id="881e2-103">Tipo de recurso assignmentReviewSettings</span><span class="sxs-lookup"><span data-stu-id="881e2-103">assignmentReviewSettings resource type</span></span>

<span data-ttu-id="881e2-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="881e2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="881e2-105">Usado para a **propriedade accessReviewSettings** de uma política [de atribuição de pacote de acesso.](accesspackageassignmentpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="881e2-105">Used for the **accessReviewSettings** property of an [access package assignment policy](accesspackageassignmentpolicy.md).</span></span> <span data-ttu-id="881e2-106">Fornece configurações adicionais para selecionar quem deve revisar as atribuições do pacote de acesso desta política e a frequência com que elas devem ser revisadas.</span><span class="sxs-lookup"><span data-stu-id="881e2-106">Provides additional settings to select who must review access package assignments from this policy, and how often they must be reviewed.</span></span>  

## <a name="properties"></a><span data-ttu-id="881e2-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="881e2-107">Properties</span></span>

<span data-ttu-id="881e2-108">Esse tipo tem as seguintes propriedades:</span><span class="sxs-lookup"><span data-stu-id="881e2-108">This type has the following properties:</span></span>

| <span data-ttu-id="881e2-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="881e2-109">Property</span></span>                     | <span data-ttu-id="881e2-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="881e2-110">Type</span></span>                      | <span data-ttu-id="881e2-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="881e2-111">Description</span></span> |
| :--------------------------- | :------------------------ | :---------- |
| <span data-ttu-id="881e2-112">isEnabled</span><span class="sxs-lookup"><span data-stu-id="881e2-112">isEnabled</span></span>| <span data-ttu-id="881e2-113">Booliano</span><span class="sxs-lookup"><span data-stu-id="881e2-113">Boolean</span></span> | <span data-ttu-id="881e2-114">Se for verdadeiro, as revisões de acesso serão necessárias para as atribuições dessa política.</span><span class="sxs-lookup"><span data-stu-id="881e2-114">If true, access reviews are required for assignments from this policy.</span></span> |
| <span data-ttu-id="881e2-115">recurrenceType</span><span class="sxs-lookup"><span data-stu-id="881e2-115">recurrenceType</span></span> | <span data-ttu-id="881e2-116">String</span><span class="sxs-lookup"><span data-stu-id="881e2-116">String</span></span> | <span data-ttu-id="881e2-117">O intervalo de recorrência, como `monthly` ou `quarterly` .</span><span class="sxs-lookup"><span data-stu-id="881e2-117">The interval for recurrence, such as `monthly` or `quarterly`.</span></span> |
| <span data-ttu-id="881e2-118">reviewerType</span><span class="sxs-lookup"><span data-stu-id="881e2-118">reviewerType</span></span> | <span data-ttu-id="881e2-119">String</span><span class="sxs-lookup"><span data-stu-id="881e2-119">String</span></span> | <span data-ttu-id="881e2-120">Quem deve ser solicitado a fazer a revisão, `Self` ou `Reviewers` .</span><span class="sxs-lookup"><span data-stu-id="881e2-120">Who should be asked to do the review, either `Self` or `Reviewers`.</span></span> |
| <span data-ttu-id="881e2-121">startDateTime</span><span class="sxs-lookup"><span data-stu-id="881e2-121">startDateTime</span></span> | <span data-ttu-id="881e2-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="881e2-122">DateTimeOffset</span></span> | <span data-ttu-id="881e2-123">Quando a primeira revisão deve começar.</span><span class="sxs-lookup"><span data-stu-id="881e2-123">When the first review should start.</span></span> |
| <span data-ttu-id="881e2-124">durationInDays</span><span class="sxs-lookup"><span data-stu-id="881e2-124">durationInDays</span></span> | <span data-ttu-id="881e2-125">Int32</span><span class="sxs-lookup"><span data-stu-id="881e2-125">Int32</span></span> | <span data-ttu-id="881e2-126">O número de dias para permitir a entrada dos revisadores.</span><span class="sxs-lookup"><span data-stu-id="881e2-126">The number of days to allow input from reviewers.</span></span>|
| <span data-ttu-id="881e2-127">reviewers</span><span class="sxs-lookup"><span data-stu-id="881e2-127">reviewers</span></span> | <span data-ttu-id="881e2-128">[Coleção userSet](userset.md)</span><span class="sxs-lookup"><span data-stu-id="881e2-128">[userSet](userset.md) collection</span></span> | <span data-ttu-id="881e2-129">Se reviewerType for , esta coleção especificará os usuários que serão revisadores, por ID ou como membros de um grupo, usando uma coleção de `Reviewers` [singleUser](singleuser.md) e [groupMembers](groupmembers.md).</span><span class="sxs-lookup"><span data-stu-id="881e2-129">If the reviewerType is `Reviewers`, this collection specifies the users who will be reviewers, either by ID or as members of a group, using a collection of [singleUser](singleuser.md) and [groupMembers](groupmembers.md).</span></span> |

## <a name="json-representation"></a><span data-ttu-id="881e2-130">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="881e2-130">JSON representation</span></span>


<span data-ttu-id="881e2-131">A seguir está uma representação JSON da propriedade de configurações de revisão de acesso de uma política.</span><span class="sxs-lookup"><span data-stu-id="881e2-131">The following is a JSON representation of the access review settings property of a policy.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.assignmentReviewSettings"
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


