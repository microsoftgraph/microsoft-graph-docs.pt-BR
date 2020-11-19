---
title: tipo de recurso configManagerPolicySummary
description: Um resumo da política de Configmanager.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: c63e85448b70abc76f4df0021c4f5516e778ebe0
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49301410"
---
# <a name="configmanagerpolicysummary-resource-type"></a><span data-ttu-id="a806f-103">tipo de recurso configManagerPolicySummary</span><span class="sxs-lookup"><span data-stu-id="a806f-103">configManagerPolicySummary resource type</span></span>

<span data-ttu-id="a806f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a806f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a806f-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a806f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a806f-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a806f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a806f-107">Um resumo da política de Configmanager.</span><span class="sxs-lookup"><span data-stu-id="a806f-107">A ConfigManager policy summary.</span></span>

## <a name="properties"></a><span data-ttu-id="a806f-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a806f-108">Properties</span></span>
|<span data-ttu-id="a806f-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a806f-109">Property</span></span>|<span data-ttu-id="a806f-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="a806f-110">Type</span></span>|<span data-ttu-id="a806f-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="a806f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a806f-112">targetedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a806f-112">targetedDeviceCount</span></span>|<span data-ttu-id="a806f-113">Int32</span><span class="sxs-lookup"><span data-stu-id="a806f-113">Int32</span></span>|<span data-ttu-id="a806f-114">O número de dispositivos direcionados pela política.</span><span class="sxs-lookup"><span data-stu-id="a806f-114">The number of devices targeted by the policy.</span></span>|
|<span data-ttu-id="a806f-115">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a806f-115">compliantDeviceCount</span></span>|<span data-ttu-id="a806f-116">Int32</span><span class="sxs-lookup"><span data-stu-id="a806f-116">Int32</span></span>|<span data-ttu-id="a806f-117">O número de dispositivos avaliados para serem compatíveis com a política.</span><span class="sxs-lookup"><span data-stu-id="a806f-117">The number of devices evaluated to be compliant by the policy.</span></span>|
|<span data-ttu-id="a806f-118">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a806f-118">nonCompliantDeviceCount</span></span>|<span data-ttu-id="a806f-119">Int32</span><span class="sxs-lookup"><span data-stu-id="a806f-119">Int32</span></span>|<span data-ttu-id="a806f-120">O número de dispositivos avaliados não são compatíveis com a política.</span><span class="sxs-lookup"><span data-stu-id="a806f-120">The number of devices evaluated to be noncompliant by the policy.</span></span>|
|<span data-ttu-id="a806f-121">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a806f-121">failedDeviceCount</span></span>|<span data-ttu-id="a806f-122">Int32</span><span class="sxs-lookup"><span data-stu-id="a806f-122">Int32</span></span>|<span data-ttu-id="a806f-123">O número de dispositivos que não puderam ser avaliados pela política.</span><span class="sxs-lookup"><span data-stu-id="a806f-123">The number of devices that failed to be evaluated by the policy.</span></span>|
|<span data-ttu-id="a806f-124">pendingDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a806f-124">pendingDeviceCount</span></span>|<span data-ttu-id="a806f-125">Int32</span><span class="sxs-lookup"><span data-stu-id="a806f-125">Int32</span></span>|<span data-ttu-id="a806f-126">O número de dispositivos que confirmaram a política, mas têm avaliação pendente.</span><span class="sxs-lookup"><span data-stu-id="a806f-126">The number of devices that have acknowledged the policy but are pending evaluation.</span></span>|
|<span data-ttu-id="a806f-127">enforcedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a806f-127">enforcedDeviceCount</span></span>|<span data-ttu-id="a806f-128">Int32</span><span class="sxs-lookup"><span data-stu-id="a806f-128">Int32</span></span>|<span data-ttu-id="a806f-129">O número de dispositivos que foram corrigidos pela política.</span><span class="sxs-lookup"><span data-stu-id="a806f-129">The number of devices that have have been remediated by the policy.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a806f-130">Relações</span><span class="sxs-lookup"><span data-stu-id="a806f-130">Relationships</span></span>
<span data-ttu-id="a806f-131">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a806f-131">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a806f-132">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a806f-132">JSON Representation</span></span>
<span data-ttu-id="a806f-133">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a806f-133">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.configManagerPolicySummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.configManagerPolicySummary",
  "targetedDeviceCount": 1024,
  "compliantDeviceCount": 1024,
  "nonCompliantDeviceCount": 1024,
  "failedDeviceCount": 1024,
  "pendingDeviceCount": 1024,
  "enforcedDeviceCount": 1024
}
```




