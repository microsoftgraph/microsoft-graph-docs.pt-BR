---
title: Tipo de recurso deviceOperatingSystemSummary
description: Resumo do sistema operacional do dispositivo.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 01965c1dfaeb04d05d2dc6293fc449c0bbc878fe
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50157635"
---
# <a name="deviceoperatingsystemsummary-resource-type"></a><span data-ttu-id="22a16-103">Tipo de recurso deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="22a16-103">deviceOperatingSystemSummary resource type</span></span>

<span data-ttu-id="22a16-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="22a16-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="22a16-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="22a16-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="22a16-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="22a16-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="22a16-107">Resumo do sistema operacional do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="22a16-107">Device operating system summary.</span></span>

## <a name="properties"></a><span data-ttu-id="22a16-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="22a16-108">Properties</span></span>
|<span data-ttu-id="22a16-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="22a16-109">Property</span></span>|<span data-ttu-id="22a16-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="22a16-110">Type</span></span>|<span data-ttu-id="22a16-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="22a16-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="22a16-112">androidCount</span><span class="sxs-lookup"><span data-stu-id="22a16-112">androidCount</span></span>|<span data-ttu-id="22a16-113">Int32</span><span class="sxs-lookup"><span data-stu-id="22a16-113">Int32</span></span>|<span data-ttu-id="22a16-114">Número da contagem de dispositivos Android.</span><span class="sxs-lookup"><span data-stu-id="22a16-114">Number of android device count.</span></span>|
|<span data-ttu-id="22a16-115">iosCount</span><span class="sxs-lookup"><span data-stu-id="22a16-115">iosCount</span></span>|<span data-ttu-id="22a16-116">Int32</span><span class="sxs-lookup"><span data-stu-id="22a16-116">Int32</span></span>|<span data-ttu-id="22a16-117">Número da contagem de dispositivo iOS.</span><span class="sxs-lookup"><span data-stu-id="22a16-117">Number of iOS device count.</span></span>|
|<span data-ttu-id="22a16-118">macOSCount</span><span class="sxs-lookup"><span data-stu-id="22a16-118">macOSCount</span></span>|<span data-ttu-id="22a16-119">Int32</span><span class="sxs-lookup"><span data-stu-id="22a16-119">Int32</span></span>|<span data-ttu-id="22a16-120">Número da contagem de dispositivos Mac OS X.</span><span class="sxs-lookup"><span data-stu-id="22a16-120">Number of Mac OS X device count.</span></span>|
|<span data-ttu-id="22a16-121">windowsMobileCount</span><span class="sxs-lookup"><span data-stu-id="22a16-121">windowsMobileCount</span></span>|<span data-ttu-id="22a16-122">Int32</span><span class="sxs-lookup"><span data-stu-id="22a16-122">Int32</span></span>|<span data-ttu-id="22a16-123">Número da contagem de dispositivos móveis Windows.</span><span class="sxs-lookup"><span data-stu-id="22a16-123">Number of Windows mobile device count.</span></span>|
|<span data-ttu-id="22a16-124">windowsCount</span><span class="sxs-lookup"><span data-stu-id="22a16-124">windowsCount</span></span>|<span data-ttu-id="22a16-125">Int32</span><span class="sxs-lookup"><span data-stu-id="22a16-125">Int32</span></span>|<span data-ttu-id="22a16-126">Número da contagem de dispositivos Windows.</span><span class="sxs-lookup"><span data-stu-id="22a16-126">Number of Windows device count.</span></span>|
|<span data-ttu-id="22a16-127">unknownCount</span><span class="sxs-lookup"><span data-stu-id="22a16-127">unknownCount</span></span>|<span data-ttu-id="22a16-128">Int32</span><span class="sxs-lookup"><span data-stu-id="22a16-128">Int32</span></span>|<span data-ttu-id="22a16-129">Número da contagem de dispositivos desconhecidos.</span><span class="sxs-lookup"><span data-stu-id="22a16-129">Number of unknown device count.</span></span>|
|<span data-ttu-id="22a16-130">androidDedicatedCount</span><span class="sxs-lookup"><span data-stu-id="22a16-130">androidDedicatedCount</span></span>|<span data-ttu-id="22a16-131">Int32</span><span class="sxs-lookup"><span data-stu-id="22a16-131">Int32</span></span>|<span data-ttu-id="22a16-132">Número de dispositivos Android dedicados.</span><span class="sxs-lookup"><span data-stu-id="22a16-132">Number of dedicated Android devices.</span></span>|
|<span data-ttu-id="22a16-133">androidDeviceAdminCount</span><span class="sxs-lookup"><span data-stu-id="22a16-133">androidDeviceAdminCount</span></span>|<span data-ttu-id="22a16-134">Int32</span><span class="sxs-lookup"><span data-stu-id="22a16-134">Int32</span></span>|<span data-ttu-id="22a16-135">Número de dispositivos Android de administração de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="22a16-135">Number of device admin Android devices.</span></span>|
|<span data-ttu-id="22a16-136">androidFullyManagedCount</span><span class="sxs-lookup"><span data-stu-id="22a16-136">androidFullyManagedCount</span></span>|<span data-ttu-id="22a16-137">Int32</span><span class="sxs-lookup"><span data-stu-id="22a16-137">Int32</span></span>|<span data-ttu-id="22a16-138">Número de dispositivos Android totalmente gerenciados.</span><span class="sxs-lookup"><span data-stu-id="22a16-138">Number of fully managed Android devices.</span></span>|
|<span data-ttu-id="22a16-139">androidWorkProfileCount</span><span class="sxs-lookup"><span data-stu-id="22a16-139">androidWorkProfileCount</span></span>|<span data-ttu-id="22a16-140">Int32</span><span class="sxs-lookup"><span data-stu-id="22a16-140">Int32</span></span>|<span data-ttu-id="22a16-141">Número de dispositivos Android de perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="22a16-141">Number of work profile Android devices.</span></span>|
|<span data-ttu-id="22a16-142">androidCorporateWorkProfileCount</span><span class="sxs-lookup"><span data-stu-id="22a16-142">androidCorporateWorkProfileCount</span></span>|<span data-ttu-id="22a16-143">Int32</span><span class="sxs-lookup"><span data-stu-id="22a16-143">Int32</span></span>|<span data-ttu-id="22a16-144">A contagem de dispositivos Android de perfil de trabalho corporativo.</span><span class="sxs-lookup"><span data-stu-id="22a16-144">The count of Corporate work profile Android devices.</span></span> <span data-ttu-id="22a16-145">Também conhecido como Corporate Owned Personally Enabled (COPE).</span><span class="sxs-lookup"><span data-stu-id="22a16-145">Also known as Corporate Owned Personally Enabled (COPE).</span></span> <span data-ttu-id="22a16-146">Valores válidos -1 a 2147483647</span><span class="sxs-lookup"><span data-stu-id="22a16-146">Valid values -1 to 2147483647</span></span>|
|<span data-ttu-id="22a16-147">configMgrDeviceCount</span><span class="sxs-lookup"><span data-stu-id="22a16-147">configMgrDeviceCount</span></span>|<span data-ttu-id="22a16-148">Int32</span><span class="sxs-lookup"><span data-stu-id="22a16-148">Int32</span></span>|<span data-ttu-id="22a16-149">Número de dispositivos gerenciados pelo ConfigMgr.</span><span class="sxs-lookup"><span data-stu-id="22a16-149">Number of ConfigMgr managed devices.</span></span>|
|<span data-ttu-id="22a16-150">aospUserlessCount</span><span class="sxs-lookup"><span data-stu-id="22a16-150">aospUserlessCount</span></span>|<span data-ttu-id="22a16-151">Int32</span><span class="sxs-lookup"><span data-stu-id="22a16-151">Int32</span></span>|<span data-ttu-id="22a16-152">Número de dispositivos Android sem usuário AOSP.</span><span class="sxs-lookup"><span data-stu-id="22a16-152">Number of AOSP userless Android devices.</span></span> <span data-ttu-id="22a16-153">Valores válidos de 0 a 2147483647</span><span class="sxs-lookup"><span data-stu-id="22a16-153">Valid values 0 to 2147483647</span></span>|
|<span data-ttu-id="22a16-154">aospUserAssociatedCount</span><span class="sxs-lookup"><span data-stu-id="22a16-154">aospUserAssociatedCount</span></span>|<span data-ttu-id="22a16-155">Int32</span><span class="sxs-lookup"><span data-stu-id="22a16-155">Int32</span></span>|<span data-ttu-id="22a16-156">Número de dispositivos Android associados ao usuário AOSP.</span><span class="sxs-lookup"><span data-stu-id="22a16-156">Number of AOSP user-associated Android devices.</span></span> <span data-ttu-id="22a16-157">Valores válidos de 0 a 2147483647</span><span class="sxs-lookup"><span data-stu-id="22a16-157">Valid values 0 to 2147483647</span></span>|

## <a name="relationships"></a><span data-ttu-id="22a16-158">Relações</span><span class="sxs-lookup"><span data-stu-id="22a16-158">Relationships</span></span>
<span data-ttu-id="22a16-159">Nenhum</span><span class="sxs-lookup"><span data-stu-id="22a16-159">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="22a16-160">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="22a16-160">JSON Representation</span></span>
<span data-ttu-id="22a16-161">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="22a16-161">Here is a JSON representation of the resource.</span></span>
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
  "aospUserlessCount": 1024,
  "aospUserAssociatedCount": 1024
}
```




