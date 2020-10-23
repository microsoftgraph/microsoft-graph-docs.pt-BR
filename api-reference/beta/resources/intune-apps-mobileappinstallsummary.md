---
title: tipo de recurso mobileAppInstallSummary
description: Contém propriedades para o resumo de instalação de um aplicativo móvel.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: dbe40a14569a4a073da333d9df684069d0c457ac
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48721517"
---
# <a name="mobileappinstallsummary-resource-type"></a><span data-ttu-id="ab86b-103">tipo de recurso mobileAppInstallSummary</span><span class="sxs-lookup"><span data-stu-id="ab86b-103">mobileAppInstallSummary resource type</span></span>

<span data-ttu-id="ab86b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ab86b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ab86b-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ab86b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ab86b-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ab86b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ab86b-107">Contém propriedades para o resumo de instalação de um aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="ab86b-107">Contains properties for the installation summary of a mobile app.</span></span>

## <a name="methods"></a><span data-ttu-id="ab86b-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="ab86b-108">Methods</span></span>
|<span data-ttu-id="ab86b-109">Método</span><span class="sxs-lookup"><span data-stu-id="ab86b-109">Method</span></span>|<span data-ttu-id="ab86b-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="ab86b-110">Return Type</span></span>|<span data-ttu-id="ab86b-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="ab86b-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="ab86b-112">Obter mobileAppInstallSummary</span><span class="sxs-lookup"><span data-stu-id="ab86b-112">Get mobileAppInstallSummary</span></span>](../api/intune-apps-mobileappinstallsummary-get.md)|[<span data-ttu-id="ab86b-113">mobileAppInstallSummary</span><span class="sxs-lookup"><span data-stu-id="ab86b-113">mobileAppInstallSummary</span></span>](../resources/intune-apps-mobileappinstallsummary.md)|<span data-ttu-id="ab86b-114">Leia as propriedades e as relações do objeto [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md) .</span><span class="sxs-lookup"><span data-stu-id="ab86b-114">Read properties and relationships of the [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md) object.</span></span>|
|[<span data-ttu-id="ab86b-115">Atualizar mobileAppInstallSummary</span><span class="sxs-lookup"><span data-stu-id="ab86b-115">Update mobileAppInstallSummary</span></span>](../api/intune-apps-mobileappinstallsummary-update.md)|[<span data-ttu-id="ab86b-116">mobileAppInstallSummary</span><span class="sxs-lookup"><span data-stu-id="ab86b-116">mobileAppInstallSummary</span></span>](../resources/intune-apps-mobileappinstallsummary.md)|<span data-ttu-id="ab86b-117">Atualiza as propriedades de um objeto [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md) .</span><span class="sxs-lookup"><span data-stu-id="ab86b-117">Update the properties of a [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="ab86b-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ab86b-118">Properties</span></span>
|<span data-ttu-id="ab86b-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ab86b-119">Property</span></span>|<span data-ttu-id="ab86b-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="ab86b-120">Type</span></span>|<span data-ttu-id="ab86b-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="ab86b-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ab86b-122">id</span><span class="sxs-lookup"><span data-stu-id="ab86b-122">id</span></span>|<span data-ttu-id="ab86b-123">String</span><span class="sxs-lookup"><span data-stu-id="ab86b-123">String</span></span>|<span data-ttu-id="ab86b-124">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="ab86b-124">Key of the entity.</span></span>|
|<span data-ttu-id="ab86b-125">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ab86b-125">installedDeviceCount</span></span>|<span data-ttu-id="ab86b-126">Int32</span><span class="sxs-lookup"><span data-stu-id="ab86b-126">Int32</span></span>|<span data-ttu-id="ab86b-127">Número de dispositivos que instalaram com êxito este aplicativo.</span><span class="sxs-lookup"><span data-stu-id="ab86b-127">Number of Devices that have successfully installed this app.</span></span>|
|<span data-ttu-id="ab86b-128">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ab86b-128">failedDeviceCount</span></span>|<span data-ttu-id="ab86b-129">Int32</span><span class="sxs-lookup"><span data-stu-id="ab86b-129">Int32</span></span>|<span data-ttu-id="ab86b-130">Número de dispositivos que falharam ao instalar este aplicativo.</span><span class="sxs-lookup"><span data-stu-id="ab86b-130">Number of Devices that have failed to install this app.</span></span>|
|<span data-ttu-id="ab86b-131">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ab86b-131">notApplicableDeviceCount</span></span>|<span data-ttu-id="ab86b-132">Int32</span><span class="sxs-lookup"><span data-stu-id="ab86b-132">Int32</span></span>|<span data-ttu-id="ab86b-133">Número de dispositivos que não se aplicam a este aplicativo.</span><span class="sxs-lookup"><span data-stu-id="ab86b-133">Number of Devices that are not applicable for this app.</span></span>|
|<span data-ttu-id="ab86b-134">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ab86b-134">notInstalledDeviceCount</span></span>|<span data-ttu-id="ab86b-135">Int32</span><span class="sxs-lookup"><span data-stu-id="ab86b-135">Int32</span></span>|<span data-ttu-id="ab86b-136">Número de dispositivos que não possuem este aplicativo instalado.</span><span class="sxs-lookup"><span data-stu-id="ab86b-136">Number of Devices that does not have this app installed.</span></span>|
|<span data-ttu-id="ab86b-137">pendingInstallDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ab86b-137">pendingInstallDeviceCount</span></span>|<span data-ttu-id="ab86b-138">Int32</span><span class="sxs-lookup"><span data-stu-id="ab86b-138">Int32</span></span>|<span data-ttu-id="ab86b-139">Número de dispositivos que foram notificados para instalar este aplicativo.</span><span class="sxs-lookup"><span data-stu-id="ab86b-139">Number of Devices that have been notified to install this app.</span></span>|
|<span data-ttu-id="ab86b-140">installedUserCount</span><span class="sxs-lookup"><span data-stu-id="ab86b-140">installedUserCount</span></span>|<span data-ttu-id="ab86b-141">Int32</span><span class="sxs-lookup"><span data-stu-id="ab86b-141">Int32</span></span>|<span data-ttu-id="ab86b-142">Número de usuários cujos dispositivos foram todos bem-sucedidos para instalar este aplicativo.</span><span class="sxs-lookup"><span data-stu-id="ab86b-142">Number of Users whose devices have all succeeded to install this app.</span></span>|
|<span data-ttu-id="ab86b-143">failedUserCount</span><span class="sxs-lookup"><span data-stu-id="ab86b-143">failedUserCount</span></span>|<span data-ttu-id="ab86b-144">Int32</span><span class="sxs-lookup"><span data-stu-id="ab86b-144">Int32</span></span>|<span data-ttu-id="ab86b-145">Número de usuários que têm um ou mais dispositivos que não instalaram este aplicativo.</span><span class="sxs-lookup"><span data-stu-id="ab86b-145">Number of Users that have 1 or more device that failed to install this app.</span></span>|
|<span data-ttu-id="ab86b-146">notApplicableUserCount</span><span class="sxs-lookup"><span data-stu-id="ab86b-146">notApplicableUserCount</span></span>|<span data-ttu-id="ab86b-147">Int32</span><span class="sxs-lookup"><span data-stu-id="ab86b-147">Int32</span></span>|<span data-ttu-id="ab86b-148">Número de usuários cujos dispositivos não são todos aplicáveis para este aplicativo.</span><span class="sxs-lookup"><span data-stu-id="ab86b-148">Number of Users whose devices were all not applicable for this app.</span></span>|
|<span data-ttu-id="ab86b-149">notInstalledUserCount</span><span class="sxs-lookup"><span data-stu-id="ab86b-149">notInstalledUserCount</span></span>|<span data-ttu-id="ab86b-150">Int32</span><span class="sxs-lookup"><span data-stu-id="ab86b-150">Int32</span></span>|<span data-ttu-id="ab86b-151">Número de usuários que têm um ou mais dispositivos que não instalaram este aplicativo.</span><span class="sxs-lookup"><span data-stu-id="ab86b-151">Number of Users that have 1 or more devices that did not install this app.</span></span>|
|<span data-ttu-id="ab86b-152">pendingInstallUserCount</span><span class="sxs-lookup"><span data-stu-id="ab86b-152">pendingInstallUserCount</span></span>|<span data-ttu-id="ab86b-153">Int32</span><span class="sxs-lookup"><span data-stu-id="ab86b-153">Int32</span></span>|<span data-ttu-id="ab86b-154">Número de usuários que têm um ou mais dispositivos que foram notificados para instalar este aplicativo e têm 0 dispositivos com falhas.</span><span class="sxs-lookup"><span data-stu-id="ab86b-154">Number of Users that have 1 or more device that have been notified to install this app and have 0 devices with failures.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ab86b-155">Relações</span><span class="sxs-lookup"><span data-stu-id="ab86b-155">Relationships</span></span>
<span data-ttu-id="ab86b-156">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ab86b-156">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ab86b-157">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ab86b-157">JSON Representation</span></span>
<span data-ttu-id="ab86b-158">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ab86b-158">Here is a JSON representation of the resource.</span></span>
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





