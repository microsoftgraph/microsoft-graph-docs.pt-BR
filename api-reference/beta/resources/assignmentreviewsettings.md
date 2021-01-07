---
title: tipo de recurso assignmentReviewSettings
description: O tipo assignmentReviewSettings, usado para a propriedade accessReviewSettings de uma política de atribuição de pacote do Access, fornece configurações adicionais para selecionar quem deve revisar as atribuições de pacote de acesso desta política e com que frequência elas devem ser revisadas.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 0bbc595395fbe7995b8ce7dfb7fa8e575faf58e8
ms.sourcegitcommit: 7732d20bd99a125118f7cea146c3f2416879f949
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/07/2021
ms.locfileid: "49777691"
---
# <a name="assignmentreviewsettings-resource-type"></a><span data-ttu-id="9573b-103">tipo de recurso assignmentReviewSettings</span><span class="sxs-lookup"><span data-stu-id="9573b-103">assignmentReviewSettings resource type</span></span>

<span data-ttu-id="9573b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9573b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9573b-105">Usado para a propriedade **accessReviewSettings** de uma [política de atribuição de pacote do Access](accesspackageassignmentpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="9573b-105">Used for the **accessReviewSettings** property of an [access package assignment policy](accesspackageassignmentpolicy.md).</span></span> <span data-ttu-id="9573b-106">Fornece configurações adicionais para selecionar quem deve revisar as atribuições de pacote de acesso desta política e com que frequência elas devem ser revisadas.</span><span class="sxs-lookup"><span data-stu-id="9573b-106">Provides additional settings to select who must review access package assignments from this policy, and how often they must be reviewed.</span></span>  

## <a name="properties"></a><span data-ttu-id="9573b-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9573b-107">Properties</span></span>

<span data-ttu-id="9573b-108">Este tipo tem as seguintes propriedades:</span><span class="sxs-lookup"><span data-stu-id="9573b-108">This type has the following properties:</span></span>

| <span data-ttu-id="9573b-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9573b-109">Property</span></span>                     | <span data-ttu-id="9573b-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="9573b-110">Type</span></span>                      | <span data-ttu-id="9573b-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="9573b-111">Description</span></span> |
| :--------------------------- | :------------------------ | :---------- |
| <span data-ttu-id="9573b-112">isEnabled</span><span class="sxs-lookup"><span data-stu-id="9573b-112">isEnabled</span></span>| <span data-ttu-id="9573b-113">Booliano</span><span class="sxs-lookup"><span data-stu-id="9573b-113">Boolean</span></span> | <span data-ttu-id="9573b-114">Se verdadeiro, as revisões do Access são necessárias para as atribuições desta política.</span><span class="sxs-lookup"><span data-stu-id="9573b-114">If true, access reviews are required for assignments from this policy.</span></span> |
| <span data-ttu-id="9573b-115">recurrenceType</span><span class="sxs-lookup"><span data-stu-id="9573b-115">recurrenceType</span></span> | <span data-ttu-id="9573b-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9573b-116">String</span></span> | <span data-ttu-id="9573b-117">O intervalo de recorrência, como `monthly` ou `quarterly` .</span><span class="sxs-lookup"><span data-stu-id="9573b-117">The interval for recurrence, such as `monthly` or `quarterly`.</span></span> |
| <span data-ttu-id="9573b-118">revisor</span><span class="sxs-lookup"><span data-stu-id="9573b-118">reviewerType</span></span> | <span data-ttu-id="9573b-119">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9573b-119">String</span></span> | <span data-ttu-id="9573b-120">Quem deve ser solicitado a fazer a revisão, `Self` ou `Reviewers` .</span><span class="sxs-lookup"><span data-stu-id="9573b-120">Who should be asked to do the review, either `Self` or `Reviewers`.</span></span> |
| <span data-ttu-id="9573b-121">startDateTime</span><span class="sxs-lookup"><span data-stu-id="9573b-121">startDateTime</span></span> | <span data-ttu-id="9573b-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9573b-122">DateTimeOffset</span></span> | <span data-ttu-id="9573b-123">Quando a primeira revisão deve iniciar.</span><span class="sxs-lookup"><span data-stu-id="9573b-123">When the first review should start.</span></span> |
| <span data-ttu-id="9573b-124">durationInDays</span><span class="sxs-lookup"><span data-stu-id="9573b-124">durationInDays</span></span> | <span data-ttu-id="9573b-125">Int32</span><span class="sxs-lookup"><span data-stu-id="9573b-125">Int32</span></span> | <span data-ttu-id="9573b-126">O número de dias para permitir a entrada de revisores.</span><span class="sxs-lookup"><span data-stu-id="9573b-126">The number of days to allow input from reviewers.</span></span>|
| <span data-ttu-id="9573b-127">revisores</span><span class="sxs-lookup"><span data-stu-id="9573b-127">reviewers</span></span> | <span data-ttu-id="9573b-128">coleção [userset](userset.md)</span><span class="sxs-lookup"><span data-stu-id="9573b-128">[userSet](userset.md) collection</span></span> | <span data-ttu-id="9573b-129">Se o revisortype for `Reviewers` , essa coleção especifica os usuários que serão revisores, por ID ou como membros de um grupo, usando uma coleção de [Únicousuário](singleuser.md) e [groupMembers](groupmembers.md).</span><span class="sxs-lookup"><span data-stu-id="9573b-129">If the reviewerType is `Reviewers`, this collection specifies the users who will be reviewers, either by ID or as members of a group, using a collection of [singleUser](singleuser.md) and [groupMembers](groupmembers.md).</span></span> |

## <a name="json-representation"></a><span data-ttu-id="9573b-130">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9573b-130">JSON representation</span></span>


<span data-ttu-id="9573b-131">Veja a seguir uma representação JSON da propriedade de configurações de revisão do Access de uma política.</span><span class="sxs-lookup"><span data-stu-id="9573b-131">The following is a JSON representation of the access review settings property of a policy.</span></span>

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


