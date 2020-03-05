---
title: Tipo de recurso deviceManagementSettings
description: Ainda não documentado
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: f3c6e3f718cb7b3915daecc700e55b733947530c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42526595"
---
# <a name="devicemanagementsettings-resource-type"></a><span data-ttu-id="6784b-103">Tipo de recurso deviceManagementSettings</span><span class="sxs-lookup"><span data-stu-id="6784b-103">deviceManagementSettings resource type</span></span>

<span data-ttu-id="6784b-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="6784b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6784b-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="6784b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6784b-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6784b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6784b-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="6784b-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="6784b-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6784b-108">Properties</span></span>
|<span data-ttu-id="6784b-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6784b-109">Property</span></span>|<span data-ttu-id="6784b-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="6784b-110">Type</span></span>|<span data-ttu-id="6784b-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="6784b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6784b-112">deviceComplianceCheckinThresholdDays</span><span class="sxs-lookup"><span data-stu-id="6784b-112">deviceComplianceCheckinThresholdDays</span></span>|<span data-ttu-id="6784b-113">Int32</span><span class="sxs-lookup"><span data-stu-id="6784b-113">Int32</span></span>|<span data-ttu-id="6784b-114">O número de dias que tem um dispositivo pode ser executado sem fazer check-in para permanecer em conformidade.</span><span class="sxs-lookup"><span data-stu-id="6784b-114">The number of days a device is allowed to go without checking in to remain compliant.</span></span>|
|<span data-ttu-id="6784b-115">isScheduledActionEnabled</span><span class="sxs-lookup"><span data-stu-id="6784b-115">isScheduledActionEnabled</span></span>|<span data-ttu-id="6784b-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="6784b-116">Boolean</span></span>|<span data-ttu-id="6784b-117">O recurso está habilitado ou não para ação agendada para a regra.</span><span class="sxs-lookup"><span data-stu-id="6784b-117">Is feature enabled or not for scheduled action for rule.</span></span>|
|<span data-ttu-id="6784b-118">secureByDefault</span><span class="sxs-lookup"><span data-stu-id="6784b-118">secureByDefault</span></span>|<span data-ttu-id="6784b-119">Booliano</span><span class="sxs-lookup"><span data-stu-id="6784b-119">Boolean</span></span>|<span data-ttu-id="6784b-120">Quando true, o dispositivo deve ser incompatível quando não há nenhuma política de conformidade direcionada</span><span class="sxs-lookup"><span data-stu-id="6784b-120">Device should be noncompliant when there is no compliance policy targeted when this is true</span></span>|
|<span data-ttu-id="6784b-121">enhancedJailBreak</span><span class="sxs-lookup"><span data-stu-id="6784b-121">enhancedJailBreak</span></span>|<span data-ttu-id="6784b-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="6784b-122">Boolean</span></span>|<span data-ttu-id="6784b-123">O recurso está habilitado ou não para a detecção de jailbreak avançada.</span><span class="sxs-lookup"><span data-stu-id="6784b-123">Is feature enabled or not for enhanced jailbreak detection.</span></span>|
|<span data-ttu-id="6784b-124">deviceInactivityBeforeRetirementInDay</span><span class="sxs-lookup"><span data-stu-id="6784b-124">deviceInactivityBeforeRetirementInDay</span></span>|<span data-ttu-id="6784b-125">Int32</span><span class="sxs-lookup"><span data-stu-id="6784b-125">Int32</span></span>|<span data-ttu-id="6784b-126">Quando o dispositivo não faz check-in por um número especificado de dias, os dados da empresa podem ser removidos e o dispositivo não estará sob gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="6784b-126">When the device does not check in for specified number of days, the company data might be removed and the device will not be under management.</span></span> <span data-ttu-id="6784b-127">Valores válidos de 30 a 270</span><span class="sxs-lookup"><span data-stu-id="6784b-127">Valid values 30 to 270</span></span>|
|<span data-ttu-id="6784b-128">derivedCredentialProvider</span><span class="sxs-lookup"><span data-stu-id="6784b-128">derivedCredentialProvider</span></span>|[<span data-ttu-id="6784b-129">derivedCredentialProviderType</span><span class="sxs-lookup"><span data-stu-id="6784b-129">derivedCredentialProviderType</span></span>](../resources/intune-deviceconfig-derivedcredentialprovidertype.md)|<span data-ttu-id="6784b-130">O provedor de credenciais derivado a ser usado para esta conta.</span><span class="sxs-lookup"><span data-stu-id="6784b-130">The Derived Credential Provider to use for this account.</span></span> <span data-ttu-id="6784b-131">Os valores possíveis são: `notConfigured`, `entrustDataCard`, `purebred`, `xTec`, `intercede`.</span><span class="sxs-lookup"><span data-stu-id="6784b-131">Possible values are: `notConfigured`, `entrustDataCard`, `purebred`, `xTec`, `intercede`.</span></span>|
|<span data-ttu-id="6784b-132">derivedCredentialUrl</span><span class="sxs-lookup"><span data-stu-id="6784b-132">derivedCredentialUrl</span></span>|<span data-ttu-id="6784b-133">String</span><span class="sxs-lookup"><span data-stu-id="6784b-133">String</span></span>|<span data-ttu-id="6784b-134">O URI de autoatendimento do provedor de credenciais derivado.</span><span class="sxs-lookup"><span data-stu-id="6784b-134">The Derived Credential Provider self-service URI.</span></span>|
|<span data-ttu-id="6784b-135">androidDeviceAdministratorEnrollmentEnabled</span><span class="sxs-lookup"><span data-stu-id="6784b-135">androidDeviceAdministratorEnrollmentEnabled</span></span>|<span data-ttu-id="6784b-136">Boolean</span><span class="sxs-lookup"><span data-stu-id="6784b-136">Boolean</span></span>|<span data-ttu-id="6784b-137">A propriedade para determinar se o registro do administrador do dispositivo Android está habilitado para esta conta.</span><span class="sxs-lookup"><span data-stu-id="6784b-137">The property to determine if Android device administrator enrollment is enabled for this account.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6784b-138">Relações</span><span class="sxs-lookup"><span data-stu-id="6784b-138">Relationships</span></span>
<span data-ttu-id="6784b-139">Nenhum</span><span class="sxs-lookup"><span data-stu-id="6784b-139">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6784b-140">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6784b-140">JSON Representation</span></span>
<span data-ttu-id="6784b-141">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6784b-141">Here is a JSON representation of the resource.</span></span>
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



