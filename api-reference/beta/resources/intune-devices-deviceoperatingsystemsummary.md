---
title: Tipo de recurso deviceOperatingSystemSummary
description: Resumo do sistema operacional do dispositivo.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 1c15adc462742adb734a503f55dc69af48bf0f82
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43470737"
---
# <a name="deviceoperatingsystemsummary-resource-type"></a><span data-ttu-id="779a6-103">Tipo de recurso deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="779a6-103">deviceOperatingSystemSummary resource type</span></span>

<span data-ttu-id="779a6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="779a6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="779a6-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="779a6-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="779a6-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="779a6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="779a6-107">Resumo do sistema operacional do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="779a6-107">Device operating system summary.</span></span>

## <a name="properties"></a><span data-ttu-id="779a6-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="779a6-108">Properties</span></span>
|<span data-ttu-id="779a6-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="779a6-109">Property</span></span>|<span data-ttu-id="779a6-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="779a6-110">Type</span></span>|<span data-ttu-id="779a6-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="779a6-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="779a6-112">androidCount</span><span class="sxs-lookup"><span data-stu-id="779a6-112">androidCount</span></span>|<span data-ttu-id="779a6-113">Int32</span><span class="sxs-lookup"><span data-stu-id="779a6-113">Int32</span></span>|<span data-ttu-id="779a6-114">Número da contagem de dispositivos Android.</span><span class="sxs-lookup"><span data-stu-id="779a6-114">Number of android device count.</span></span>|
|<span data-ttu-id="779a6-115">iosCount</span><span class="sxs-lookup"><span data-stu-id="779a6-115">iosCount</span></span>|<span data-ttu-id="779a6-116">Int32</span><span class="sxs-lookup"><span data-stu-id="779a6-116">Int32</span></span>|<span data-ttu-id="779a6-117">Número da contagem de dispositivo iOS.</span><span class="sxs-lookup"><span data-stu-id="779a6-117">Number of iOS device count.</span></span>|
|<span data-ttu-id="779a6-118">macOSCount</span><span class="sxs-lookup"><span data-stu-id="779a6-118">macOSCount</span></span>|<span data-ttu-id="779a6-119">Int32</span><span class="sxs-lookup"><span data-stu-id="779a6-119">Int32</span></span>|<span data-ttu-id="779a6-120">Número da contagem de dispositivos Mac OS X.</span><span class="sxs-lookup"><span data-stu-id="779a6-120">Number of Mac OS X device count.</span></span>|
|<span data-ttu-id="779a6-121">windowsMobileCount</span><span class="sxs-lookup"><span data-stu-id="779a6-121">windowsMobileCount</span></span>|<span data-ttu-id="779a6-122">Int32</span><span class="sxs-lookup"><span data-stu-id="779a6-122">Int32</span></span>|<span data-ttu-id="779a6-123">Número da contagem de dispositivos móveis Windows.</span><span class="sxs-lookup"><span data-stu-id="779a6-123">Number of Windows mobile device count.</span></span>|
|<span data-ttu-id="779a6-124">windowsCount</span><span class="sxs-lookup"><span data-stu-id="779a6-124">windowsCount</span></span>|<span data-ttu-id="779a6-125">Int32</span><span class="sxs-lookup"><span data-stu-id="779a6-125">Int32</span></span>|<span data-ttu-id="779a6-126">Número da contagem de dispositivos Windows.</span><span class="sxs-lookup"><span data-stu-id="779a6-126">Number of Windows device count.</span></span>|
|<span data-ttu-id="779a6-127">unknownCount</span><span class="sxs-lookup"><span data-stu-id="779a6-127">unknownCount</span></span>|<span data-ttu-id="779a6-128">Int32</span><span class="sxs-lookup"><span data-stu-id="779a6-128">Int32</span></span>|<span data-ttu-id="779a6-129">Número da contagem de dispositivos desconhecidos.</span><span class="sxs-lookup"><span data-stu-id="779a6-129">Number of unknown device count.</span></span>|
|<span data-ttu-id="779a6-130">androidDedicatedCount</span><span class="sxs-lookup"><span data-stu-id="779a6-130">androidDedicatedCount</span></span>|<span data-ttu-id="779a6-131">Int32</span><span class="sxs-lookup"><span data-stu-id="779a6-131">Int32</span></span>|<span data-ttu-id="779a6-132">Número de dispositivos Android dedicados.</span><span class="sxs-lookup"><span data-stu-id="779a6-132">Number of dedicated Android devices.</span></span>|
|<span data-ttu-id="779a6-133">androidDeviceAdminCount</span><span class="sxs-lookup"><span data-stu-id="779a6-133">androidDeviceAdminCount</span></span>|<span data-ttu-id="779a6-134">Int32</span><span class="sxs-lookup"><span data-stu-id="779a6-134">Int32</span></span>|<span data-ttu-id="779a6-135">Número de dispositivos Android de administrador de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="779a6-135">Number of device admin Android devices.</span></span>|
|<span data-ttu-id="779a6-136">androidFullyManagedCount</span><span class="sxs-lookup"><span data-stu-id="779a6-136">androidFullyManagedCount</span></span>|<span data-ttu-id="779a6-137">Int32</span><span class="sxs-lookup"><span data-stu-id="779a6-137">Int32</span></span>|<span data-ttu-id="779a6-138">Número de dispositivos Android totalmente gerenciados.</span><span class="sxs-lookup"><span data-stu-id="779a6-138">Number of fully managed Android devices.</span></span>|
|<span data-ttu-id="779a6-139">androidWorkProfileCount</span><span class="sxs-lookup"><span data-stu-id="779a6-139">androidWorkProfileCount</span></span>|<span data-ttu-id="779a6-140">Int32</span><span class="sxs-lookup"><span data-stu-id="779a6-140">Int32</span></span>|<span data-ttu-id="779a6-141">Número de dispositivos Android de perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="779a6-141">Number of work profile Android devices.</span></span>|
|<span data-ttu-id="779a6-142">configMgrDeviceCount</span><span class="sxs-lookup"><span data-stu-id="779a6-142">configMgrDeviceCount</span></span>|<span data-ttu-id="779a6-143">Int32</span><span class="sxs-lookup"><span data-stu-id="779a6-143">Int32</span></span>|<span data-ttu-id="779a6-144">Número de dispositivos gerenciados pelo ConfigMgr.</span><span class="sxs-lookup"><span data-stu-id="779a6-144">Number of ConfigMgr managed devices.</span></span>|

## <a name="relationships"></a><span data-ttu-id="779a6-145">Relações</span><span class="sxs-lookup"><span data-stu-id="779a6-145">Relationships</span></span>
<span data-ttu-id="779a6-146">Nenhum</span><span class="sxs-lookup"><span data-stu-id="779a6-146">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="779a6-147">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="779a6-147">JSON Representation</span></span>
<span data-ttu-id="779a6-148">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="779a6-148">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceOperatingSystemSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceOperatingSystemSummary",
  "androidCount": 1024,
  "iosCount": 1024,
  "macOSCount": 1024,
  "windowsMobileCount": 1024,
  "windowsCount": 1024,
  "unknownCount": 1024,
  "androidDedicatedCount": 1024,
  "androidDeviceAdminCount": 1024,
  "androidFullyManagedCount": 1024,
  "androidWorkProfileCount": 1024,
  "configMgrDeviceCount": 1024
}
```



