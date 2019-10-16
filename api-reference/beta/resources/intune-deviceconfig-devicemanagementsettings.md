---
title: Tipo de recurso deviceManagementSettings
description: Ainda não documentado
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: fdc01e2c9cd4aabf47c900bd38bb2b0f7035308b
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/16/2019
ms.locfileid: "37538963"
---
# <a name="devicemanagementsettings-resource-type"></a><span data-ttu-id="b3cd2-103">Tipo de recurso deviceManagementSettings</span><span class="sxs-lookup"><span data-stu-id="b3cd2-103">deviceManagementSettings resource type</span></span>

> <span data-ttu-id="b3cd2-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b3cd2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b3cd2-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b3cd2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b3cd2-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="b3cd2-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="b3cd2-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b3cd2-107">Properties</span></span>
|<span data-ttu-id="b3cd2-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b3cd2-108">Property</span></span>|<span data-ttu-id="b3cd2-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="b3cd2-109">Type</span></span>|<span data-ttu-id="b3cd2-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="b3cd2-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b3cd2-111">deviceComplianceCheckinThresholdDays</span><span class="sxs-lookup"><span data-stu-id="b3cd2-111">deviceComplianceCheckinThresholdDays</span></span>|<span data-ttu-id="b3cd2-112">Int32</span><span class="sxs-lookup"><span data-stu-id="b3cd2-112">Int32</span></span>|<span data-ttu-id="b3cd2-113">O número de dias que tem um dispositivo pode ser executado sem fazer check-in para permanecer em conformidade.</span><span class="sxs-lookup"><span data-stu-id="b3cd2-113">The number of days a device is allowed to go without checking in to remain compliant.</span></span>|
|<span data-ttu-id="b3cd2-114">isScheduledActionEnabled</span><span class="sxs-lookup"><span data-stu-id="b3cd2-114">isScheduledActionEnabled</span></span>|<span data-ttu-id="b3cd2-115">Booliano</span><span class="sxs-lookup"><span data-stu-id="b3cd2-115">Boolean</span></span>|<span data-ttu-id="b3cd2-116">O recurso está habilitado ou não para ação agendada para a regra.</span><span class="sxs-lookup"><span data-stu-id="b3cd2-116">Is feature enabled or not for scheduled action for rule.</span></span>|
|<span data-ttu-id="b3cd2-117">secureByDefault</span><span class="sxs-lookup"><span data-stu-id="b3cd2-117">secureByDefault</span></span>|<span data-ttu-id="b3cd2-118">Booliano</span><span class="sxs-lookup"><span data-stu-id="b3cd2-118">Boolean</span></span>|<span data-ttu-id="b3cd2-119">Quando true, o dispositivo deve ser incompatível quando não há nenhuma política de conformidade direcionada</span><span class="sxs-lookup"><span data-stu-id="b3cd2-119">Device should be noncompliant when there is no compliance policy targeted when this is true</span></span>|
|<span data-ttu-id="b3cd2-120">enhancedJailBreak</span><span class="sxs-lookup"><span data-stu-id="b3cd2-120">enhancedJailBreak</span></span>|<span data-ttu-id="b3cd2-121">Booliano</span><span class="sxs-lookup"><span data-stu-id="b3cd2-121">Boolean</span></span>|<span data-ttu-id="b3cd2-122">O recurso está habilitado ou não para a detecção de jailbreak avançada.</span><span class="sxs-lookup"><span data-stu-id="b3cd2-122">Is feature enabled or not for enhanced jailbreak detection.</span></span>|
|<span data-ttu-id="b3cd2-123">deviceInactivityBeforeRetirementInDay</span><span class="sxs-lookup"><span data-stu-id="b3cd2-123">deviceInactivityBeforeRetirementInDay</span></span>|<span data-ttu-id="b3cd2-124">Int32</span><span class="sxs-lookup"><span data-stu-id="b3cd2-124">Int32</span></span>|<span data-ttu-id="b3cd2-125">Quando o dispositivo não faz check-in por um número especificado de dias, os dados da empresa podem ser removidos e o dispositivo não estará sob gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="b3cd2-125">When the device does not check in for specified number of days, the company data might be removed and the device will not be under management.</span></span> <span data-ttu-id="b3cd2-126">Valores válidos de 30 a 270</span><span class="sxs-lookup"><span data-stu-id="b3cd2-126">Valid values 30 to 270</span></span>|
|<span data-ttu-id="b3cd2-127">derivedCredentialProvider</span><span class="sxs-lookup"><span data-stu-id="b3cd2-127">derivedCredentialProvider</span></span>|[<span data-ttu-id="b3cd2-128">derivedCredentialProviderType</span><span class="sxs-lookup"><span data-stu-id="b3cd2-128">derivedCredentialProviderType</span></span>](../resources/intune-deviceconfig-derivedcredentialprovidertype.md)|<span data-ttu-id="b3cd2-129">O provedor de credenciais derivado a ser usado para esta conta.</span><span class="sxs-lookup"><span data-stu-id="b3cd2-129">The Derived Credential Provider to use for this account.</span></span> <span data-ttu-id="b3cd2-130">Os valores possíveis são: `notConfigured`, `entrustDataCard`, `purebred`, `xTec`, `intercede`.</span><span class="sxs-lookup"><span data-stu-id="b3cd2-130">Possible values are: `notConfigured`, `entrustDataCard`, `purebred`, `xTec`, `intercede`.</span></span>|
|<span data-ttu-id="b3cd2-131">derivedCredentialUrl</span><span class="sxs-lookup"><span data-stu-id="b3cd2-131">derivedCredentialUrl</span></span>|<span data-ttu-id="b3cd2-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b3cd2-132">String</span></span>|<span data-ttu-id="b3cd2-133">O URI de autoatendimento do provedor de credenciais derivado.</span><span class="sxs-lookup"><span data-stu-id="b3cd2-133">The Derived Credential Provider self-service URI.</span></span>|
|<span data-ttu-id="b3cd2-134">androidDeviceAdministratorEnrollmentEnabled</span><span class="sxs-lookup"><span data-stu-id="b3cd2-134">androidDeviceAdministratorEnrollmentEnabled</span></span>|<span data-ttu-id="b3cd2-135">Booliano</span><span class="sxs-lookup"><span data-stu-id="b3cd2-135">Boolean</span></span>|<span data-ttu-id="b3cd2-136">A propriedade para determinar se o registro do administrador do dispositivo Android está habilitado para esta conta.</span><span class="sxs-lookup"><span data-stu-id="b3cd2-136">The property to determine if Android device administrator enrollment is enabled for this account.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b3cd2-137">Relações</span><span class="sxs-lookup"><span data-stu-id="b3cd2-137">Relationships</span></span>
<span data-ttu-id="b3cd2-138">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b3cd2-138">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b3cd2-139">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b3cd2-139">JSON Representation</span></span>
<span data-ttu-id="b3cd2-140">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b3cd2-140">Here is a JSON representation of the resource.</span></span>
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



