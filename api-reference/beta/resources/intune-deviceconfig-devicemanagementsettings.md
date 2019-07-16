---
title: Tipo de recurso deviceManagementSettings
description: Ainda não documentado
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 025008a74df37daee068fe557df1511d60dcc48f
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35734455"
---
# <a name="devicemanagementsettings-resource-type"></a><span data-ttu-id="d6b52-103">Tipo de recurso deviceManagementSettings</span><span class="sxs-lookup"><span data-stu-id="d6b52-103">deviceManagementSettings resource type</span></span>

> <span data-ttu-id="d6b52-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d6b52-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d6b52-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d6b52-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d6b52-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="d6b52-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="d6b52-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d6b52-107">Properties</span></span>
|<span data-ttu-id="d6b52-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d6b52-108">Property</span></span>|<span data-ttu-id="d6b52-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="d6b52-109">Type</span></span>|<span data-ttu-id="d6b52-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="d6b52-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d6b52-111">deviceComplianceCheckinThresholdDays</span><span class="sxs-lookup"><span data-stu-id="d6b52-111">deviceComplianceCheckinThresholdDays</span></span>|<span data-ttu-id="d6b52-112">Int32</span><span class="sxs-lookup"><span data-stu-id="d6b52-112">Int32</span></span>|<span data-ttu-id="d6b52-113">O número de dias que tem um dispositivo pode ser executado sem fazer check-in para permanecer em conformidade.</span><span class="sxs-lookup"><span data-stu-id="d6b52-113">The number of days a device is allowed to go without checking in to remain compliant.</span></span> <span data-ttu-id="d6b52-114">Valores válidos de 0 a 120</span><span class="sxs-lookup"><span data-stu-id="d6b52-114">Valid values 0 to 120</span></span>|
|<span data-ttu-id="d6b52-115">isScheduledActionEnabled</span><span class="sxs-lookup"><span data-stu-id="d6b52-115">isScheduledActionEnabled</span></span>|<span data-ttu-id="d6b52-116">Booliano</span><span class="sxs-lookup"><span data-stu-id="d6b52-116">Boolean</span></span>|<span data-ttu-id="d6b52-117">O recurso está habilitado ou não para ação agendada para a regra.</span><span class="sxs-lookup"><span data-stu-id="d6b52-117">Is feature enabled or not for scheduled action for rule.</span></span>|
|<span data-ttu-id="d6b52-118">secureByDefault</span><span class="sxs-lookup"><span data-stu-id="d6b52-118">secureByDefault</span></span>|<span data-ttu-id="d6b52-119">Booliano</span><span class="sxs-lookup"><span data-stu-id="d6b52-119">Boolean</span></span>|<span data-ttu-id="d6b52-120">Quando true, o dispositivo deve ser incompatível quando não há nenhuma política de conformidade direcionada</span><span class="sxs-lookup"><span data-stu-id="d6b52-120">Device should be noncompliant when there is no compliance policy targeted when this is true</span></span>|
|<span data-ttu-id="d6b52-121">enhancedJailBreak</span><span class="sxs-lookup"><span data-stu-id="d6b52-121">enhancedJailBreak</span></span>|<span data-ttu-id="d6b52-122">Booliano</span><span class="sxs-lookup"><span data-stu-id="d6b52-122">Boolean</span></span>|<span data-ttu-id="d6b52-123">O recurso está habilitado ou não para a detecção de jailbreak avançada.</span><span class="sxs-lookup"><span data-stu-id="d6b52-123">Is feature enabled or not for enhanced jailbreak detection.</span></span>|
|<span data-ttu-id="d6b52-124">deviceInactivityBeforeRetirementInDay</span><span class="sxs-lookup"><span data-stu-id="d6b52-124">deviceInactivityBeforeRetirementInDay</span></span>|<span data-ttu-id="d6b52-125">Int32</span><span class="sxs-lookup"><span data-stu-id="d6b52-125">Int32</span></span>|<span data-ttu-id="d6b52-126">Quando o dispositivo não faz check-in por um número especificado de dias, os dados da empresa podem ser removidos e o dispositivo não estará sob gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="d6b52-126">When the device does not check in for specified number of days, the company data might be removed and the device will not be under management.</span></span> <span data-ttu-id="d6b52-127">Valores válidos de 30 a 270</span><span class="sxs-lookup"><span data-stu-id="d6b52-127">Valid values 30 to 270</span></span>|
|<span data-ttu-id="d6b52-128">derivedCredentialProvider</span><span class="sxs-lookup"><span data-stu-id="d6b52-128">derivedCredentialProvider</span></span>|[<span data-ttu-id="d6b52-129">derivedCredentialProviderType</span><span class="sxs-lookup"><span data-stu-id="d6b52-129">derivedCredentialProviderType</span></span>](../resources/intune-deviceconfig-derivedcredentialprovidertype.md)|<span data-ttu-id="d6b52-130">O provedor de credenciais derivado a ser usado para esta conta.</span><span class="sxs-lookup"><span data-stu-id="d6b52-130">The Derived Credential Provider to use for this account.</span></span> <span data-ttu-id="d6b52-131">Os valores possíveis são: `notConfigured`, `entrustDataCard`, `purebred`, `xTec`, `intercede`.</span><span class="sxs-lookup"><span data-stu-id="d6b52-131">Possible values are: `notConfigured`, `entrustDataCard`, `purebred`, `xTec`, `intercede`.</span></span>|
|<span data-ttu-id="d6b52-132">derivedCredentialUrl</span><span class="sxs-lookup"><span data-stu-id="d6b52-132">derivedCredentialUrl</span></span>|<span data-ttu-id="d6b52-133">String</span><span class="sxs-lookup"><span data-stu-id="d6b52-133">String</span></span>|<span data-ttu-id="d6b52-134">O URI de autoatendimento do provedor de credenciais derivado.</span><span class="sxs-lookup"><span data-stu-id="d6b52-134">The Derived Credential Provider self-service URI.</span></span>|
|<span data-ttu-id="d6b52-135">androidDeviceAdministratorEnrollmentEnabled</span><span class="sxs-lookup"><span data-stu-id="d6b52-135">androidDeviceAdministratorEnrollmentEnabled</span></span>|<span data-ttu-id="d6b52-136">Booliano</span><span class="sxs-lookup"><span data-stu-id="d6b52-136">Boolean</span></span>|<span data-ttu-id="d6b52-137">A propriedade para determinar se o registro do administrador do dispositivo Android está habilitado para esta conta.</span><span class="sxs-lookup"><span data-stu-id="d6b52-137">The property to determine if Android device administrator enrollment is enabled for this account.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d6b52-138">Relações</span><span class="sxs-lookup"><span data-stu-id="d6b52-138">Relationships</span></span>
<span data-ttu-id="d6b52-139">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d6b52-139">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d6b52-140">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d6b52-140">JSON Representation</span></span>
<span data-ttu-id="d6b52-141">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d6b52-141">Here is a JSON representation of the resource.</span></span>
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





