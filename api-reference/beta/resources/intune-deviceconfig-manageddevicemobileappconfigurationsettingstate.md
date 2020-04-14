---
title: tipo de recurso managedDeviceMobileAppConfigurationSettingState
description: Estado da configuração do aplicativo móvel do dispositivo gerenciado para um determinado dispositivo.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 9f5fbdae9a59b19216db0db0f460402ce3ba374a
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43437289"
---
# <a name="manageddevicemobileappconfigurationsettingstate-resource-type"></a><span data-ttu-id="9d34e-103">tipo de recurso managedDeviceMobileAppConfigurationSettingState</span><span class="sxs-lookup"><span data-stu-id="9d34e-103">managedDeviceMobileAppConfigurationSettingState resource type</span></span>

<span data-ttu-id="9d34e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9d34e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9d34e-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="9d34e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9d34e-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="9d34e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9d34e-107">Estado da configuração do aplicativo móvel do dispositivo gerenciado para um determinado dispositivo.</span><span class="sxs-lookup"><span data-stu-id="9d34e-107">Managed Device Mobile App Configuration Setting State for a given device.</span></span>

## <a name="properties"></a><span data-ttu-id="9d34e-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9d34e-108">Properties</span></span>
|<span data-ttu-id="9d34e-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9d34e-109">Property</span></span>|<span data-ttu-id="9d34e-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="9d34e-110">Type</span></span>|<span data-ttu-id="9d34e-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="9d34e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9d34e-112">configuração</span><span class="sxs-lookup"><span data-stu-id="9d34e-112">setting</span></span>|<span data-ttu-id="9d34e-113">String</span><span class="sxs-lookup"><span data-stu-id="9d34e-113">String</span></span>|<span data-ttu-id="9d34e-114">A configuração que é relatada</span><span class="sxs-lookup"><span data-stu-id="9d34e-114">The setting that is being reported</span></span>|
|<span data-ttu-id="9d34e-115">settingName</span><span class="sxs-lookup"><span data-stu-id="9d34e-115">settingName</span></span>|<span data-ttu-id="9d34e-116">String</span><span class="sxs-lookup"><span data-stu-id="9d34e-116">String</span></span>|<span data-ttu-id="9d34e-117">Nome de configuração localizada/de usuário que é relatada</span><span class="sxs-lookup"><span data-stu-id="9d34e-117">Localized/user friendly setting name that is being reported</span></span>|
|<span data-ttu-id="9d34e-118">instanceDisplayName</span><span class="sxs-lookup"><span data-stu-id="9d34e-118">instanceDisplayName</span></span>|<span data-ttu-id="9d34e-119">String</span><span class="sxs-lookup"><span data-stu-id="9d34e-119">String</span></span>|<span data-ttu-id="9d34e-120">Nome da instância de configuração que é relatada.</span><span class="sxs-lookup"><span data-stu-id="9d34e-120">Name of setting instance that is being reported.</span></span>|
|<span data-ttu-id="9d34e-121">state</span><span class="sxs-lookup"><span data-stu-id="9d34e-121">state</span></span>|[<span data-ttu-id="9d34e-122">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="9d34e-122">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="9d34e-123">O estado de conformidade da configuração.</span><span class="sxs-lookup"><span data-stu-id="9d34e-123">The compliance state of the setting.</span></span> <span data-ttu-id="9d34e-124">Os valores possíveis são: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="9d34e-124">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="9d34e-125">errorCode</span><span class="sxs-lookup"><span data-stu-id="9d34e-125">errorCode</span></span>|<span data-ttu-id="9d34e-126">Int64</span><span class="sxs-lookup"><span data-stu-id="9d34e-126">Int64</span></span>|<span data-ttu-id="9d34e-127">Código de erro da configuração</span><span class="sxs-lookup"><span data-stu-id="9d34e-127">Error code for the setting</span></span>|
|<span data-ttu-id="9d34e-128">errorDescription</span><span class="sxs-lookup"><span data-stu-id="9d34e-128">errorDescription</span></span>|<span data-ttu-id="9d34e-129">String</span><span class="sxs-lookup"><span data-stu-id="9d34e-129">String</span></span>|<span data-ttu-id="9d34e-130">Descrição de erro</span><span class="sxs-lookup"><span data-stu-id="9d34e-130">Error description</span></span>|
|<span data-ttu-id="9d34e-131">userId</span><span class="sxs-lookup"><span data-stu-id="9d34e-131">userId</span></span>|<span data-ttu-id="9d34e-132">String</span><span class="sxs-lookup"><span data-stu-id="9d34e-132">String</span></span>|<span data-ttu-id="9d34e-133">UserId</span><span class="sxs-lookup"><span data-stu-id="9d34e-133">UserId</span></span>|
|<span data-ttu-id="9d34e-134">userName</span><span class="sxs-lookup"><span data-stu-id="9d34e-134">userName</span></span>|<span data-ttu-id="9d34e-135">String</span><span class="sxs-lookup"><span data-stu-id="9d34e-135">String</span></span>|<span data-ttu-id="9d34e-136">UserName</span><span class="sxs-lookup"><span data-stu-id="9d34e-136">UserName</span></span>|
|<span data-ttu-id="9d34e-137">userEmail</span><span class="sxs-lookup"><span data-stu-id="9d34e-137">userEmail</span></span>|<span data-ttu-id="9d34e-138">String</span><span class="sxs-lookup"><span data-stu-id="9d34e-138">String</span></span>|<span data-ttu-id="9d34e-139">UserEmail</span><span class="sxs-lookup"><span data-stu-id="9d34e-139">UserEmail</span></span>|
|<span data-ttu-id="9d34e-140">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="9d34e-140">userPrincipalName</span></span>|<span data-ttu-id="9d34e-141">String</span><span class="sxs-lookup"><span data-stu-id="9d34e-141">String</span></span>|<span data-ttu-id="9d34e-142">UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="9d34e-142">UserPrincipalName.</span></span>|
|<span data-ttu-id="9d34e-143">fontes</span><span class="sxs-lookup"><span data-stu-id="9d34e-143">sources</span></span>|<span data-ttu-id="9d34e-144">Conjunto [settingSource](../resources/intune-deviceconfig-settingsource.md)</span><span class="sxs-lookup"><span data-stu-id="9d34e-144">[settingSource](../resources/intune-deviceconfig-settingsource.md) collection</span></span>|<span data-ttu-id="9d34e-145">Políticas de colaboração</span><span class="sxs-lookup"><span data-stu-id="9d34e-145">Contributing policies</span></span>|
|<span data-ttu-id="9d34e-146">currentValue</span><span class="sxs-lookup"><span data-stu-id="9d34e-146">currentValue</span></span>|<span data-ttu-id="9d34e-147">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9d34e-147">String</span></span>|<span data-ttu-id="9d34e-148">Valor atual da configuração em um dispositivo</span><span class="sxs-lookup"><span data-stu-id="9d34e-148">Current value of setting on device</span></span>|
|<span data-ttu-id="9d34e-149">settingInstanceId</span><span class="sxs-lookup"><span data-stu-id="9d34e-149">settingInstanceId</span></span>|<span data-ttu-id="9d34e-150">String</span><span class="sxs-lookup"><span data-stu-id="9d34e-150">String</span></span>|<span data-ttu-id="9d34e-151">SettingInstanceId</span><span class="sxs-lookup"><span data-stu-id="9d34e-151">SettingInstanceId</span></span>|

## <a name="relationships"></a><span data-ttu-id="9d34e-152">Relações</span><span class="sxs-lookup"><span data-stu-id="9d34e-152">Relationships</span></span>
<span data-ttu-id="9d34e-153">Nenhum</span><span class="sxs-lookup"><span data-stu-id="9d34e-153">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9d34e-154">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9d34e-154">JSON Representation</span></span>
<span data-ttu-id="9d34e-155">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9d34e-155">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managedDeviceMobileAppConfigurationSettingState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationSettingState",
  "setting": "String",
  "settingName": "String",
  "instanceDisplayName": "String",
  "state": "String",
  "errorCode": 1024,
  "errorDescription": "String",
  "userId": "String",
  "userName": "String",
  "userEmail": "String",
  "userPrincipalName": "String",
  "sources": [
    {
      "@odata.type": "microsoft.graph.settingSource",
      "id": "String",
      "displayName": "String"
    }
  ],
  "currentValue": "String",
  "settingInstanceId": "String"
}
```



