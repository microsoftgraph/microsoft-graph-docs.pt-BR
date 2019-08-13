---
title: Tipo de recurso deviceManagementSettings
description: Ainda não documentado
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 726fe757e8db9b1d965c617476006d4866b040ec
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36332761"
---
# <a name="devicemanagementsettings-resource-type"></a><span data-ttu-id="9f0f4-103">Tipo de recurso deviceManagementSettings</span><span class="sxs-lookup"><span data-stu-id="9f0f4-103">deviceManagementSettings resource type</span></span>

> <span data-ttu-id="9f0f4-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="9f0f4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9f0f4-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="9f0f4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9f0f4-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="9f0f4-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="9f0f4-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9f0f4-107">Properties</span></span>
|<span data-ttu-id="9f0f4-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9f0f4-108">Property</span></span>|<span data-ttu-id="9f0f4-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="9f0f4-109">Type</span></span>|<span data-ttu-id="9f0f4-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="9f0f4-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9f0f4-111">deviceComplianceCheckinThresholdDays</span><span class="sxs-lookup"><span data-stu-id="9f0f4-111">deviceComplianceCheckinThresholdDays</span></span>|<span data-ttu-id="9f0f4-112">Int32</span><span class="sxs-lookup"><span data-stu-id="9f0f4-112">Int32</span></span>|<span data-ttu-id="9f0f4-113">O número de dias que tem um dispositivo pode ser executado sem fazer check-in para permanecer em conformidade.</span><span class="sxs-lookup"><span data-stu-id="9f0f4-113">The number of days a device is allowed to go without checking in to remain compliant.</span></span> <span data-ttu-id="9f0f4-114">Valores válidos de 0 a 120</span><span class="sxs-lookup"><span data-stu-id="9f0f4-114">Valid values 0 to 120</span></span>|
|<span data-ttu-id="9f0f4-115">isScheduledActionEnabled</span><span class="sxs-lookup"><span data-stu-id="9f0f4-115">isScheduledActionEnabled</span></span>|<span data-ttu-id="9f0f4-116">Booliano</span><span class="sxs-lookup"><span data-stu-id="9f0f4-116">Boolean</span></span>|<span data-ttu-id="9f0f4-117">O recurso está habilitado ou não para ação agendada para a regra.</span><span class="sxs-lookup"><span data-stu-id="9f0f4-117">Is feature enabled or not for scheduled action for rule.</span></span>|
|<span data-ttu-id="9f0f4-118">secureByDefault</span><span class="sxs-lookup"><span data-stu-id="9f0f4-118">secureByDefault</span></span>|<span data-ttu-id="9f0f4-119">Booliano</span><span class="sxs-lookup"><span data-stu-id="9f0f4-119">Boolean</span></span>|<span data-ttu-id="9f0f4-120">Quando true, o dispositivo deve ser incompatível quando não há nenhuma política de conformidade direcionada</span><span class="sxs-lookup"><span data-stu-id="9f0f4-120">Device should be noncompliant when there is no compliance policy targeted when this is true</span></span>|
|<span data-ttu-id="9f0f4-121">enhancedJailBreak</span><span class="sxs-lookup"><span data-stu-id="9f0f4-121">enhancedJailBreak</span></span>|<span data-ttu-id="9f0f4-122">Booliano</span><span class="sxs-lookup"><span data-stu-id="9f0f4-122">Boolean</span></span>|<span data-ttu-id="9f0f4-123">O recurso está habilitado ou não para a detecção de jailbreak avançada.</span><span class="sxs-lookup"><span data-stu-id="9f0f4-123">Is feature enabled or not for enhanced jailbreak detection.</span></span>|
|<span data-ttu-id="9f0f4-124">deviceInactivityBeforeRetirementInDay</span><span class="sxs-lookup"><span data-stu-id="9f0f4-124">deviceInactivityBeforeRetirementInDay</span></span>|<span data-ttu-id="9f0f4-125">Int32</span><span class="sxs-lookup"><span data-stu-id="9f0f4-125">Int32</span></span>|<span data-ttu-id="9f0f4-126">Quando o dispositivo não faz check-in por um número especificado de dias, os dados da empresa podem ser removidos e o dispositivo não estará sob gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="9f0f4-126">When the device does not check in for specified number of days, the company data might be removed and the device will not be under management.</span></span> <span data-ttu-id="9f0f4-127">Valores válidos de 30 a 270</span><span class="sxs-lookup"><span data-stu-id="9f0f4-127">Valid values 30 to 270</span></span>|
|<span data-ttu-id="9f0f4-128">derivedCredentialProvider</span><span class="sxs-lookup"><span data-stu-id="9f0f4-128">derivedCredentialProvider</span></span>|[<span data-ttu-id="9f0f4-129">derivedCredentialProviderType</span><span class="sxs-lookup"><span data-stu-id="9f0f4-129">derivedCredentialProviderType</span></span>](../resources/intune-deviceconfig-derivedcredentialprovidertype.md)|<span data-ttu-id="9f0f4-130">O provedor de credenciais derivado a ser usado para esta conta.</span><span class="sxs-lookup"><span data-stu-id="9f0f4-130">The Derived Credential Provider to use for this account.</span></span> <span data-ttu-id="9f0f4-131">Os valores possíveis são: `notConfigured`, `entrustDataCard`, `purebred`, `xTec`, `intercede`.</span><span class="sxs-lookup"><span data-stu-id="9f0f4-131">Possible values are: `notConfigured`, `entrustDataCard`, `purebred`, `xTec`, `intercede`.</span></span>|
|<span data-ttu-id="9f0f4-132">derivedCredentialUrl</span><span class="sxs-lookup"><span data-stu-id="9f0f4-132">derivedCredentialUrl</span></span>|<span data-ttu-id="9f0f4-133">String</span><span class="sxs-lookup"><span data-stu-id="9f0f4-133">String</span></span>|<span data-ttu-id="9f0f4-134">O URI de autoatendimento do provedor de credenciais derivado.</span><span class="sxs-lookup"><span data-stu-id="9f0f4-134">The Derived Credential Provider self-service URI.</span></span>|
|<span data-ttu-id="9f0f4-135">androidDeviceAdministratorEnrollmentEnabled</span><span class="sxs-lookup"><span data-stu-id="9f0f4-135">androidDeviceAdministratorEnrollmentEnabled</span></span>|<span data-ttu-id="9f0f4-136">Booliano</span><span class="sxs-lookup"><span data-stu-id="9f0f4-136">Boolean</span></span>|<span data-ttu-id="9f0f4-137">A propriedade para determinar se o registro do administrador do dispositivo Android está habilitado para esta conta.</span><span class="sxs-lookup"><span data-stu-id="9f0f4-137">The property to determine if Android device administrator enrollment is enabled for this account.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9f0f4-138">Relações</span><span class="sxs-lookup"><span data-stu-id="9f0f4-138">Relationships</span></span>
<span data-ttu-id="9f0f4-139">Nenhum</span><span class="sxs-lookup"><span data-stu-id="9f0f4-139">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9f0f4-140">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9f0f4-140">JSON Representation</span></span>
<span data-ttu-id="9f0f4-141">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9f0f4-141">Here is a JSON representation of the resource.</span></span>
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
  "androidDeviceAdministratorEnrollmentEnabled": true
}
```



