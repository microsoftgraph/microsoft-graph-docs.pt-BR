---
title: tipo de recurso deviceManagementConfigurationWindowsSettingApplicability
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: ca3b520a194a09d178790f5a82f3ca21c1e00d2d
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49301383"
---
# <a name="devicemanagementconfigurationwindowssettingapplicability-resource-type"></a><span data-ttu-id="f177d-103">tipo de recurso deviceManagementConfigurationWindowsSettingApplicability</span><span class="sxs-lookup"><span data-stu-id="f177d-103">deviceManagementConfigurationWindowsSettingApplicability resource type</span></span>

<span data-ttu-id="f177d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f177d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f177d-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f177d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f177d-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f177d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f177d-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="f177d-107">Not yet documented</span></span>


<span data-ttu-id="f177d-108">Herda de [deviceManagementConfigurationSettingApplicability](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingapplicability.md)</span><span class="sxs-lookup"><span data-stu-id="f177d-108">Inherits from [deviceManagementConfigurationSettingApplicability](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingapplicability.md)</span></span>

## <a name="properties"></a><span data-ttu-id="f177d-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f177d-109">Properties</span></span>
|<span data-ttu-id="f177d-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f177d-110">Property</span></span>|<span data-ttu-id="f177d-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="f177d-111">Type</span></span>|<span data-ttu-id="f177d-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="f177d-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f177d-113">description</span><span class="sxs-lookup"><span data-stu-id="f177d-113">description</span></span>|<span data-ttu-id="f177d-114">String</span><span class="sxs-lookup"><span data-stu-id="f177d-114">String</span></span>|<span data-ttu-id="f177d-115">Descrição da configuração herdada de [deviceManagementConfigurationSettingApplicability](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingapplicability.md)</span><span class="sxs-lookup"><span data-stu-id="f177d-115">description of the setting Inherited from [deviceManagementConfigurationSettingApplicability](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingapplicability.md)</span></span>|
|<span data-ttu-id="f177d-116">plataforma</span><span class="sxs-lookup"><span data-stu-id="f177d-116">platform</span></span>|[<span data-ttu-id="f177d-117">deviceManagementConfigurationPlatforms</span><span class="sxs-lookup"><span data-stu-id="f177d-117">deviceManagementConfigurationPlatforms</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationplatforms.md)|<span data-ttu-id="f177d-118">A configuração de plataforma pode ser aplicada no herdado de [deviceManagementConfigurationSettingApplicability](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingapplicability.md).</span><span class="sxs-lookup"><span data-stu-id="f177d-118">Platform setting can be applied on Inherited from [deviceManagementConfigurationSettingApplicability](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingapplicability.md).</span></span> <span data-ttu-id="f177d-119">Os valores possíveis são: `none`, `macOS`, `windows10X`, `windows10`.</span><span class="sxs-lookup"><span data-stu-id="f177d-119">Possible values are: `none`, `macOS`, `windows10X`, `windows10`.</span></span>|
|<span data-ttu-id="f177d-120">devicemode</span><span class="sxs-lookup"><span data-stu-id="f177d-120">deviceMode</span></span>|[<span data-ttu-id="f177d-121">deviceManagementConfigurationDeviceMode</span><span class="sxs-lookup"><span data-stu-id="f177d-121">deviceManagementConfigurationDeviceMode</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationdevicemode.md)|<span data-ttu-id="f177d-122">O modo de dispositivo que a configuração pode ser aplicada no herdado de [deviceManagementConfigurationSettingApplicability](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingapplicability.md).</span><span class="sxs-lookup"><span data-stu-id="f177d-122">Device Mode that setting can be applied on Inherited from [deviceManagementConfigurationSettingApplicability](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingapplicability.md).</span></span> <span data-ttu-id="f177d-123">Os valores possíveis são: `none` e `kiosk`.</span><span class="sxs-lookup"><span data-stu-id="f177d-123">Possible values are: `none`, `kiosk`.</span></span>|
|<span data-ttu-id="f177d-124">tecnologias</span><span class="sxs-lookup"><span data-stu-id="f177d-124">technologies</span></span>|[<span data-ttu-id="f177d-125">deviceManagementConfigurationTechnologies</span><span class="sxs-lookup"><span data-stu-id="f177d-125">deviceManagementConfigurationTechnologies</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationtechnologies.md)|<span data-ttu-id="f177d-126">Quais canais de tecnologia essa configuração pode ser implantada por herança de [deviceManagementConfigurationSettingApplicability](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingapplicability.md).</span><span class="sxs-lookup"><span data-stu-id="f177d-126">Which technology channels this setting can be deployed through Inherited from [deviceManagementConfigurationSettingApplicability](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingapplicability.md).</span></span> <span data-ttu-id="f177d-127">Os valores possíveis são: `none`, `mdm`, `windows10XManagement`, `configManager`.</span><span class="sxs-lookup"><span data-stu-id="f177d-127">Possible values are: `none`, `mdm`, `windows10XManagement`, `configManager`.</span></span>|
|<span data-ttu-id="f177d-128">configurationServiceProviderVersion</span><span class="sxs-lookup"><span data-stu-id="f177d-128">configurationServiceProviderVersion</span></span>|<span data-ttu-id="f177d-129">String</span><span class="sxs-lookup"><span data-stu-id="f177d-129">String</span></span>|<span data-ttu-id="f177d-130">Versão da configuração de CSP é parte de</span><span class="sxs-lookup"><span data-stu-id="f177d-130">Version of CSP setting is a part of</span></span>|
|<span data-ttu-id="f177d-131">maximumSupportedVersion</span><span class="sxs-lookup"><span data-stu-id="f177d-131">maximumSupportedVersion</span></span>|<span data-ttu-id="f177d-132">String</span><span class="sxs-lookup"><span data-stu-id="f177d-132">String</span></span>|<span data-ttu-id="f177d-133">Versão máxima com suporte do Windows</span><span class="sxs-lookup"><span data-stu-id="f177d-133">Maximum supported version of Windows</span></span>|
|<span data-ttu-id="f177d-134">minimumSupportedVersion</span><span class="sxs-lookup"><span data-stu-id="f177d-134">minimumSupportedVersion</span></span>|<span data-ttu-id="f177d-135">String</span><span class="sxs-lookup"><span data-stu-id="f177d-135">String</span></span>|<span data-ttu-id="f177d-136">Versão mínima com suporte do Windows</span><span class="sxs-lookup"><span data-stu-id="f177d-136">Minimum supported version of Windows</span></span>|
|<span data-ttu-id="f177d-137">windowsSkus</span><span class="sxs-lookup"><span data-stu-id="f177d-137">windowsSkus</span></span>|<span data-ttu-id="f177d-138">coleção [deviceManagementConfigurationWindowsSkus](../resources/intune-deviceconfigv2-devicemanagementconfigurationwindowsskus.md)</span><span class="sxs-lookup"><span data-stu-id="f177d-138">[deviceManagementConfigurationWindowsSkus](../resources/intune-deviceconfigv2-devicemanagementconfigurationwindowsskus.md) collection</span></span>|<span data-ttu-id="f177d-139">Lista de SKUs do Windows às quais a configuração se aplica</span><span class="sxs-lookup"><span data-stu-id="f177d-139">List of Windows SKUs that the setting is applicable for</span></span>|
|<span data-ttu-id="f177d-140">requiresAzureAd</span><span class="sxs-lookup"><span data-stu-id="f177d-140">requiresAzureAd</span></span>|<span data-ttu-id="f177d-141">Booliano</span><span class="sxs-lookup"><span data-stu-id="f177d-141">Boolean</span></span>|<span data-ttu-id="f177d-142">Requisito de configuração AzureAD</span><span class="sxs-lookup"><span data-stu-id="f177d-142">AzureAD setting requirement</span></span>|
|<span data-ttu-id="f177d-143">requiredAzureAdTrustType</span><span class="sxs-lookup"><span data-stu-id="f177d-143">requiredAzureAdTrustType</span></span>|[<span data-ttu-id="f177d-144">deviceManagementConfigurationAzureAdTrustType</span><span class="sxs-lookup"><span data-stu-id="f177d-144">deviceManagementConfigurationAzureAdTrustType</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationazureadtrusttype.md)|<span data-ttu-id="f177d-145">Tipo de confiança AzureAD necessário.</span><span class="sxs-lookup"><span data-stu-id="f177d-145">Required AzureAD trust type.</span></span> <span data-ttu-id="f177d-146">Os valores possíveis são: `none`, `azureAdJoined`, `addWorkAccount`, `mdmOnly`.</span><span class="sxs-lookup"><span data-stu-id="f177d-146">Possible values are: `none`, `azureAdJoined`, `addWorkAccount`, `mdmOnly`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f177d-147">Relações</span><span class="sxs-lookup"><span data-stu-id="f177d-147">Relationships</span></span>
<span data-ttu-id="f177d-148">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f177d-148">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f177d-149">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f177d-149">JSON Representation</span></span>
<span data-ttu-id="f177d-150">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f177d-150">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationWindowsSettingApplicability"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationWindowsSettingApplicability",
  "description": "String",
  "platform": "String",
  "deviceMode": "String",
  "technologies": "String",
  "configurationServiceProviderVersion": "String",
  "maximumSupportedVersion": "String",
  "minimumSupportedVersion": "String",
  "windowsSkus": [
    "String"
  ],
  "requiresAzureAd": true,
  "requiredAzureAdTrustType": "String"
}
```




