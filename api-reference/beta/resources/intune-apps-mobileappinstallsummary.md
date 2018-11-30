---
title: tipo de recurso de mobileAppInstallSummary
description: Contém propriedades para o resumo da instalação de um aplicativo móvel.
ms.openlocfilehash: bda3f798a86b38ca0d1224ce509c355a8aec998a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27033620"
---
# <a name="mobileappinstallsummary-resource-type"></a><span data-ttu-id="0ec23-103">tipo de recurso de mobileAppInstallSummary</span><span class="sxs-lookup"><span data-stu-id="0ec23-103">mobileAppInstallSummary resource type</span></span>

> <span data-ttu-id="0ec23-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="0ec23-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0ec23-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="0ec23-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0ec23-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="0ec23-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0ec23-107">Contém propriedades para o resumo da instalação de um aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="0ec23-107">Contains properties for the installation summary of a mobile app.</span></span>
## <a name="methods"></a><span data-ttu-id="0ec23-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="0ec23-108">Methods</span></span>
|<span data-ttu-id="0ec23-109">Método</span><span class="sxs-lookup"><span data-stu-id="0ec23-109">Method</span></span>|<span data-ttu-id="0ec23-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="0ec23-110">Return Type</span></span>|<span data-ttu-id="0ec23-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="0ec23-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="0ec23-112">Obter mobileAppInstallSummary</span><span class="sxs-lookup"><span data-stu-id="0ec23-112">Get mobileAppInstallSummary</span></span>](../api/intune-apps-mobileappinstallsummary-get.md)|[<span data-ttu-id="0ec23-113">mobileAppInstallSummary</span><span class="sxs-lookup"><span data-stu-id="0ec23-113">mobileAppInstallSummary</span></span>](../resources/intune-apps-mobileappinstallsummary.md)|<span data-ttu-id="0ec23-114">Leia as propriedades e os relacionamentos do objeto [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md) .</span><span class="sxs-lookup"><span data-stu-id="0ec23-114">Read properties and relationships of the [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md) object.</span></span>|
|[<span data-ttu-id="0ec23-115">Atualizar mobileAppInstallSummary</span><span class="sxs-lookup"><span data-stu-id="0ec23-115">Update mobileAppInstallSummary</span></span>](../api/intune-apps-mobileappinstallsummary-update.md)|[<span data-ttu-id="0ec23-116">mobileAppInstallSummary</span><span class="sxs-lookup"><span data-stu-id="0ec23-116">mobileAppInstallSummary</span></span>](../resources/intune-apps-mobileappinstallsummary.md)|<span data-ttu-id="0ec23-117">Atualize as propriedades de um objeto [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md) .</span><span class="sxs-lookup"><span data-stu-id="0ec23-117">Update the properties of a [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="0ec23-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0ec23-118">Properties</span></span>
|<span data-ttu-id="0ec23-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0ec23-119">Property</span></span>|<span data-ttu-id="0ec23-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="0ec23-120">Type</span></span>|<span data-ttu-id="0ec23-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="0ec23-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0ec23-122">id</span><span class="sxs-lookup"><span data-stu-id="0ec23-122">id</span></span>|<span data-ttu-id="0ec23-123">String</span><span class="sxs-lookup"><span data-stu-id="0ec23-123">String</span></span>|<span data-ttu-id="0ec23-124">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="0ec23-124">Key of the entity.</span></span>|
|<span data-ttu-id="0ec23-125">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="0ec23-125">installedDeviceCount</span></span>|<span data-ttu-id="0ec23-126">Int32</span><span class="sxs-lookup"><span data-stu-id="0ec23-126">Int32</span></span>|<span data-ttu-id="0ec23-127">Número de dispositivos que instalou com sucesso deste aplicativo.</span><span class="sxs-lookup"><span data-stu-id="0ec23-127">Number of Devices that have successfully installed this app.</span></span>|
|<span data-ttu-id="0ec23-128">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="0ec23-128">failedDeviceCount</span></span>|<span data-ttu-id="0ec23-129">Int32</span><span class="sxs-lookup"><span data-stu-id="0ec23-129">Int32</span></span>|<span data-ttu-id="0ec23-130">Número de dispositivos que não tenha conseguido instalar esse aplicativo.</span><span class="sxs-lookup"><span data-stu-id="0ec23-130">Number of Devices that have failed to install this app.</span></span>|
|<span data-ttu-id="0ec23-131">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="0ec23-131">notApplicableDeviceCount</span></span>|<span data-ttu-id="0ec23-132">Int32</span><span class="sxs-lookup"><span data-stu-id="0ec23-132">Int32</span></span>|<span data-ttu-id="0ec23-133">Número de dispositivos que não são aplicáveis para esse aplicativo.</span><span class="sxs-lookup"><span data-stu-id="0ec23-133">Number of Devices that are not applicable for this app.</span></span>|
|<span data-ttu-id="0ec23-134">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="0ec23-134">notInstalledDeviceCount</span></span>|<span data-ttu-id="0ec23-135">Int32</span><span class="sxs-lookup"><span data-stu-id="0ec23-135">Int32</span></span>|<span data-ttu-id="0ec23-136">Número de dispositivos que não tem este aplicativo instalado.</span><span class="sxs-lookup"><span data-stu-id="0ec23-136">Number of Devices that does not have this app installed.</span></span>|
|<span data-ttu-id="0ec23-137">pendingInstallDeviceCount</span><span class="sxs-lookup"><span data-stu-id="0ec23-137">pendingInstallDeviceCount</span></span>|<span data-ttu-id="0ec23-138">Int32</span><span class="sxs-lookup"><span data-stu-id="0ec23-138">Int32</span></span>|<span data-ttu-id="0ec23-139">Número de dispositivos que foram notificados para instalar esse aplicativo.</span><span class="sxs-lookup"><span data-stu-id="0ec23-139">Number of Devices that have been notified to install this app.</span></span>|
|<span data-ttu-id="0ec23-140">installedUserCount</span><span class="sxs-lookup"><span data-stu-id="0ec23-140">installedUserCount</span></span>|<span data-ttu-id="0ec23-141">Int32</span><span class="sxs-lookup"><span data-stu-id="0ec23-141">Int32</span></span>|<span data-ttu-id="0ec23-142">Número de usuários cujos dispositivos tiveram êxito para instalar esse aplicativo.</span><span class="sxs-lookup"><span data-stu-id="0ec23-142">Number of Users whose devices have all succeeded to install this app.</span></span>|
|<span data-ttu-id="0ec23-143">failedUserCount</span><span class="sxs-lookup"><span data-stu-id="0ec23-143">failedUserCount</span></span>|<span data-ttu-id="0ec23-144">Int32</span><span class="sxs-lookup"><span data-stu-id="0ec23-144">Int32</span></span>|<span data-ttu-id="0ec23-145">Número de usuários que têm 1 ou mais dispositivo com falha para instalar esse aplicativo.</span><span class="sxs-lookup"><span data-stu-id="0ec23-145">Number of Users that have 1 or more device that failed to install this app.</span></span>|
|<span data-ttu-id="0ec23-146">notApplicableUserCount</span><span class="sxs-lookup"><span data-stu-id="0ec23-146">notApplicableUserCount</span></span>|<span data-ttu-id="0ec23-147">Int32</span><span class="sxs-lookup"><span data-stu-id="0ec23-147">Int32</span></span>|<span data-ttu-id="0ec23-148">Número de usuários cujos dispositivos tudo não eram aplicáveis para esse aplicativo.</span><span class="sxs-lookup"><span data-stu-id="0ec23-148">Number of Users whose devices were all not applicable for this app.</span></span>|
|<span data-ttu-id="0ec23-149">notInstalledUserCount</span><span class="sxs-lookup"><span data-stu-id="0ec23-149">notInstalledUserCount</span></span>|<span data-ttu-id="0ec23-150">Int32</span><span class="sxs-lookup"><span data-stu-id="0ec23-150">Int32</span></span>|<span data-ttu-id="0ec23-151">Número de usuários que têm 1 ou mais dispositivos que não tiver instalado esse aplicativo.</span><span class="sxs-lookup"><span data-stu-id="0ec23-151">Number of Users that have 1 or more devices that did not install this app.</span></span>|
|<span data-ttu-id="0ec23-152">pendingInstallUserCount</span><span class="sxs-lookup"><span data-stu-id="0ec23-152">pendingInstallUserCount</span></span>|<span data-ttu-id="0ec23-153">Int32</span><span class="sxs-lookup"><span data-stu-id="0ec23-153">Int32</span></span>|<span data-ttu-id="0ec23-154">Número de usuários que têm 1 ou mais dispositivo que foram notificados para instalar esse aplicativo e tiver 0 dispositivos com falhas.</span><span class="sxs-lookup"><span data-stu-id="0ec23-154">Number of Users that have 1 or more device that have been notified to install this app and have 0 devices with failures.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0ec23-155">Relações</span><span class="sxs-lookup"><span data-stu-id="0ec23-155">Relationships</span></span>
<span data-ttu-id="0ec23-156">Nenhum</span><span class="sxs-lookup"><span data-stu-id="0ec23-156">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="0ec23-157">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0ec23-157">JSON Representation</span></span>
<span data-ttu-id="0ec23-158">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0ec23-158">Here is a JSON representation of the resource.</span></span>
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





