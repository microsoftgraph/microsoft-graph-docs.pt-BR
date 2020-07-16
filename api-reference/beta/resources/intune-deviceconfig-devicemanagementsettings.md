---
title: Tipo de recurso deviceManagementSettings
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 7dd44406211e8d0763625e5c1ae252444505265e
ms.sourcegitcommit: f3dda172d95ef1eda8f6dd9e3ffdc7d3c0744c0a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/14/2020
ms.locfileid: "45123950"
---
# <a name="devicemanagementsettings-resource-type"></a><span data-ttu-id="a4380-103">Tipo de recurso deviceManagementSettings</span><span class="sxs-lookup"><span data-stu-id="a4380-103">deviceManagementSettings resource type</span></span>

<span data-ttu-id="a4380-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a4380-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a4380-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a4380-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a4380-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a4380-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a4380-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="a4380-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="a4380-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a4380-108">Properties</span></span>
|<span data-ttu-id="a4380-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a4380-109">Property</span></span>|<span data-ttu-id="a4380-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="a4380-110">Type</span></span>|<span data-ttu-id="a4380-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="a4380-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a4380-112">deviceComplianceCheckinThresholdDays</span><span class="sxs-lookup"><span data-stu-id="a4380-112">deviceComplianceCheckinThresholdDays</span></span>|<span data-ttu-id="a4380-113">Int32</span><span class="sxs-lookup"><span data-stu-id="a4380-113">Int32</span></span>|<span data-ttu-id="a4380-114">O número de dias que tem um dispositivo pode ser executado sem fazer check-in para permanecer em conformidade.</span><span class="sxs-lookup"><span data-stu-id="a4380-114">The number of days a device is allowed to go without checking in to remain compliant.</span></span>|
|<span data-ttu-id="a4380-115">isScheduledActionEnabled</span><span class="sxs-lookup"><span data-stu-id="a4380-115">isScheduledActionEnabled</span></span>|<span data-ttu-id="a4380-116">Booliano</span><span class="sxs-lookup"><span data-stu-id="a4380-116">Boolean</span></span>|<span data-ttu-id="a4380-117">O recurso está habilitado ou não para ação agendada para a regra.</span><span class="sxs-lookup"><span data-stu-id="a4380-117">Is feature enabled or not for scheduled action for rule.</span></span>|
|<span data-ttu-id="a4380-118">secureByDefault</span><span class="sxs-lookup"><span data-stu-id="a4380-118">secureByDefault</span></span>|<span data-ttu-id="a4380-119">Booliano</span><span class="sxs-lookup"><span data-stu-id="a4380-119">Boolean</span></span>|<span data-ttu-id="a4380-120">Quando true, o dispositivo deve ser incompatível quando não há nenhuma política de conformidade direcionada</span><span class="sxs-lookup"><span data-stu-id="a4380-120">Device should be noncompliant when there is no compliance policy targeted when this is true</span></span>|
|<span data-ttu-id="a4380-121">enhancedJailBreak</span><span class="sxs-lookup"><span data-stu-id="a4380-121">enhancedJailBreak</span></span>|<span data-ttu-id="a4380-122">Booliano</span><span class="sxs-lookup"><span data-stu-id="a4380-122">Boolean</span></span>|<span data-ttu-id="a4380-123">O recurso está habilitado ou não para a detecção de jailbreak avançada.</span><span class="sxs-lookup"><span data-stu-id="a4380-123">Is feature enabled or not for enhanced jailbreak detection.</span></span>|
|<span data-ttu-id="a4380-124">deviceInactivityBeforeRetirementInDay</span><span class="sxs-lookup"><span data-stu-id="a4380-124">deviceInactivityBeforeRetirementInDay</span></span>|<span data-ttu-id="a4380-125">Int32</span><span class="sxs-lookup"><span data-stu-id="a4380-125">Int32</span></span>|<span data-ttu-id="a4380-126">Quando o dispositivo não faz check-in por um número especificado de dias, os dados da empresa podem ser removidos e o dispositivo não estará sob gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="a4380-126">When the device does not check in for specified number of days, the company data might be removed and the device will not be under management.</span></span> <span data-ttu-id="a4380-127">Valores válidos de 30 a 270</span><span class="sxs-lookup"><span data-stu-id="a4380-127">Valid values 30 to 270</span></span>|
|<span data-ttu-id="a4380-128">derivedCredentialProvider</span><span class="sxs-lookup"><span data-stu-id="a4380-128">derivedCredentialProvider</span></span>|[<span data-ttu-id="a4380-129">derivedCredentialProviderType</span><span class="sxs-lookup"><span data-stu-id="a4380-129">derivedCredentialProviderType</span></span>](../resources/intune-deviceconfig-derivedcredentialprovidertype.md)|<span data-ttu-id="a4380-130">O provedor de credenciais derivado a ser usado para esta conta.</span><span class="sxs-lookup"><span data-stu-id="a4380-130">The Derived Credential Provider to use for this account.</span></span> <span data-ttu-id="a4380-131">Os valores possíveis são: `notConfigured`, `entrustDataCard`, `purebred`, `xTec`, `intercede`.</span><span class="sxs-lookup"><span data-stu-id="a4380-131">Possible values are: `notConfigured`, `entrustDataCard`, `purebred`, `xTec`, `intercede`.</span></span>|
|<span data-ttu-id="a4380-132">derivedCredentialUrl</span><span class="sxs-lookup"><span data-stu-id="a4380-132">derivedCredentialUrl</span></span>|<span data-ttu-id="a4380-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a4380-133">String</span></span>|<span data-ttu-id="a4380-134">O URI de autoatendimento do provedor de credenciais derivado.</span><span class="sxs-lookup"><span data-stu-id="a4380-134">The Derived Credential Provider self-service URI.</span></span>|
|<span data-ttu-id="a4380-135">androidDeviceAdministratorEnrollmentEnabled</span><span class="sxs-lookup"><span data-stu-id="a4380-135">androidDeviceAdministratorEnrollmentEnabled</span></span>|<span data-ttu-id="a4380-136">Booliano</span><span class="sxs-lookup"><span data-stu-id="a4380-136">Boolean</span></span>|<span data-ttu-id="a4380-137">A propriedade para determinar se o registro do administrador do dispositivo Android está habilitado para esta conta.</span><span class="sxs-lookup"><span data-stu-id="a4380-137">The property to determine if Android device administrator enrollment is enabled for this account.</span></span>|
|<span data-ttu-id="a4380-138">ignoreDevicesForUnsupportedSettingsEnabled</span><span class="sxs-lookup"><span data-stu-id="a4380-138">ignoreDevicesForUnsupportedSettingsEnabled</span></span>|<span data-ttu-id="a4380-139">Booliano</span><span class="sxs-lookup"><span data-stu-id="a4380-139">Boolean</span></span>|<span data-ttu-id="a4380-140">A propriedade para determinar se deve ignorar as configurações de conformidade não suportadas em determinados modelos de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="a4380-140">The property to determine whether to ignore unsupported compliance settings on certian models of devices.</span></span>|
|<span data-ttu-id="a4380-141">enableLogCollection</span><span class="sxs-lookup"><span data-stu-id="a4380-141">enableLogCollection</span></span>|<span data-ttu-id="a4380-142">Booliano</span><span class="sxs-lookup"><span data-stu-id="a4380-142">Boolean</span></span>|<span data-ttu-id="a4380-143">Determina se o recurso de coleção de logs deve estar disponível para uso.</span><span class="sxs-lookup"><span data-stu-id="a4380-143">Determines whether the log collection feature should be available for use.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a4380-144">Relações</span><span class="sxs-lookup"><span data-stu-id="a4380-144">Relationships</span></span>
<span data-ttu-id="a4380-145">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a4380-145">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a4380-146">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a4380-146">JSON Representation</span></span>
<span data-ttu-id="a4380-147">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a4380-147">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementSettings",
  "deviceComplianceCheckinThresholdDays": 1024,
  "isScheduledActionEnabled": true,
  "secureByDefault": true,
  "enhancedJailBreak": true,
  "deviceInactivityBeforeRetirementInDay": 1024,
  "derivedCredentialProvider": "String",
  "derivedCredentialUrl": "String",
  "androidDeviceAdministratorEnrollmentEnabled": true,
  "ignoreDevicesForUnsupportedSettingsEnabled": true,
  "enableLogCollection": true
}
```



