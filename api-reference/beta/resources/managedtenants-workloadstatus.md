---
title: Tipo de recurso workloadStatus
description: Represente o status de uma carga de trabalho.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: 50cbd9cdc59426f413333835c4418112401d8038
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/13/2021
ms.locfileid: "53402125"
---
# <a name="workloadstatus-resource-type"></a><span data-ttu-id="eaca6-103">Tipo de recurso workloadStatus</span><span class="sxs-lookup"><span data-stu-id="eaca6-103">workloadStatus resource type</span></span>

<span data-ttu-id="eaca6-104">Namespace: microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="eaca6-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="eaca6-105">Represente o status de uma carga de trabalho.</span><span class="sxs-lookup"><span data-stu-id="eaca6-105">Represent the status for a workload.</span></span>

## <a name="properties"></a><span data-ttu-id="eaca6-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="eaca6-106">Properties</span></span>
|<span data-ttu-id="eaca6-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="eaca6-107">Property</span></span>|<span data-ttu-id="eaca6-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="eaca6-108">Type</span></span>|<span data-ttu-id="eaca6-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="eaca6-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eaca6-110">displayName</span><span class="sxs-lookup"><span data-stu-id="eaca6-110">displayName</span></span>|<span data-ttu-id="eaca6-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="eaca6-111">String</span></span>|<span data-ttu-id="eaca6-112">O nome de exibição da carga de trabalho.</span><span class="sxs-lookup"><span data-stu-id="eaca6-112">The display name for the workload.</span></span> <span data-ttu-id="eaca6-113">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="eaca6-113">Required.</span></span> <span data-ttu-id="eaca6-114">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="eaca6-114">Read-only.</span></span>|
|<span data-ttu-id="eaca6-115">offboardedDateTime</span><span class="sxs-lookup"><span data-stu-id="eaca6-115">offboardedDateTime</span></span>|<span data-ttu-id="eaca6-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="eaca6-116">DateTimeOffset</span></span>|<span data-ttu-id="eaca6-117">A data e a hora em que a carga de trabalho foi desligada.</span><span class="sxs-lookup"><span data-stu-id="eaca6-117">The date and time the workload was offboarded.</span></span> <span data-ttu-id="eaca6-118">Opcional.</span><span class="sxs-lookup"><span data-stu-id="eaca6-118">Optional.</span></span> <span data-ttu-id="eaca6-119">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="eaca6-119">Read-only.</span></span>|
|<span data-ttu-id="eaca6-120">onboardedDateTime</span><span class="sxs-lookup"><span data-stu-id="eaca6-120">onboardedDateTime</span></span>|<span data-ttu-id="eaca6-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="eaca6-121">DateTimeOffset</span></span>|<span data-ttu-id="eaca6-122">A data e a hora em que a carga de trabalho foi internada.</span><span class="sxs-lookup"><span data-stu-id="eaca6-122">The date and time the workload was onboarded.</span></span> <span data-ttu-id="eaca6-123">Opcional.</span><span class="sxs-lookup"><span data-stu-id="eaca6-123">Optional.</span></span> <span data-ttu-id="eaca6-124">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="eaca6-124">Read-only.</span></span>|
|<span data-ttu-id="eaca6-125">onboardingStatus</span><span class="sxs-lookup"><span data-stu-id="eaca6-125">onboardingStatus</span></span>|<span data-ttu-id="eaca6-126">workloadOnboardingStatus</span><span class="sxs-lookup"><span data-stu-id="eaca6-126">workloadOnboardingStatus</span></span>|<span data-ttu-id="eaca6-127">O status de integração da carga de trabalho.</span><span class="sxs-lookup"><span data-stu-id="eaca6-127">The onboarding status for the workload.</span></span> <span data-ttu-id="eaca6-128">Os valores possíveis são: `notOnboarded`, `onboarded`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="eaca6-128">Possible values are: `notOnboarded`, `onboarded`, `unknownFutureValue`.</span></span> <span data-ttu-id="eaca6-129">Opcional.</span><span class="sxs-lookup"><span data-stu-id="eaca6-129">Optional.</span></span> <span data-ttu-id="eaca6-130">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="eaca6-130">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="eaca6-131">Relações</span><span class="sxs-lookup"><span data-stu-id="eaca6-131">Relationships</span></span>
<span data-ttu-id="eaca6-132">Nenhum</span><span class="sxs-lookup"><span data-stu-id="eaca6-132">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="eaca6-133">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="eaca6-133">JSON representation</span></span>
<span data-ttu-id="eaca6-134">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="eaca6-134">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managedTenants.workloadStatus"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.workloadStatus",
  "onboardingStatus": "String",
  "onboardedDateTime": "String (timestamp)",
  "displayName": "String",
  "offboardedDateTime": "String (timestamp)"
}
```
