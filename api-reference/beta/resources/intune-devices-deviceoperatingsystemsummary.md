---
title: Tipo de recurso deviceOperatingSystemSummary
description: Resumo do sistema operacional do dispositivo.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 2b1a49496357a3688bd9f484d8759fdd0c2140eb
ms.sourcegitcommit: f3dda172d95ef1eda8f6dd9e3ffdc7d3c0744c0a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/14/2020
ms.locfileid: "45122627"
---
# <a name="deviceoperatingsystemsummary-resource-type"></a><span data-ttu-id="154aa-103">Tipo de recurso deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="154aa-103">deviceOperatingSystemSummary resource type</span></span>

<span data-ttu-id="154aa-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="154aa-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="154aa-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="154aa-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="154aa-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="154aa-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="154aa-107">Resumo do sistema operacional do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="154aa-107">Device operating system summary.</span></span>

## <a name="properties"></a><span data-ttu-id="154aa-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="154aa-108">Properties</span></span>
|<span data-ttu-id="154aa-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="154aa-109">Property</span></span>|<span data-ttu-id="154aa-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="154aa-110">Type</span></span>|<span data-ttu-id="154aa-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="154aa-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="154aa-112">androidCount</span><span class="sxs-lookup"><span data-stu-id="154aa-112">androidCount</span></span>|<span data-ttu-id="154aa-113">Int32</span><span class="sxs-lookup"><span data-stu-id="154aa-113">Int32</span></span>|<span data-ttu-id="154aa-114">Número da contagem de dispositivos Android.</span><span class="sxs-lookup"><span data-stu-id="154aa-114">Number of android device count.</span></span>|
|<span data-ttu-id="154aa-115">iosCount</span><span class="sxs-lookup"><span data-stu-id="154aa-115">iosCount</span></span>|<span data-ttu-id="154aa-116">Int32</span><span class="sxs-lookup"><span data-stu-id="154aa-116">Int32</span></span>|<span data-ttu-id="154aa-117">Número da contagem de dispositivo iOS.</span><span class="sxs-lookup"><span data-stu-id="154aa-117">Number of iOS device count.</span></span>|
|<span data-ttu-id="154aa-118">macOSCount</span><span class="sxs-lookup"><span data-stu-id="154aa-118">macOSCount</span></span>|<span data-ttu-id="154aa-119">Int32</span><span class="sxs-lookup"><span data-stu-id="154aa-119">Int32</span></span>|<span data-ttu-id="154aa-120">Número da contagem de dispositivos Mac OS X.</span><span class="sxs-lookup"><span data-stu-id="154aa-120">Number of Mac OS X device count.</span></span>|
|<span data-ttu-id="154aa-121">windowsMobileCount</span><span class="sxs-lookup"><span data-stu-id="154aa-121">windowsMobileCount</span></span>|<span data-ttu-id="154aa-122">Int32</span><span class="sxs-lookup"><span data-stu-id="154aa-122">Int32</span></span>|<span data-ttu-id="154aa-123">Número da contagem de dispositivos móveis Windows.</span><span class="sxs-lookup"><span data-stu-id="154aa-123">Number of Windows mobile device count.</span></span>|
|<span data-ttu-id="154aa-124">windowsCount</span><span class="sxs-lookup"><span data-stu-id="154aa-124">windowsCount</span></span>|<span data-ttu-id="154aa-125">Int32</span><span class="sxs-lookup"><span data-stu-id="154aa-125">Int32</span></span>|<span data-ttu-id="154aa-126">Número da contagem de dispositivos Windows.</span><span class="sxs-lookup"><span data-stu-id="154aa-126">Number of Windows device count.</span></span>|
|<span data-ttu-id="154aa-127">unknownCount</span><span class="sxs-lookup"><span data-stu-id="154aa-127">unknownCount</span></span>|<span data-ttu-id="154aa-128">Int32</span><span class="sxs-lookup"><span data-stu-id="154aa-128">Int32</span></span>|<span data-ttu-id="154aa-129">Número da contagem de dispositivos desconhecidos.</span><span class="sxs-lookup"><span data-stu-id="154aa-129">Number of unknown device count.</span></span>|
|<span data-ttu-id="154aa-130">androidDedicatedCount</span><span class="sxs-lookup"><span data-stu-id="154aa-130">androidDedicatedCount</span></span>|<span data-ttu-id="154aa-131">Int32</span><span class="sxs-lookup"><span data-stu-id="154aa-131">Int32</span></span>|<span data-ttu-id="154aa-132">Número de dispositivos Android dedicados.</span><span class="sxs-lookup"><span data-stu-id="154aa-132">Number of dedicated Android devices.</span></span>|
|<span data-ttu-id="154aa-133">androidDeviceAdminCount</span><span class="sxs-lookup"><span data-stu-id="154aa-133">androidDeviceAdminCount</span></span>|<span data-ttu-id="154aa-134">Int32</span><span class="sxs-lookup"><span data-stu-id="154aa-134">Int32</span></span>|<span data-ttu-id="154aa-135">Número de dispositivos Android de administrador de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="154aa-135">Number of device admin Android devices.</span></span>|
|<span data-ttu-id="154aa-136">androidFullyManagedCount</span><span class="sxs-lookup"><span data-stu-id="154aa-136">androidFullyManagedCount</span></span>|<span data-ttu-id="154aa-137">Int32</span><span class="sxs-lookup"><span data-stu-id="154aa-137">Int32</span></span>|<span data-ttu-id="154aa-138">Número de dispositivos Android totalmente gerenciados.</span><span class="sxs-lookup"><span data-stu-id="154aa-138">Number of fully managed Android devices.</span></span>|
|<span data-ttu-id="154aa-139">androidWorkProfileCount</span><span class="sxs-lookup"><span data-stu-id="154aa-139">androidWorkProfileCount</span></span>|<span data-ttu-id="154aa-140">Int32</span><span class="sxs-lookup"><span data-stu-id="154aa-140">Int32</span></span>|<span data-ttu-id="154aa-141">Número de dispositivos Android de perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="154aa-141">Number of work profile Android devices.</span></span>|
|<span data-ttu-id="154aa-142">androidCorporateWorkProfileCount</span><span class="sxs-lookup"><span data-stu-id="154aa-142">androidCorporateWorkProfileCount</span></span>|<span data-ttu-id="154aa-143">Int32</span><span class="sxs-lookup"><span data-stu-id="154aa-143">Int32</span></span>|<span data-ttu-id="154aa-144">A contagem de dispositivos Android do perfil corporativo de trabalho.</span><span class="sxs-lookup"><span data-stu-id="154aa-144">The count of Corporate work profile Android devices.</span></span> <span data-ttu-id="154aa-145">Também conhecido como pessoal de propriedade corporativa (lidar).</span><span class="sxs-lookup"><span data-stu-id="154aa-145">Also known as Corporate Owned Personally Enabled (COPE).</span></span> <span data-ttu-id="154aa-146">Valores válidos-1 a 2147483647</span><span class="sxs-lookup"><span data-stu-id="154aa-146">Valid values -1 to 2147483647</span></span>|
|<span data-ttu-id="154aa-147">configMgrDeviceCount</span><span class="sxs-lookup"><span data-stu-id="154aa-147">configMgrDeviceCount</span></span>|<span data-ttu-id="154aa-148">Int32</span><span class="sxs-lookup"><span data-stu-id="154aa-148">Int32</span></span>|<span data-ttu-id="154aa-149">Número de dispositivos gerenciados pelo ConfigMgr.</span><span class="sxs-lookup"><span data-stu-id="154aa-149">Number of ConfigMgr managed devices.</span></span>|

## <a name="relationships"></a><span data-ttu-id="154aa-150">Relações</span><span class="sxs-lookup"><span data-stu-id="154aa-150">Relationships</span></span>
<span data-ttu-id="154aa-151">Nenhum</span><span class="sxs-lookup"><span data-stu-id="154aa-151">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="154aa-152">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="154aa-152">JSON Representation</span></span>
<span data-ttu-id="154aa-153">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="154aa-153">Here is a JSON representation of the resource.</span></span>
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
  "configMgrDeviceCount": 1024
}
```



