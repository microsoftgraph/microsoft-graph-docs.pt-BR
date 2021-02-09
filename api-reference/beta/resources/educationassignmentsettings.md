---
title: Tipo de recurso educationAssignmentSettings
description: Especifica configurações de atribuições de nível de classe.
author: dipakboyed
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: d5990453eefbe63013ecfa0be03ff5b4d99330fa
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50153638"
---
# <a name="educationassignmentsettings-resource-type"></a><span data-ttu-id="6761f-103">Tipo de recurso educationAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="6761f-103">educationAssignmentSettings resource type</span></span>

<span data-ttu-id="6761f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6761f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6761f-105">Especifica configurações de atribuições de nível de classe.</span><span class="sxs-lookup"><span data-stu-id="6761f-105">Specifies class-level assignments settings.</span></span>

## <a name="methods"></a><span data-ttu-id="6761f-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="6761f-106">Methods</span></span>
|<span data-ttu-id="6761f-107">Método</span><span class="sxs-lookup"><span data-stu-id="6761f-107">Method</span></span>|<span data-ttu-id="6761f-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="6761f-108">Return type</span></span>|<span data-ttu-id="6761f-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="6761f-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="6761f-110">Obter educationAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="6761f-110">Get educationAssignmentSettings</span></span>](../api/educationassignmentsettings-get.md)|[<span data-ttu-id="6761f-111">educationAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="6761f-111">educationAssignmentSettings</span></span>](../resources/educationassignmentsettings.md)|<span data-ttu-id="6761f-112">Leia as propriedades e os relacionamentos de um [objeto educationAssignmentSettings.](../resources/educationassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="6761f-112">Read the properties and relationships of an [educationAssignmentSettings](../resources/educationassignmentsettings.md) object.</span></span>|
|[<span data-ttu-id="6761f-113">Atualizar educationAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="6761f-113">Update educationAssignmentSettings</span></span>](../api/educationassignmentsettings-update.md)|[<span data-ttu-id="6761f-114">educationAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="6761f-114">educationAssignmentSettings</span></span>](../resources/educationassignmentsettings.md)|<span data-ttu-id="6761f-115">Atualizar as propriedades de um [objeto educationAssignmentSettings.](../resources/educationassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="6761f-115">Update the properties of an [educationAssignmentSettings](../resources/educationassignmentsettings.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="6761f-116">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6761f-116">Properties</span></span>
|<span data-ttu-id="6761f-117">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6761f-117">Property</span></span>|<span data-ttu-id="6761f-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="6761f-118">Type</span></span>|<span data-ttu-id="6761f-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="6761f-119">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6761f-120">submissionAnimationDisabled</span><span class="sxs-lookup"><span data-stu-id="6761f-120">submissionAnimationDisabled</span></span>|<span data-ttu-id="6761f-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="6761f-121">Boolean</span></span>|<span data-ttu-id="6761f-122">Indica se a animação de celebração de turn-in será mostrada.</span><span class="sxs-lookup"><span data-stu-id="6761f-122">Indicates whether turn-in celebration animation will be shown.</span></span> <span data-ttu-id="6761f-123">Um valor indica `true` que a animação não será mostrada.</span><span class="sxs-lookup"><span data-stu-id="6761f-123">A value of `true` indicates that the animation will not be shown.</span></span> <span data-ttu-id="6761f-124">O valor padrão é `false`.</span><span class="sxs-lookup"><span data-stu-id="6761f-124">Default value is `false`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6761f-125">Relações</span><span class="sxs-lookup"><span data-stu-id="6761f-125">Relationships</span></span>
<span data-ttu-id="6761f-126">Nenhum</span><span class="sxs-lookup"><span data-stu-id="6761f-126">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="6761f-127">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6761f-127">JSON representation</span></span>
<span data-ttu-id="6761f-128">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6761f-128">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.educationAssignmentSettings",
  "openType": false
}
-->
``` json
{
  "submissionAnimationDisabled": false
}
```

