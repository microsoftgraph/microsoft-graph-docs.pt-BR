---
title: Tipo de recurso educationAssignmentSettings
description: Especifica as configurações de atribuições de nível de classe.
author: sharad-sharma-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: ccaa51c84e50e2f9c5302836ffd9b92754f517fd
ms.sourcegitcommit: f77c1385306fd40557aceb24fdfe4832cbb60a27
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/12/2021
ms.locfileid: "52912225"
---
# <a name="educationassignmentsettings-resource-type"></a><span data-ttu-id="52bc9-103">Tipo de recurso educationAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="52bc9-103">educationAssignmentSettings resource type</span></span>

<span data-ttu-id="52bc9-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="52bc9-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="52bc9-105">Especifica as configurações de atribuições de nível de classe.</span><span class="sxs-lookup"><span data-stu-id="52bc9-105">Specifies class-level assignments settings.</span></span>

## <a name="methods"></a><span data-ttu-id="52bc9-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="52bc9-106">Methods</span></span>
|<span data-ttu-id="52bc9-107">Método</span><span class="sxs-lookup"><span data-stu-id="52bc9-107">Method</span></span>|<span data-ttu-id="52bc9-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="52bc9-108">Return type</span></span>|<span data-ttu-id="52bc9-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="52bc9-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="52bc9-110">Obter educationAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="52bc9-110">Get educationAssignmentSettings</span></span>](../api/educationassignmentsettings-get.md)|[<span data-ttu-id="52bc9-111">educationAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="52bc9-111">educationAssignmentSettings</span></span>](../resources/educationassignmentsettings.md)|<span data-ttu-id="52bc9-112">Leia as propriedades e as relações de um [objeto educationAssignmentSettings.](../resources/educationassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="52bc9-112">Read the properties and relationships of an [educationAssignmentSettings](../resources/educationassignmentsettings.md) object.</span></span>|
|[<span data-ttu-id="52bc9-113">Atualizar educationAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="52bc9-113">Update educationAssignmentSettings</span></span>](../api/educationassignmentsettings-update.md)|[<span data-ttu-id="52bc9-114">educationAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="52bc9-114">educationAssignmentSettings</span></span>](../resources/educationassignmentsettings.md)|<span data-ttu-id="52bc9-115">Atualize as propriedades de [um objeto educationAssignmentSettings.](../resources/educationassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="52bc9-115">Update the properties of an [educationAssignmentSettings](../resources/educationassignmentsettings.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="52bc9-116">Propriedades</span><span class="sxs-lookup"><span data-stu-id="52bc9-116">Properties</span></span>
|<span data-ttu-id="52bc9-117">Propriedade</span><span class="sxs-lookup"><span data-stu-id="52bc9-117">Property</span></span>|<span data-ttu-id="52bc9-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="52bc9-118">Type</span></span>|<span data-ttu-id="52bc9-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="52bc9-119">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="52bc9-120">submissionAnimationDisabled</span><span class="sxs-lookup"><span data-stu-id="52bc9-120">submissionAnimationDisabled</span></span>|<span data-ttu-id="52bc9-121">Booliano</span><span class="sxs-lookup"><span data-stu-id="52bc9-121">Boolean</span></span>|<span data-ttu-id="52bc9-122">Indica se a animação de celebração de turn-in será mostrada.</span><span class="sxs-lookup"><span data-stu-id="52bc9-122">Indicates whether turn-in celebration animation will be shown.</span></span> <span data-ttu-id="52bc9-123">Um valor `true` indica que a animação não será mostrada.</span><span class="sxs-lookup"><span data-stu-id="52bc9-123">A value of `true` indicates that the animation will not be shown.</span></span> <span data-ttu-id="52bc9-124">O valor padrão é `false`.</span><span class="sxs-lookup"><span data-stu-id="52bc9-124">Default value is `false`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="52bc9-125">Relações</span><span class="sxs-lookup"><span data-stu-id="52bc9-125">Relationships</span></span>
<span data-ttu-id="52bc9-126">Nenhum</span><span class="sxs-lookup"><span data-stu-id="52bc9-126">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="52bc9-127">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="52bc9-127">JSON representation</span></span>
<span data-ttu-id="52bc9-128">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="52bc9-128">The following is a JSON representation of the resource.</span></span>
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

