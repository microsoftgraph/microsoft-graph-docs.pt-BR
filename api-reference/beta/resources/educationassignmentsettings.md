---
title: Tipo de recurso educationAssignmentSettings
description: Especifica configurações de atribuições de nível de classe.
author: dipakboyed
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: c670cb2bbef0b82ff80996e4acb52c2826ec118f
ms.sourcegitcommit: 9a03b719d1316729dd022bf4d268894e91515475
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/28/2021
ms.locfileid: "50034325"
---
# <a name="educationassignmentsettings-resource-type"></a><span data-ttu-id="6878b-103">Tipo de recurso educationAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="6878b-103">educationAssignmentSettings resource type</span></span>

<span data-ttu-id="6878b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6878b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6878b-105">Especifica configurações de atribuições de nível de classe.</span><span class="sxs-lookup"><span data-stu-id="6878b-105">Specifies class-level assignments settings.</span></span>

## <a name="methods"></a><span data-ttu-id="6878b-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="6878b-106">Methods</span></span>
|<span data-ttu-id="6878b-107">Método</span><span class="sxs-lookup"><span data-stu-id="6878b-107">Method</span></span>|<span data-ttu-id="6878b-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="6878b-108">Return type</span></span>|<span data-ttu-id="6878b-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="6878b-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="6878b-110">Obter educationAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="6878b-110">Get educationAssignmentSettings</span></span>](../api/educationassignmentsettings-get.md)|[<span data-ttu-id="6878b-111">educationAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="6878b-111">educationAssignmentSettings</span></span>](../resources/educationassignmentsettings.md)|<span data-ttu-id="6878b-112">Leia as propriedades e os relacionamentos de um [objeto educationAssignmentSettings.](../resources/educationassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="6878b-112">Read the properties and relationships of an [educationAssignmentSettings](../resources/educationassignmentsettings.md) object.</span></span>|
|[<span data-ttu-id="6878b-113">Atualizar educationAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="6878b-113">Update educationAssignmentSettings</span></span>](../api/educationassignmentsettings-update.md)|[<span data-ttu-id="6878b-114">educationAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="6878b-114">educationAssignmentSettings</span></span>](../resources/educationassignmentsettings.md)|<span data-ttu-id="6878b-115">Atualizar as propriedades de um [objeto educationAssignmentSettings.](../resources/educationassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="6878b-115">Update the properties of an [educationAssignmentSettings](../resources/educationassignmentsettings.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="6878b-116">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6878b-116">Properties</span></span>
|<span data-ttu-id="6878b-117">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6878b-117">Property</span></span>|<span data-ttu-id="6878b-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="6878b-118">Type</span></span>|<span data-ttu-id="6878b-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="6878b-119">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6878b-120">submissionAnimationDisabled</span><span class="sxs-lookup"><span data-stu-id="6878b-120">submissionAnimationDisabled</span></span>|<span data-ttu-id="6878b-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="6878b-121">Boolean</span></span>|<span data-ttu-id="6878b-122">Indica se a animação de celebração de turn-in será mostrada.</span><span class="sxs-lookup"><span data-stu-id="6878b-122">Indicates whether turn-in celebration animation will be shown.</span></span> <span data-ttu-id="6878b-123">Um valor indica `true` que a animação não será mostrada.</span><span class="sxs-lookup"><span data-stu-id="6878b-123">A value of `true` indicates that the animation will not be shown.</span></span> <span data-ttu-id="6878b-124">O valor padrão é `false`.</span><span class="sxs-lookup"><span data-stu-id="6878b-124">Default value is `false`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6878b-125">Relações</span><span class="sxs-lookup"><span data-stu-id="6878b-125">Relationships</span></span>
<span data-ttu-id="6878b-126">Nenhum</span><span class="sxs-lookup"><span data-stu-id="6878b-126">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="6878b-127">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6878b-127">JSON representation</span></span>
<span data-ttu-id="6878b-128">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6878b-128">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.educationAssignmentSettings",
  "baseType": "",
  "openType": false
}
-->
``` json
{
  "submissionAnimationDisabled": false
}
```

