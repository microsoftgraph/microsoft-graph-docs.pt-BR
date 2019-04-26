---
title: tipo de recurso mobileAppInstallSummary
description: Contém propriedades para o resumo de instalação de um aplicativo móvel.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a981477daefae92b6afcd3612a173d75b37e8637
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32551866"
---
# <a name="mobileappinstallsummary-resource-type"></a><span data-ttu-id="e3cf8-103">tipo de recurso mobileAppInstallSummary</span><span class="sxs-lookup"><span data-stu-id="e3cf8-103">mobileAppInstallSummary resource type</span></span>

> <span data-ttu-id="e3cf8-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e3cf8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e3cf8-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e3cf8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e3cf8-106">Contém propriedades para o resumo de instalação de um aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="e3cf8-106">Contains properties for the installation summary of a mobile app.</span></span>

## <a name="methods"></a><span data-ttu-id="e3cf8-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="e3cf8-107">Methods</span></span>
|<span data-ttu-id="e3cf8-108">Método</span><span class="sxs-lookup"><span data-stu-id="e3cf8-108">Method</span></span>|<span data-ttu-id="e3cf8-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="e3cf8-109">Return Type</span></span>|<span data-ttu-id="e3cf8-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="e3cf8-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="e3cf8-111">Obter mobileAppInstallSummary</span><span class="sxs-lookup"><span data-stu-id="e3cf8-111">Get mobileAppInstallSummary</span></span>](../api/intune-apps-mobileappinstallsummary-get.md)|[<span data-ttu-id="e3cf8-112">mobileAppInstallSummary</span><span class="sxs-lookup"><span data-stu-id="e3cf8-112">mobileAppInstallSummary</span></span>](../resources/intune-apps-mobileappinstallsummary.md)|<span data-ttu-id="e3cf8-113">Leia as propriedades e as relações do objeto [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md) .</span><span class="sxs-lookup"><span data-stu-id="e3cf8-113">Read properties and relationships of the [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md) object.</span></span>|
|[<span data-ttu-id="e3cf8-114">Atualizar mobileAppInstallSummary</span><span class="sxs-lookup"><span data-stu-id="e3cf8-114">Update mobileAppInstallSummary</span></span>](../api/intune-apps-mobileappinstallsummary-update.md)|[<span data-ttu-id="e3cf8-115">mobileAppInstallSummary</span><span class="sxs-lookup"><span data-stu-id="e3cf8-115">mobileAppInstallSummary</span></span>](../resources/intune-apps-mobileappinstallsummary.md)|<span data-ttu-id="e3cf8-116">Atualiza as propriedades de um objeto [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md) .</span><span class="sxs-lookup"><span data-stu-id="e3cf8-116">Update the properties of a [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="e3cf8-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e3cf8-117">Properties</span></span>
|<span data-ttu-id="e3cf8-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e3cf8-118">Property</span></span>|<span data-ttu-id="e3cf8-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="e3cf8-119">Type</span></span>|<span data-ttu-id="e3cf8-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="e3cf8-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e3cf8-121">id</span><span class="sxs-lookup"><span data-stu-id="e3cf8-121">id</span></span>|<span data-ttu-id="e3cf8-122">String</span><span class="sxs-lookup"><span data-stu-id="e3cf8-122">String</span></span>|<span data-ttu-id="e3cf8-123">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="e3cf8-123">Key of the entity.</span></span>|
|<span data-ttu-id="e3cf8-124">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e3cf8-124">installedDeviceCount</span></span>|<span data-ttu-id="e3cf8-125">Int32</span><span class="sxs-lookup"><span data-stu-id="e3cf8-125">Int32</span></span>|<span data-ttu-id="e3cf8-126">Número de dispositivos que instalaram com êxito este aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e3cf8-126">Number of Devices that have successfully installed this app.</span></span>|
|<span data-ttu-id="e3cf8-127">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e3cf8-127">failedDeviceCount</span></span>|<span data-ttu-id="e3cf8-128">Int32</span><span class="sxs-lookup"><span data-stu-id="e3cf8-128">Int32</span></span>|<span data-ttu-id="e3cf8-129">Número de dispositivos que falharam ao instalar este aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e3cf8-129">Number of Devices that have failed to install this app.</span></span>|
|<span data-ttu-id="e3cf8-130">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e3cf8-130">notApplicableDeviceCount</span></span>|<span data-ttu-id="e3cf8-131">Int32</span><span class="sxs-lookup"><span data-stu-id="e3cf8-131">Int32</span></span>|<span data-ttu-id="e3cf8-132">Número de dispositivos que não se aplicam a este aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e3cf8-132">Number of Devices that are not applicable for this app.</span></span>|
|<span data-ttu-id="e3cf8-133">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e3cf8-133">notInstalledDeviceCount</span></span>|<span data-ttu-id="e3cf8-134">Int32</span><span class="sxs-lookup"><span data-stu-id="e3cf8-134">Int32</span></span>|<span data-ttu-id="e3cf8-135">Número de dispositivos que não possuem este aplicativo instalado.</span><span class="sxs-lookup"><span data-stu-id="e3cf8-135">Number of Devices that does not have this app installed.</span></span>|
|<span data-ttu-id="e3cf8-136">pendingInstallDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e3cf8-136">pendingInstallDeviceCount</span></span>|<span data-ttu-id="e3cf8-137">Int32</span><span class="sxs-lookup"><span data-stu-id="e3cf8-137">Int32</span></span>|<span data-ttu-id="e3cf8-138">Número de dispositivos que foram notificados para instalar este aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e3cf8-138">Number of Devices that have been notified to install this app.</span></span>|
|<span data-ttu-id="e3cf8-139">installedUserCount</span><span class="sxs-lookup"><span data-stu-id="e3cf8-139">installedUserCount</span></span>|<span data-ttu-id="e3cf8-140">Int32</span><span class="sxs-lookup"><span data-stu-id="e3cf8-140">Int32</span></span>|<span data-ttu-id="e3cf8-141">Número de usuários cujos dispositivos foram todos bem-sucedidos para instalar este aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e3cf8-141">Number of Users whose devices have all succeeded to install this app.</span></span>|
|<span data-ttu-id="e3cf8-142">failedUserCount</span><span class="sxs-lookup"><span data-stu-id="e3cf8-142">failedUserCount</span></span>|<span data-ttu-id="e3cf8-143">Int32</span><span class="sxs-lookup"><span data-stu-id="e3cf8-143">Int32</span></span>|<span data-ttu-id="e3cf8-144">Número de usuários que têm um ou mais dispositivos que não instalaram este aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e3cf8-144">Number of Users that have 1 or more device that failed to install this app.</span></span>|
|<span data-ttu-id="e3cf8-145">notApplicableUserCount</span><span class="sxs-lookup"><span data-stu-id="e3cf8-145">notApplicableUserCount</span></span>|<span data-ttu-id="e3cf8-146">Int32</span><span class="sxs-lookup"><span data-stu-id="e3cf8-146">Int32</span></span>|<span data-ttu-id="e3cf8-147">Número de usuários cujos dispositivos não são todos aplicáveis para este aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e3cf8-147">Number of Users whose devices were all not applicable for this app.</span></span>|
|<span data-ttu-id="e3cf8-148">notInstalledUserCount</span><span class="sxs-lookup"><span data-stu-id="e3cf8-148">notInstalledUserCount</span></span>|<span data-ttu-id="e3cf8-149">Int32</span><span class="sxs-lookup"><span data-stu-id="e3cf8-149">Int32</span></span>|<span data-ttu-id="e3cf8-150">Número de usuários que têm um ou mais dispositivos que não instalaram este aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e3cf8-150">Number of Users that have 1 or more devices that did not install this app.</span></span>|
|<span data-ttu-id="e3cf8-151">pendingInstallUserCount</span><span class="sxs-lookup"><span data-stu-id="e3cf8-151">pendingInstallUserCount</span></span>|<span data-ttu-id="e3cf8-152">Int32</span><span class="sxs-lookup"><span data-stu-id="e3cf8-152">Int32</span></span>|<span data-ttu-id="e3cf8-153">Número de usuários que têm um ou mais dispositivos que foram notificados para instalar este aplicativo e têm 0 dispositivos com falhas.</span><span class="sxs-lookup"><span data-stu-id="e3cf8-153">Number of Users that have 1 or more device that have been notified to install this app and have 0 devices with failures.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e3cf8-154">Relações</span><span class="sxs-lookup"><span data-stu-id="e3cf8-154">Relationships</span></span>
<span data-ttu-id="e3cf8-155">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e3cf8-155">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e3cf8-156">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e3cf8-156">JSON Representation</span></span>
<span data-ttu-id="e3cf8-157">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e3cf8-157">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mobileAppInstallSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppInstallSummary",
  "id": "String (identifier)",
  "installedDeviceCount": 1024,
  "failedDeviceCount": 1024,
  "notApplicableDeviceCount": 1024,
  "notInstalledDeviceCount": 1024,
  "pendingInstallDeviceCount": 1024,
  "installedUserCount": 1024,
  "failedUserCount": 1024,
  "notApplicableUserCount": 1024,
  "notInstalledUserCount": 1024,
  "pendingInstallUserCount": 1024
}
```





