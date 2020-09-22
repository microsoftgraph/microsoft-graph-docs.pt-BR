---
title: tipo de recurso mobileAppInstallSummary
description: Contém propriedades para o resumo de instalação de um aplicativo móvel.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: ff53cb0d244a28924b00f2bb5b287e51db49ef24
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47973887"
---
# <a name="mobileappinstallsummary-resource-type"></a><span data-ttu-id="80eda-103">tipo de recurso mobileAppInstallSummary</span><span class="sxs-lookup"><span data-stu-id="80eda-103">mobileAppInstallSummary resource type</span></span>

<span data-ttu-id="80eda-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="80eda-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="80eda-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="80eda-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="80eda-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="80eda-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="80eda-107">Contém propriedades para o resumo de instalação de um aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="80eda-107">Contains properties for the installation summary of a mobile app.</span></span>

## <a name="methods"></a><span data-ttu-id="80eda-108">Methods</span><span class="sxs-lookup"><span data-stu-id="80eda-108">Methods</span></span>
|<span data-ttu-id="80eda-109">Método</span><span class="sxs-lookup"><span data-stu-id="80eda-109">Method</span></span>|<span data-ttu-id="80eda-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="80eda-110">Return Type</span></span>|<span data-ttu-id="80eda-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="80eda-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="80eda-112">Obter mobileAppInstallSummary</span><span class="sxs-lookup"><span data-stu-id="80eda-112">Get mobileAppInstallSummary</span></span>](../api/intune-apps-mobileappinstallsummary-get.md)|[<span data-ttu-id="80eda-113">mobileAppInstallSummary</span><span class="sxs-lookup"><span data-stu-id="80eda-113">mobileAppInstallSummary</span></span>](../resources/intune-apps-mobileappinstallsummary.md)|<span data-ttu-id="80eda-114">Leia as propriedades e as relações do objeto [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md) .</span><span class="sxs-lookup"><span data-stu-id="80eda-114">Read properties and relationships of the [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md) object.</span></span>|
|[<span data-ttu-id="80eda-115">Atualizar mobileAppInstallSummary</span><span class="sxs-lookup"><span data-stu-id="80eda-115">Update mobileAppInstallSummary</span></span>](../api/intune-apps-mobileappinstallsummary-update.md)|[<span data-ttu-id="80eda-116">mobileAppInstallSummary</span><span class="sxs-lookup"><span data-stu-id="80eda-116">mobileAppInstallSummary</span></span>](../resources/intune-apps-mobileappinstallsummary.md)|<span data-ttu-id="80eda-117">Atualiza as propriedades de um objeto [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md) .</span><span class="sxs-lookup"><span data-stu-id="80eda-117">Update the properties of a [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="80eda-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="80eda-118">Properties</span></span>
|<span data-ttu-id="80eda-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="80eda-119">Property</span></span>|<span data-ttu-id="80eda-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="80eda-120">Type</span></span>|<span data-ttu-id="80eda-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="80eda-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="80eda-122">id</span><span class="sxs-lookup"><span data-stu-id="80eda-122">id</span></span>|<span data-ttu-id="80eda-123">String</span><span class="sxs-lookup"><span data-stu-id="80eda-123">String</span></span>|<span data-ttu-id="80eda-124">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="80eda-124">Key of the entity.</span></span>|
|<span data-ttu-id="80eda-125">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="80eda-125">installedDeviceCount</span></span>|<span data-ttu-id="80eda-126">Int32</span><span class="sxs-lookup"><span data-stu-id="80eda-126">Int32</span></span>|<span data-ttu-id="80eda-127">Número de dispositivos que instalaram com êxito este aplicativo.</span><span class="sxs-lookup"><span data-stu-id="80eda-127">Number of Devices that have successfully installed this app.</span></span>|
|<span data-ttu-id="80eda-128">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="80eda-128">failedDeviceCount</span></span>|<span data-ttu-id="80eda-129">Int32</span><span class="sxs-lookup"><span data-stu-id="80eda-129">Int32</span></span>|<span data-ttu-id="80eda-130">Número de dispositivos que falharam ao instalar este aplicativo.</span><span class="sxs-lookup"><span data-stu-id="80eda-130">Number of Devices that have failed to install this app.</span></span>|
|<span data-ttu-id="80eda-131">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="80eda-131">notApplicableDeviceCount</span></span>|<span data-ttu-id="80eda-132">Int32</span><span class="sxs-lookup"><span data-stu-id="80eda-132">Int32</span></span>|<span data-ttu-id="80eda-133">Número de dispositivos que não se aplicam a este aplicativo.</span><span class="sxs-lookup"><span data-stu-id="80eda-133">Number of Devices that are not applicable for this app.</span></span>|
|<span data-ttu-id="80eda-134">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="80eda-134">notInstalledDeviceCount</span></span>|<span data-ttu-id="80eda-135">Int32</span><span class="sxs-lookup"><span data-stu-id="80eda-135">Int32</span></span>|<span data-ttu-id="80eda-136">Número de dispositivos que não possuem este aplicativo instalado.</span><span class="sxs-lookup"><span data-stu-id="80eda-136">Number of Devices that does not have this app installed.</span></span>|
|<span data-ttu-id="80eda-137">pendingInstallDeviceCount</span><span class="sxs-lookup"><span data-stu-id="80eda-137">pendingInstallDeviceCount</span></span>|<span data-ttu-id="80eda-138">Int32</span><span class="sxs-lookup"><span data-stu-id="80eda-138">Int32</span></span>|<span data-ttu-id="80eda-139">Número de dispositivos que foram notificados para instalar este aplicativo.</span><span class="sxs-lookup"><span data-stu-id="80eda-139">Number of Devices that have been notified to install this app.</span></span>|
|<span data-ttu-id="80eda-140">installedUserCount</span><span class="sxs-lookup"><span data-stu-id="80eda-140">installedUserCount</span></span>|<span data-ttu-id="80eda-141">Int32</span><span class="sxs-lookup"><span data-stu-id="80eda-141">Int32</span></span>|<span data-ttu-id="80eda-142">Número de usuários cujos dispositivos foram todos bem-sucedidos para instalar este aplicativo.</span><span class="sxs-lookup"><span data-stu-id="80eda-142">Number of Users whose devices have all succeeded to install this app.</span></span>|
|<span data-ttu-id="80eda-143">failedUserCount</span><span class="sxs-lookup"><span data-stu-id="80eda-143">failedUserCount</span></span>|<span data-ttu-id="80eda-144">Int32</span><span class="sxs-lookup"><span data-stu-id="80eda-144">Int32</span></span>|<span data-ttu-id="80eda-145">Número de usuários que têm um ou mais dispositivos que não instalaram este aplicativo.</span><span class="sxs-lookup"><span data-stu-id="80eda-145">Number of Users that have 1 or more device that failed to install this app.</span></span>|
|<span data-ttu-id="80eda-146">notApplicableUserCount</span><span class="sxs-lookup"><span data-stu-id="80eda-146">notApplicableUserCount</span></span>|<span data-ttu-id="80eda-147">Int32</span><span class="sxs-lookup"><span data-stu-id="80eda-147">Int32</span></span>|<span data-ttu-id="80eda-148">Número de usuários cujos dispositivos não são todos aplicáveis para este aplicativo.</span><span class="sxs-lookup"><span data-stu-id="80eda-148">Number of Users whose devices were all not applicable for this app.</span></span>|
|<span data-ttu-id="80eda-149">notInstalledUserCount</span><span class="sxs-lookup"><span data-stu-id="80eda-149">notInstalledUserCount</span></span>|<span data-ttu-id="80eda-150">Int32</span><span class="sxs-lookup"><span data-stu-id="80eda-150">Int32</span></span>|<span data-ttu-id="80eda-151">Número de usuários que têm um ou mais dispositivos que não instalaram este aplicativo.</span><span class="sxs-lookup"><span data-stu-id="80eda-151">Number of Users that have 1 or more devices that did not install this app.</span></span>|
|<span data-ttu-id="80eda-152">pendingInstallUserCount</span><span class="sxs-lookup"><span data-stu-id="80eda-152">pendingInstallUserCount</span></span>|<span data-ttu-id="80eda-153">Int32</span><span class="sxs-lookup"><span data-stu-id="80eda-153">Int32</span></span>|<span data-ttu-id="80eda-154">Número de usuários que têm um ou mais dispositivos que foram notificados para instalar este aplicativo e têm 0 dispositivos com falhas.</span><span class="sxs-lookup"><span data-stu-id="80eda-154">Number of Users that have 1 or more device that have been notified to install this app and have 0 devices with failures.</span></span>|

## <a name="relationships"></a><span data-ttu-id="80eda-155">Relações</span><span class="sxs-lookup"><span data-stu-id="80eda-155">Relationships</span></span>
<span data-ttu-id="80eda-156">Nenhum</span><span class="sxs-lookup"><span data-stu-id="80eda-156">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="80eda-157">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="80eda-157">JSON Representation</span></span>
<span data-ttu-id="80eda-158">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="80eda-158">Here is a JSON representation of the resource.</span></span>
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






