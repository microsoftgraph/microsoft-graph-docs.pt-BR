---
title: Tipo de recurso deviceManagementSettings
description: Ainda não documentado
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 4f676eed1acbf6711f526e612bd6c073b749607d
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29417662"
---
# <a name="devicemanagementsettings-resource-type"></a><span data-ttu-id="64e36-103">Tipo de recurso deviceManagementSettings</span><span class="sxs-lookup"><span data-stu-id="64e36-103">deviceManagementSettings resource type</span></span>

> <span data-ttu-id="64e36-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="64e36-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="64e36-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="64e36-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="64e36-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="64e36-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="64e36-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="64e36-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="64e36-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="64e36-108">Properties</span></span>
|<span data-ttu-id="64e36-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="64e36-109">Property</span></span>|<span data-ttu-id="64e36-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="64e36-110">Type</span></span>|<span data-ttu-id="64e36-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="64e36-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="64e36-112">deviceComplianceCheckinThresholdDays</span><span class="sxs-lookup"><span data-stu-id="64e36-112">deviceComplianceCheckinThresholdDays</span></span>|<span data-ttu-id="64e36-113">Int32</span><span class="sxs-lookup"><span data-stu-id="64e36-113">Int32</span></span>|<span data-ttu-id="64e36-114">O número de dias que tem um dispositivo pode ser executado sem fazer check-in para permanecer em conformidade.</span><span class="sxs-lookup"><span data-stu-id="64e36-114">The number of days a device is allowed to go without checking in to remain compliant.</span></span> <span data-ttu-id="64e36-115">Valores válidos de 0 a 120</span><span class="sxs-lookup"><span data-stu-id="64e36-115">Valid values 0 to 120</span></span>|
|<span data-ttu-id="64e36-116">isScheduledActionEnabled</span><span class="sxs-lookup"><span data-stu-id="64e36-116">isScheduledActionEnabled</span></span>|<span data-ttu-id="64e36-117">Booliano</span><span class="sxs-lookup"><span data-stu-id="64e36-117">Boolean</span></span>|<span data-ttu-id="64e36-118">O recurso está habilitado ou não para ação agendada para a regra.</span><span class="sxs-lookup"><span data-stu-id="64e36-118">Is feature enabled or not for scheduled action for rule.</span></span>|
|<span data-ttu-id="64e36-119">secureByDefault</span><span class="sxs-lookup"><span data-stu-id="64e36-119">secureByDefault</span></span>|<span data-ttu-id="64e36-120">Booliano</span><span class="sxs-lookup"><span data-stu-id="64e36-120">Boolean</span></span>|<span data-ttu-id="64e36-121">Quando true, o dispositivo deve ser incompatível quando não há nenhuma política de conformidade direcionada</span><span class="sxs-lookup"><span data-stu-id="64e36-121">Device should be noncompliant when there is no compliance policy targeted when this is true</span></span>|
|<span data-ttu-id="64e36-122">enhancedJailBreak</span><span class="sxs-lookup"><span data-stu-id="64e36-122">enhancedJailBreak</span></span>|<span data-ttu-id="64e36-123">Boolean</span><span class="sxs-lookup"><span data-stu-id="64e36-123">Boolean</span></span>|<span data-ttu-id="64e36-124">É o recurso habilitado ou não para maior detecção de jailbreak.</span><span class="sxs-lookup"><span data-stu-id="64e36-124">Is feature enabled or not for enhanced jailbreak detection.</span></span>|
|<span data-ttu-id="64e36-125">deviceInactivityBeforeRetirementInDay</span><span class="sxs-lookup"><span data-stu-id="64e36-125">deviceInactivityBeforeRetirementInDay</span></span>|<span data-ttu-id="64e36-126">Int32</span><span class="sxs-lookup"><span data-stu-id="64e36-126">Int32</span></span>|<span data-ttu-id="64e36-127">Quando o dispositivo não check-in do número especificado de dias, os dados da empresa podem ser removidos e o dispositivo não estará sob gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="64e36-127">When the device does not check in for specified number of days, the company data might be removed and the device will not be under management.</span></span> <span data-ttu-id="64e36-128">Valores válidos 30 a 270</span><span class="sxs-lookup"><span data-stu-id="64e36-128">Valid values 30 to 270</span></span>|
|<span data-ttu-id="64e36-129">derivedCredentialProvider</span><span class="sxs-lookup"><span data-stu-id="64e36-129">derivedCredentialProvider</span></span>|[<span data-ttu-id="64e36-130">derivedCredentialProviderType</span><span class="sxs-lookup"><span data-stu-id="64e36-130">derivedCredentialProviderType</span></span>](../resources/intune-deviceconfig-derivedcredentialprovidertype.md)|<span data-ttu-id="64e36-131">O provedor de credenciais derivados a ser usado para essa conta.</span><span class="sxs-lookup"><span data-stu-id="64e36-131">The Derived Credential Provider to use for this account.</span></span> <span data-ttu-id="64e36-132">Os valores possíveis são: `notConfigured`, `entrustDataCard`, `purebred`, `xTec`, `intercede`.</span><span class="sxs-lookup"><span data-stu-id="64e36-132">Possible values are: `notConfigured`, `entrustDataCard`, `purebred`, `xTec`, `intercede`.</span></span>|
|<span data-ttu-id="64e36-133">derivedCredentialUrl</span><span class="sxs-lookup"><span data-stu-id="64e36-133">derivedCredentialUrl</span></span>|<span data-ttu-id="64e36-134">String</span><span class="sxs-lookup"><span data-stu-id="64e36-134">String</span></span>|<span data-ttu-id="64e36-135">O URI de autoatendimento derivados provedor de credenciais.</span><span class="sxs-lookup"><span data-stu-id="64e36-135">The Derived Credential Provider self-service URI.</span></span>|

## <a name="relationships"></a><span data-ttu-id="64e36-136">Relações</span><span class="sxs-lookup"><span data-stu-id="64e36-136">Relationships</span></span>
<span data-ttu-id="64e36-137">Nenhum</span><span class="sxs-lookup"><span data-stu-id="64e36-137">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="64e36-138">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="64e36-138">JSON Representation</span></span>
<span data-ttu-id="64e36-139">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="64e36-139">Here is a JSON representation of the resource.</span></span>
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
  "derivedCredentialUrl": "String"
}
```




