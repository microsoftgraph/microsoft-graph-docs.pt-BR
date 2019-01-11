---
title: tipo de recurso de mobileAppInstallSummary
description: Contém propriedades para o resumo da instalação de um aplicativo móvel.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 3b730f73b8a86c8acba531ab0d30a67b2f8e7a7f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27820353"
---
# <a name="mobileappinstallsummary-resource-type"></a><span data-ttu-id="1753a-103">tipo de recurso de mobileAppInstallSummary</span><span class="sxs-lookup"><span data-stu-id="1753a-103">mobileAppInstallSummary resource type</span></span>

> <span data-ttu-id="1753a-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="1753a-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1753a-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="1753a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1753a-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="1753a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1753a-107">Contém propriedades para o resumo da instalação de um aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="1753a-107">Contains properties for the installation summary of a mobile app.</span></span>
## <a name="methods"></a><span data-ttu-id="1753a-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="1753a-108">Methods</span></span>
|<span data-ttu-id="1753a-109">Método</span><span class="sxs-lookup"><span data-stu-id="1753a-109">Method</span></span>|<span data-ttu-id="1753a-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="1753a-110">Return Type</span></span>|<span data-ttu-id="1753a-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="1753a-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="1753a-112">Obter mobileAppInstallSummary</span><span class="sxs-lookup"><span data-stu-id="1753a-112">Get mobileAppInstallSummary</span></span>](../api/intune-apps-mobileappinstallsummary-get.md)|[<span data-ttu-id="1753a-113">mobileAppInstallSummary</span><span class="sxs-lookup"><span data-stu-id="1753a-113">mobileAppInstallSummary</span></span>](../resources/intune-apps-mobileappinstallsummary.md)|<span data-ttu-id="1753a-114">Leia as propriedades e os relacionamentos do objeto [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md) .</span><span class="sxs-lookup"><span data-stu-id="1753a-114">Read properties and relationships of the [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md) object.</span></span>|
|[<span data-ttu-id="1753a-115">Atualizar mobileAppInstallSummary</span><span class="sxs-lookup"><span data-stu-id="1753a-115">Update mobileAppInstallSummary</span></span>](../api/intune-apps-mobileappinstallsummary-update.md)|[<span data-ttu-id="1753a-116">mobileAppInstallSummary</span><span class="sxs-lookup"><span data-stu-id="1753a-116">mobileAppInstallSummary</span></span>](../resources/intune-apps-mobileappinstallsummary.md)|<span data-ttu-id="1753a-117">Atualize as propriedades de um objeto [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md) .</span><span class="sxs-lookup"><span data-stu-id="1753a-117">Update the properties of a [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="1753a-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1753a-118">Properties</span></span>
|<span data-ttu-id="1753a-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1753a-119">Property</span></span>|<span data-ttu-id="1753a-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="1753a-120">Type</span></span>|<span data-ttu-id="1753a-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="1753a-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1753a-122">id</span><span class="sxs-lookup"><span data-stu-id="1753a-122">id</span></span>|<span data-ttu-id="1753a-123">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1753a-123">String</span></span>|<span data-ttu-id="1753a-124">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="1753a-124">Key of the entity.</span></span>|
|<span data-ttu-id="1753a-125">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="1753a-125">installedDeviceCount</span></span>|<span data-ttu-id="1753a-126">Int32</span><span class="sxs-lookup"><span data-stu-id="1753a-126">Int32</span></span>|<span data-ttu-id="1753a-127">Número de dispositivos que instalou com sucesso deste aplicativo.</span><span class="sxs-lookup"><span data-stu-id="1753a-127">Number of Devices that have successfully installed this app.</span></span>|
|<span data-ttu-id="1753a-128">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="1753a-128">failedDeviceCount</span></span>|<span data-ttu-id="1753a-129">Int32</span><span class="sxs-lookup"><span data-stu-id="1753a-129">Int32</span></span>|<span data-ttu-id="1753a-130">Número de dispositivos que não tenha conseguido instalar esse aplicativo.</span><span class="sxs-lookup"><span data-stu-id="1753a-130">Number of Devices that have failed to install this app.</span></span>|
|<span data-ttu-id="1753a-131">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="1753a-131">notApplicableDeviceCount</span></span>|<span data-ttu-id="1753a-132">Int32</span><span class="sxs-lookup"><span data-stu-id="1753a-132">Int32</span></span>|<span data-ttu-id="1753a-133">Número de dispositivos que não são aplicáveis para esse aplicativo.</span><span class="sxs-lookup"><span data-stu-id="1753a-133">Number of Devices that are not applicable for this app.</span></span>|
|<span data-ttu-id="1753a-134">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="1753a-134">notInstalledDeviceCount</span></span>|<span data-ttu-id="1753a-135">Int32</span><span class="sxs-lookup"><span data-stu-id="1753a-135">Int32</span></span>|<span data-ttu-id="1753a-136">Número de dispositivos que não tem este aplicativo instalado.</span><span class="sxs-lookup"><span data-stu-id="1753a-136">Number of Devices that does not have this app installed.</span></span>|
|<span data-ttu-id="1753a-137">pendingInstallDeviceCount</span><span class="sxs-lookup"><span data-stu-id="1753a-137">pendingInstallDeviceCount</span></span>|<span data-ttu-id="1753a-138">Int32</span><span class="sxs-lookup"><span data-stu-id="1753a-138">Int32</span></span>|<span data-ttu-id="1753a-139">Número de dispositivos que foram notificados para instalar esse aplicativo.</span><span class="sxs-lookup"><span data-stu-id="1753a-139">Number of Devices that have been notified to install this app.</span></span>|
|<span data-ttu-id="1753a-140">installedUserCount</span><span class="sxs-lookup"><span data-stu-id="1753a-140">installedUserCount</span></span>|<span data-ttu-id="1753a-141">Int32</span><span class="sxs-lookup"><span data-stu-id="1753a-141">Int32</span></span>|<span data-ttu-id="1753a-142">Número de usuários cujos dispositivos tiveram êxito para instalar esse aplicativo.</span><span class="sxs-lookup"><span data-stu-id="1753a-142">Number of Users whose devices have all succeeded to install this app.</span></span>|
|<span data-ttu-id="1753a-143">failedUserCount</span><span class="sxs-lookup"><span data-stu-id="1753a-143">failedUserCount</span></span>|<span data-ttu-id="1753a-144">Int32</span><span class="sxs-lookup"><span data-stu-id="1753a-144">Int32</span></span>|<span data-ttu-id="1753a-145">Número de usuários que têm 1 ou mais dispositivo com falha para instalar esse aplicativo.</span><span class="sxs-lookup"><span data-stu-id="1753a-145">Number of Users that have 1 or more device that failed to install this app.</span></span>|
|<span data-ttu-id="1753a-146">notApplicableUserCount</span><span class="sxs-lookup"><span data-stu-id="1753a-146">notApplicableUserCount</span></span>|<span data-ttu-id="1753a-147">Int32</span><span class="sxs-lookup"><span data-stu-id="1753a-147">Int32</span></span>|<span data-ttu-id="1753a-148">Número de usuários cujos dispositivos tudo não eram aplicáveis para esse aplicativo.</span><span class="sxs-lookup"><span data-stu-id="1753a-148">Number of Users whose devices were all not applicable for this app.</span></span>|
|<span data-ttu-id="1753a-149">notInstalledUserCount</span><span class="sxs-lookup"><span data-stu-id="1753a-149">notInstalledUserCount</span></span>|<span data-ttu-id="1753a-150">Int32</span><span class="sxs-lookup"><span data-stu-id="1753a-150">Int32</span></span>|<span data-ttu-id="1753a-151">Número de usuários que têm 1 ou mais dispositivos que não tiver instalado esse aplicativo.</span><span class="sxs-lookup"><span data-stu-id="1753a-151">Number of Users that have 1 or more devices that did not install this app.</span></span>|
|<span data-ttu-id="1753a-152">pendingInstallUserCount</span><span class="sxs-lookup"><span data-stu-id="1753a-152">pendingInstallUserCount</span></span>|<span data-ttu-id="1753a-153">Int32</span><span class="sxs-lookup"><span data-stu-id="1753a-153">Int32</span></span>|<span data-ttu-id="1753a-154">Número de usuários que têm 1 ou mais dispositivo que foram notificados para instalar esse aplicativo e tiver 0 dispositivos com falhas.</span><span class="sxs-lookup"><span data-stu-id="1753a-154">Number of Users that have 1 or more device that have been notified to install this app and have 0 devices with failures.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1753a-155">Relações</span><span class="sxs-lookup"><span data-stu-id="1753a-155">Relationships</span></span>
<span data-ttu-id="1753a-156">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1753a-156">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="1753a-157">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1753a-157">JSON Representation</span></span>
<span data-ttu-id="1753a-158">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1753a-158">Here is a JSON representation of the resource.</span></span>
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





