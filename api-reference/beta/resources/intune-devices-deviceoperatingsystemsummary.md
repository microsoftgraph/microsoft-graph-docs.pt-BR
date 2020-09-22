---
title: Tipo de recurso deviceOperatingSystemSummary
description: Resumo do sistema operacional do dispositivo.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 8979a669638d511729817f6835afd894e155b796
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48081486"
---
# <a name="deviceoperatingsystemsummary-resource-type"></a><span data-ttu-id="89f84-103">Tipo de recurso deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="89f84-103">deviceOperatingSystemSummary resource type</span></span>

<span data-ttu-id="89f84-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="89f84-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="89f84-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="89f84-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="89f84-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="89f84-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="89f84-107">Resumo do sistema operacional do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="89f84-107">Device operating system summary.</span></span>

## <a name="properties"></a><span data-ttu-id="89f84-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="89f84-108">Properties</span></span>
|<span data-ttu-id="89f84-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="89f84-109">Property</span></span>|<span data-ttu-id="89f84-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="89f84-110">Type</span></span>|<span data-ttu-id="89f84-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="89f84-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="89f84-112">androidCount</span><span class="sxs-lookup"><span data-stu-id="89f84-112">androidCount</span></span>|<span data-ttu-id="89f84-113">Int32</span><span class="sxs-lookup"><span data-stu-id="89f84-113">Int32</span></span>|<span data-ttu-id="89f84-114">Número da contagem de dispositivos Android.</span><span class="sxs-lookup"><span data-stu-id="89f84-114">Number of android device count.</span></span>|
|<span data-ttu-id="89f84-115">iosCount</span><span class="sxs-lookup"><span data-stu-id="89f84-115">iosCount</span></span>|<span data-ttu-id="89f84-116">Int32</span><span class="sxs-lookup"><span data-stu-id="89f84-116">Int32</span></span>|<span data-ttu-id="89f84-117">Número da contagem de dispositivo iOS.</span><span class="sxs-lookup"><span data-stu-id="89f84-117">Number of iOS device count.</span></span>|
|<span data-ttu-id="89f84-118">macOSCount</span><span class="sxs-lookup"><span data-stu-id="89f84-118">macOSCount</span></span>|<span data-ttu-id="89f84-119">Int32</span><span class="sxs-lookup"><span data-stu-id="89f84-119">Int32</span></span>|<span data-ttu-id="89f84-120">Número da contagem de dispositivos Mac OS X.</span><span class="sxs-lookup"><span data-stu-id="89f84-120">Number of Mac OS X device count.</span></span>|
|<span data-ttu-id="89f84-121">windowsMobileCount</span><span class="sxs-lookup"><span data-stu-id="89f84-121">windowsMobileCount</span></span>|<span data-ttu-id="89f84-122">Int32</span><span class="sxs-lookup"><span data-stu-id="89f84-122">Int32</span></span>|<span data-ttu-id="89f84-123">Número da contagem de dispositivos móveis Windows.</span><span class="sxs-lookup"><span data-stu-id="89f84-123">Number of Windows mobile device count.</span></span>|
|<span data-ttu-id="89f84-124">windowsCount</span><span class="sxs-lookup"><span data-stu-id="89f84-124">windowsCount</span></span>|<span data-ttu-id="89f84-125">Int32</span><span class="sxs-lookup"><span data-stu-id="89f84-125">Int32</span></span>|<span data-ttu-id="89f84-126">Número da contagem de dispositivos Windows.</span><span class="sxs-lookup"><span data-stu-id="89f84-126">Number of Windows device count.</span></span>|
|<span data-ttu-id="89f84-127">unknownCount</span><span class="sxs-lookup"><span data-stu-id="89f84-127">unknownCount</span></span>|<span data-ttu-id="89f84-128">Int32</span><span class="sxs-lookup"><span data-stu-id="89f84-128">Int32</span></span>|<span data-ttu-id="89f84-129">Número da contagem de dispositivos desconhecidos.</span><span class="sxs-lookup"><span data-stu-id="89f84-129">Number of unknown device count.</span></span>|
|<span data-ttu-id="89f84-130">androidDedicatedCount</span><span class="sxs-lookup"><span data-stu-id="89f84-130">androidDedicatedCount</span></span>|<span data-ttu-id="89f84-131">Int32</span><span class="sxs-lookup"><span data-stu-id="89f84-131">Int32</span></span>|<span data-ttu-id="89f84-132">Número de dispositivos Android dedicados.</span><span class="sxs-lookup"><span data-stu-id="89f84-132">Number of dedicated Android devices.</span></span>|
|<span data-ttu-id="89f84-133">androidDeviceAdminCount</span><span class="sxs-lookup"><span data-stu-id="89f84-133">androidDeviceAdminCount</span></span>|<span data-ttu-id="89f84-134">Int32</span><span class="sxs-lookup"><span data-stu-id="89f84-134">Int32</span></span>|<span data-ttu-id="89f84-135">Número de dispositivos Android de administrador de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="89f84-135">Number of device admin Android devices.</span></span>|
|<span data-ttu-id="89f84-136">androidFullyManagedCount</span><span class="sxs-lookup"><span data-stu-id="89f84-136">androidFullyManagedCount</span></span>|<span data-ttu-id="89f84-137">Int32</span><span class="sxs-lookup"><span data-stu-id="89f84-137">Int32</span></span>|<span data-ttu-id="89f84-138">Número de dispositivos Android totalmente gerenciados.</span><span class="sxs-lookup"><span data-stu-id="89f84-138">Number of fully managed Android devices.</span></span>|
|<span data-ttu-id="89f84-139">androidWorkProfileCount</span><span class="sxs-lookup"><span data-stu-id="89f84-139">androidWorkProfileCount</span></span>|<span data-ttu-id="89f84-140">Int32</span><span class="sxs-lookup"><span data-stu-id="89f84-140">Int32</span></span>|<span data-ttu-id="89f84-141">Número de dispositivos Android de perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="89f84-141">Number of work profile Android devices.</span></span>|
|<span data-ttu-id="89f84-142">androidCorporateWorkProfileCount</span><span class="sxs-lookup"><span data-stu-id="89f84-142">androidCorporateWorkProfileCount</span></span>|<span data-ttu-id="89f84-143">Int32</span><span class="sxs-lookup"><span data-stu-id="89f84-143">Int32</span></span>|<span data-ttu-id="89f84-144">A contagem de dispositivos Android do perfil corporativo de trabalho.</span><span class="sxs-lookup"><span data-stu-id="89f84-144">The count of Corporate work profile Android devices.</span></span> <span data-ttu-id="89f84-145">Também conhecido como pessoal de propriedade corporativa (lidar).</span><span class="sxs-lookup"><span data-stu-id="89f84-145">Also known as Corporate Owned Personally Enabled (COPE).</span></span> <span data-ttu-id="89f84-146">Valores válidos-1 a 2147483647</span><span class="sxs-lookup"><span data-stu-id="89f84-146">Valid values -1 to 2147483647</span></span>|
|<span data-ttu-id="89f84-147">configMgrDeviceCount</span><span class="sxs-lookup"><span data-stu-id="89f84-147">configMgrDeviceCount</span></span>|<span data-ttu-id="89f84-148">Int32</span><span class="sxs-lookup"><span data-stu-id="89f84-148">Int32</span></span>|<span data-ttu-id="89f84-149">Número de dispositivos gerenciados pelo ConfigMgr.</span><span class="sxs-lookup"><span data-stu-id="89f84-149">Number of ConfigMgr managed devices.</span></span>|
|<span data-ttu-id="89f84-150">aospUserlessCount</span><span class="sxs-lookup"><span data-stu-id="89f84-150">aospUserlessCount</span></span>|<span data-ttu-id="89f84-151">Int32</span><span class="sxs-lookup"><span data-stu-id="89f84-151">Int32</span></span>|<span data-ttu-id="89f84-152">Número de dispositivos Android AOSP dedicados.</span><span class="sxs-lookup"><span data-stu-id="89f84-152">Number of AOSP dedicated Android devices.</span></span> <span data-ttu-id="89f84-153">Valores válidos de 0 a 2147483647</span><span class="sxs-lookup"><span data-stu-id="89f84-153">Valid values 0 to 2147483647</span></span>|

## <a name="relationships"></a><span data-ttu-id="89f84-154">Relações</span><span class="sxs-lookup"><span data-stu-id="89f84-154">Relationships</span></span>
<span data-ttu-id="89f84-155">Nenhum</span><span class="sxs-lookup"><span data-stu-id="89f84-155">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="89f84-156">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="89f84-156">JSON Representation</span></span>
<span data-ttu-id="89f84-157">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="89f84-157">Here is a JSON representation of the resource.</span></span>
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
  "androidCorporateWorkProfileCount": 1024,
  "configMgrDeviceCount": 1024,
  "aospUserlessCount": 1024
}
```






