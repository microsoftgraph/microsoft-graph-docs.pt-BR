---
title: tipo de recurso de educationAssignmentPointsGrade
description: Quando uma atribuição for definida como um tipo de nível de pontos, a cada envio terão este objeto associado com a propriedade **submission.grade** . Isso cria uma subclasse do educationAssignmentGrade,
localization_priority: Normal
author: dipakboyed
ms.prod: education
ms.openlocfilehash: d96b84380bc7a6d2298117b5dfeaee25d943efb2
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27982383"
---
# <a name="educationassignmentpointsgrade-resource-type"></a><span data-ttu-id="f2cda-104">tipo de recurso de educationAssignmentPointsGrade</span><span class="sxs-lookup"><span data-stu-id="f2cda-104">educationAssignmentPointsGrade resource type</span></span>

> <span data-ttu-id="f2cda-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="f2cda-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f2cda-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="f2cda-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f2cda-107">Quando uma atribuição for definida como um tipo de nível de pontos, a cada envio terão este objeto associado com a propriedade **submission.grade** .</span><span class="sxs-lookup"><span data-stu-id="f2cda-107">When an assignment is set to a points grade type, each submission will have this object associated with the **submission.grade** property.</span></span> <span data-ttu-id="f2cda-108">Isso cria uma subclasse do [educationAssignmentGrade](educationassignmentgrade.md), que adicionará a quem dados para esta propriedade.</span><span class="sxs-lookup"><span data-stu-id="f2cda-108">This creates a subclass from [educationAssignmentGrade](educationassignmentgrade.md), which will add the who data to this property.</span></span> <span data-ttu-id="f2cda-109">Os pontos máximo é armazenado na propriedade **assignments.grading** .</span><span class="sxs-lookup"><span data-stu-id="f2cda-109">The max points is stored in the **assignments.grading** property.</span></span>


## <a name="properties"></a><span data-ttu-id="f2cda-110">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f2cda-110">Properties</span></span>
| <span data-ttu-id="f2cda-111">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f2cda-111">Property</span></span>     | <span data-ttu-id="f2cda-112">Tipo</span><span class="sxs-lookup"><span data-stu-id="f2cda-112">Type</span></span>   |<span data-ttu-id="f2cda-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="f2cda-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f2cda-114">points</span><span class="sxs-lookup"><span data-stu-id="f2cda-114">points</span></span>|<span data-ttu-id="f2cda-115">Single</span><span class="sxs-lookup"><span data-stu-id="f2cda-115">Single</span></span>|<span data-ttu-id="f2cda-116">Número de pontos um professor está dando este objeto de envio.</span><span class="sxs-lookup"><span data-stu-id="f2cda-116">Number of points a teacher is giving this submission object.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f2cda-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f2cda-117">JSON representation</span></span>

<span data-ttu-id="f2cda-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f2cda-118">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationAssignmentPointsGrade"
}-->

```json
{
  "points": "Single"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationAssignmentPointsGrade resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
