---
title: tipo de recurso de mobileAppInstallSummary
description: Contém propriedades para o resumo da instalação de um aplicativo móvel.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: a2bd7c30c1b00e83731766bcd80f9a9fafd8e8b7
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29416710"
---
# <a name="mobileappinstallsummary-resource-type"></a><span data-ttu-id="428b0-103">tipo de recurso de mobileAppInstallSummary</span><span class="sxs-lookup"><span data-stu-id="428b0-103">mobileAppInstallSummary resource type</span></span>

> <span data-ttu-id="428b0-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="428b0-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="428b0-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="428b0-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="428b0-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="428b0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="428b0-107">Contém propriedades para o resumo da instalação de um aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="428b0-107">Contains properties for the installation summary of a mobile app.</span></span>

## <a name="methods"></a><span data-ttu-id="428b0-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="428b0-108">Methods</span></span>
|<span data-ttu-id="428b0-109">Método</span><span class="sxs-lookup"><span data-stu-id="428b0-109">Method</span></span>|<span data-ttu-id="428b0-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="428b0-110">Return Type</span></span>|<span data-ttu-id="428b0-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="428b0-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="428b0-112">Obter mobileAppInstallSummary</span><span class="sxs-lookup"><span data-stu-id="428b0-112">Get mobileAppInstallSummary</span></span>](../api/intune-apps-mobileappinstallsummary-get.md)|[<span data-ttu-id="428b0-113">mobileAppInstallSummary</span><span class="sxs-lookup"><span data-stu-id="428b0-113">mobileAppInstallSummary</span></span>](../resources/intune-apps-mobileappinstallsummary.md)|<span data-ttu-id="428b0-114">Leia as propriedades e os relacionamentos do objeto [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md) .</span><span class="sxs-lookup"><span data-stu-id="428b0-114">Read properties and relationships of the [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md) object.</span></span>|
|[<span data-ttu-id="428b0-115">Atualizar mobileAppInstallSummary</span><span class="sxs-lookup"><span data-stu-id="428b0-115">Update mobileAppInstallSummary</span></span>](../api/intune-apps-mobileappinstallsummary-update.md)|[<span data-ttu-id="428b0-116">mobileAppInstallSummary</span><span class="sxs-lookup"><span data-stu-id="428b0-116">mobileAppInstallSummary</span></span>](../resources/intune-apps-mobileappinstallsummary.md)|<span data-ttu-id="428b0-117">Atualize as propriedades de um objeto [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md) .</span><span class="sxs-lookup"><span data-stu-id="428b0-117">Update the properties of a [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="428b0-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="428b0-118">Properties</span></span>
|<span data-ttu-id="428b0-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="428b0-119">Property</span></span>|<span data-ttu-id="428b0-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="428b0-120">Type</span></span>|<span data-ttu-id="428b0-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="428b0-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="428b0-122">id</span><span class="sxs-lookup"><span data-stu-id="428b0-122">id</span></span>|<span data-ttu-id="428b0-123">String</span><span class="sxs-lookup"><span data-stu-id="428b0-123">String</span></span>|<span data-ttu-id="428b0-124">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="428b0-124">Key of the entity.</span></span>|
|<span data-ttu-id="428b0-125">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="428b0-125">installedDeviceCount</span></span>|<span data-ttu-id="428b0-126">Int32</span><span class="sxs-lookup"><span data-stu-id="428b0-126">Int32</span></span>|<span data-ttu-id="428b0-127">Número de dispositivos que instalou com sucesso deste aplicativo.</span><span class="sxs-lookup"><span data-stu-id="428b0-127">Number of Devices that have successfully installed this app.</span></span>|
|<span data-ttu-id="428b0-128">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="428b0-128">failedDeviceCount</span></span>|<span data-ttu-id="428b0-129">Int32</span><span class="sxs-lookup"><span data-stu-id="428b0-129">Int32</span></span>|<span data-ttu-id="428b0-130">Número de dispositivos que não tenha conseguido instalar esse aplicativo.</span><span class="sxs-lookup"><span data-stu-id="428b0-130">Number of Devices that have failed to install this app.</span></span>|
|<span data-ttu-id="428b0-131">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="428b0-131">notApplicableDeviceCount</span></span>|<span data-ttu-id="428b0-132">Int32</span><span class="sxs-lookup"><span data-stu-id="428b0-132">Int32</span></span>|<span data-ttu-id="428b0-133">Número de dispositivos que não são aplicáveis para esse aplicativo.</span><span class="sxs-lookup"><span data-stu-id="428b0-133">Number of Devices that are not applicable for this app.</span></span>|
|<span data-ttu-id="428b0-134">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="428b0-134">notInstalledDeviceCount</span></span>|<span data-ttu-id="428b0-135">Int32</span><span class="sxs-lookup"><span data-stu-id="428b0-135">Int32</span></span>|<span data-ttu-id="428b0-136">Número de dispositivos que não tem este aplicativo instalado.</span><span class="sxs-lookup"><span data-stu-id="428b0-136">Number of Devices that does not have this app installed.</span></span>|
|<span data-ttu-id="428b0-137">pendingInstallDeviceCount</span><span class="sxs-lookup"><span data-stu-id="428b0-137">pendingInstallDeviceCount</span></span>|<span data-ttu-id="428b0-138">Int32</span><span class="sxs-lookup"><span data-stu-id="428b0-138">Int32</span></span>|<span data-ttu-id="428b0-139">Número de dispositivos que foram notificados para instalar esse aplicativo.</span><span class="sxs-lookup"><span data-stu-id="428b0-139">Number of Devices that have been notified to install this app.</span></span>|
|<span data-ttu-id="428b0-140">installedUserCount</span><span class="sxs-lookup"><span data-stu-id="428b0-140">installedUserCount</span></span>|<span data-ttu-id="428b0-141">Int32</span><span class="sxs-lookup"><span data-stu-id="428b0-141">Int32</span></span>|<span data-ttu-id="428b0-142">Número de usuários cujos dispositivos tiveram êxito para instalar esse aplicativo.</span><span class="sxs-lookup"><span data-stu-id="428b0-142">Number of Users whose devices have all succeeded to install this app.</span></span>|
|<span data-ttu-id="428b0-143">failedUserCount</span><span class="sxs-lookup"><span data-stu-id="428b0-143">failedUserCount</span></span>|<span data-ttu-id="428b0-144">Int32</span><span class="sxs-lookup"><span data-stu-id="428b0-144">Int32</span></span>|<span data-ttu-id="428b0-145">Número de usuários que têm 1 ou mais dispositivo com falha para instalar esse aplicativo.</span><span class="sxs-lookup"><span data-stu-id="428b0-145">Number of Users that have 1 or more device that failed to install this app.</span></span>|
|<span data-ttu-id="428b0-146">notApplicableUserCount</span><span class="sxs-lookup"><span data-stu-id="428b0-146">notApplicableUserCount</span></span>|<span data-ttu-id="428b0-147">Int32</span><span class="sxs-lookup"><span data-stu-id="428b0-147">Int32</span></span>|<span data-ttu-id="428b0-148">Número de usuários cujos dispositivos tudo não eram aplicáveis para esse aplicativo.</span><span class="sxs-lookup"><span data-stu-id="428b0-148">Number of Users whose devices were all not applicable for this app.</span></span>|
|<span data-ttu-id="428b0-149">notInstalledUserCount</span><span class="sxs-lookup"><span data-stu-id="428b0-149">notInstalledUserCount</span></span>|<span data-ttu-id="428b0-150">Int32</span><span class="sxs-lookup"><span data-stu-id="428b0-150">Int32</span></span>|<span data-ttu-id="428b0-151">Número de usuários que têm 1 ou mais dispositivos que não tiver instalado esse aplicativo.</span><span class="sxs-lookup"><span data-stu-id="428b0-151">Number of Users that have 1 or more devices that did not install this app.</span></span>|
|<span data-ttu-id="428b0-152">pendingInstallUserCount</span><span class="sxs-lookup"><span data-stu-id="428b0-152">pendingInstallUserCount</span></span>|<span data-ttu-id="428b0-153">Int32</span><span class="sxs-lookup"><span data-stu-id="428b0-153">Int32</span></span>|<span data-ttu-id="428b0-154">Número de usuários que têm 1 ou mais dispositivo que foram notificados para instalar esse aplicativo e tiver 0 dispositivos com falhas.</span><span class="sxs-lookup"><span data-stu-id="428b0-154">Number of Users that have 1 or more device that have been notified to install this app and have 0 devices with failures.</span></span>|

## <a name="relationships"></a><span data-ttu-id="428b0-155">Relações</span><span class="sxs-lookup"><span data-stu-id="428b0-155">Relationships</span></span>
<span data-ttu-id="428b0-156">Nenhum</span><span class="sxs-lookup"><span data-stu-id="428b0-156">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="428b0-157">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="428b0-157">JSON Representation</span></span>
<span data-ttu-id="428b0-158">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="428b0-158">Here is a JSON representation of the resource.</span></span>
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




