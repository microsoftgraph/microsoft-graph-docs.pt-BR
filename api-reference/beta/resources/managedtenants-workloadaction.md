---
title: Tipo de recurso workloadAction
description: Representa uma ação que será executada para uma carga de trabalho específica.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: e6dbbe1458aa6dba37a26af70ee0e64b92a52cf4
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/13/2021
ms.locfileid: "53401962"
---
# <a name="workloadaction-resource-type"></a><span data-ttu-id="38900-103">Tipo de recurso workloadAction</span><span class="sxs-lookup"><span data-stu-id="38900-103">workloadAction resource type</span></span>

<span data-ttu-id="38900-104">Namespace: microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="38900-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="38900-105">Representa uma ação que será executada para uma carga de trabalho específica.</span><span class="sxs-lookup"><span data-stu-id="38900-105">Represents an action that will be performed for a specific workload.</span></span>

## <a name="properties"></a><span data-ttu-id="38900-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="38900-106">Properties</span></span>
|<span data-ttu-id="38900-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="38900-107">Property</span></span>|<span data-ttu-id="38900-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="38900-108">Type</span></span>|<span data-ttu-id="38900-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="38900-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="38900-110">actionId</span><span class="sxs-lookup"><span data-stu-id="38900-110">actionId</span></span>|<span data-ttu-id="38900-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="38900-111">String</span></span>|<span data-ttu-id="38900-112">O identificador exclusivo da ação de carga de trabalho.</span><span class="sxs-lookup"><span data-stu-id="38900-112">The unique identifier for the workload action.</span></span> <span data-ttu-id="38900-113">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="38900-113">Required.</span></span> <span data-ttu-id="38900-114">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="38900-114">Read-only.</span></span>|
|<span data-ttu-id="38900-115">category</span><span class="sxs-lookup"><span data-stu-id="38900-115">category</span></span>|<span data-ttu-id="38900-116">workloadActionCategory</span><span class="sxs-lookup"><span data-stu-id="38900-116">workloadActionCategory</span></span>|<span data-ttu-id="38900-117">A categoria da ação de carga de trabalho.</span><span class="sxs-lookup"><span data-stu-id="38900-117">The category for the workload action.</span></span> <span data-ttu-id="38900-118">Os valores possíveis são: `automated`, `manual`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="38900-118">Possible values are: `automated`, `manual`, `unknownFutureValue`.</span></span> <span data-ttu-id="38900-119">Opcional.</span><span class="sxs-lookup"><span data-stu-id="38900-119">Optional.</span></span> <span data-ttu-id="38900-120">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="38900-120">Read-only.</span></span>|
|<span data-ttu-id="38900-121">description</span><span class="sxs-lookup"><span data-stu-id="38900-121">description</span></span>|<span data-ttu-id="38900-122">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="38900-122">String</span></span>|<span data-ttu-id="38900-123">A descrição da ação de carga de trabalho.</span><span class="sxs-lookup"><span data-stu-id="38900-123">The description for the workload action.</span></span> <span data-ttu-id="38900-124">Opcional.</span><span class="sxs-lookup"><span data-stu-id="38900-124">Optional.</span></span> <span data-ttu-id="38900-125">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="38900-125">Read-only.</span></span>|
|<span data-ttu-id="38900-126">displayName</span><span class="sxs-lookup"><span data-stu-id="38900-126">displayName</span></span>|<span data-ttu-id="38900-127">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="38900-127">String</span></span>|<span data-ttu-id="38900-128">O nome de exibição da ação de carga de trabalho.</span><span class="sxs-lookup"><span data-stu-id="38900-128">The display name for the workload action.</span></span> <span data-ttu-id="38900-129">Opcional.</span><span class="sxs-lookup"><span data-stu-id="38900-129">Optional.</span></span> <span data-ttu-id="38900-130">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="38900-130">Read-only.</span></span>|
|<span data-ttu-id="38900-131">service</span><span class="sxs-lookup"><span data-stu-id="38900-131">service</span></span>|<span data-ttu-id="38900-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="38900-132">String</span></span>|<span data-ttu-id="38900-133">O serviço associado à ação de carga de trabalho.</span><span class="sxs-lookup"><span data-stu-id="38900-133">The service associated with workload action.</span></span> <span data-ttu-id="38900-134">Opcional.</span><span class="sxs-lookup"><span data-stu-id="38900-134">Optional.</span></span> <span data-ttu-id="38900-135">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="38900-135">Read-only.</span></span>|
|<span data-ttu-id="38900-136">configurações</span><span class="sxs-lookup"><span data-stu-id="38900-136">settings</span></span>|<span data-ttu-id="38900-137">[coleção microsoft.graph.managedTenants.setting](../resources/managedtenants-setting.md)</span><span class="sxs-lookup"><span data-stu-id="38900-137">[microsoft.graph.managedTenants.setting](../resources/managedtenants-setting.md) collection</span></span>|<span data-ttu-id="38900-138">A coleção de configurações associadas à ação de carga de trabalho.</span><span class="sxs-lookup"><span data-stu-id="38900-138">The collection of settings associated with the workload action.</span></span> <span data-ttu-id="38900-139">Opcional.</span><span class="sxs-lookup"><span data-stu-id="38900-139">Optional.</span></span> <span data-ttu-id="38900-140">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="38900-140">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="38900-141">Relações</span><span class="sxs-lookup"><span data-stu-id="38900-141">Relationships</span></span>
<span data-ttu-id="38900-142">Nenhum</span><span class="sxs-lookup"><span data-stu-id="38900-142">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="38900-143">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="38900-143">JSON representation</span></span>
<span data-ttu-id="38900-144">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="38900-144">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managedTenants.workloadAction"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.workloadAction",
  "actionId": "String",
  "category": "String",
  "displayName": "String",
  "description": "String",
  "service": "String",
  "settings": [
    {
      "@odata.type": "microsoft.graph.managedTenants.setting"
    }
  ]
}
```
