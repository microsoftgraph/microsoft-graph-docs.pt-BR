---
title: Tipo de recurso deviceCompliancePolicySettingState
description: Estado da configuração da política de conformidade de dispositivo para um determinado dispositivo.
author: tfitzmac
ms.openlocfilehash: 3dcd63327a3518314619cd7add6ac6f23e69396b
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27320367"
---
# <a name="devicecompliancepolicysettingstate-resource-type"></a><span data-ttu-id="e22c7-103">Tipo de recurso deviceCompliancePolicySettingState</span><span class="sxs-lookup"><span data-stu-id="e22c7-103">deviceCompliancePolicySettingState resource type</span></span>

> <span data-ttu-id="e22c7-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="e22c7-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e22c7-105">Estado da configuração da política de conformidade de dispositivo para um determinado dispositivo.</span><span class="sxs-lookup"><span data-stu-id="e22c7-105">Device Compilance Policy Setting State for a given device.</span></span>
## <a name="properties"></a><span data-ttu-id="e22c7-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e22c7-106">Properties</span></span>
|<span data-ttu-id="e22c7-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e22c7-107">Property</span></span>|<span data-ttu-id="e22c7-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="e22c7-108">Type</span></span>|<span data-ttu-id="e22c7-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="e22c7-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e22c7-110">configuração</span><span class="sxs-lookup"><span data-stu-id="e22c7-110">setting</span></span>|<span data-ttu-id="e22c7-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e22c7-111">String</span></span>|<span data-ttu-id="e22c7-112">A configuração que está sendo relatada</span><span class="sxs-lookup"><span data-stu-id="e22c7-112">The setting that is being reported</span></span>|
|<span data-ttu-id="e22c7-113">settingName</span><span class="sxs-lookup"><span data-stu-id="e22c7-113">settingName</span></span>|<span data-ttu-id="e22c7-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e22c7-114">String</span></span>|<span data-ttu-id="e22c7-115">Nome traduzido/amigável para o usuário da configuração que está sendo relatada</span><span class="sxs-lookup"><span data-stu-id="e22c7-115">Localized/user friendly setting name that is being reported</span></span>|
|<span data-ttu-id="e22c7-116">instanceDisplayName</span><span class="sxs-lookup"><span data-stu-id="e22c7-116">instanceDisplayName</span></span>|<span data-ttu-id="e22c7-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e22c7-117">String</span></span>|<span data-ttu-id="e22c7-118">Nome da instância de configuração está sendo relatada.</span><span class="sxs-lookup"><span data-stu-id="e22c7-118">Name of setting instance that is being reported.</span></span>|
|<span data-ttu-id="e22c7-119">estado</span><span class="sxs-lookup"><span data-stu-id="e22c7-119">state</span></span>|[<span data-ttu-id="e22c7-120">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="e22c7-120">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="e22c7-121">O estado de conformidade da configuração.</span><span class="sxs-lookup"><span data-stu-id="e22c7-121">The compliance state of the setting.</span></span> <span data-ttu-id="e22c7-122">Os valores possíveis são: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="e22c7-122">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="e22c7-123">errorCode</span><span class="sxs-lookup"><span data-stu-id="e22c7-123">errorCode</span></span>|<span data-ttu-id="e22c7-124">Int64</span><span class="sxs-lookup"><span data-stu-id="e22c7-124">Int64</span></span>|<span data-ttu-id="e22c7-125">Código de erro da configuração</span><span class="sxs-lookup"><span data-stu-id="e22c7-125">Error code for the setting</span></span>|
|<span data-ttu-id="e22c7-126">errorDescription</span><span class="sxs-lookup"><span data-stu-id="e22c7-126">errorDescription</span></span>|<span data-ttu-id="e22c7-127">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e22c7-127">String</span></span>|<span data-ttu-id="e22c7-128">Descrição do erro</span><span class="sxs-lookup"><span data-stu-id="e22c7-128">Error description</span></span>|
|<span data-ttu-id="e22c7-129">userId</span><span class="sxs-lookup"><span data-stu-id="e22c7-129">userId</span></span>|<span data-ttu-id="e22c7-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e22c7-130">String</span></span>|<span data-ttu-id="e22c7-131">UserId</span><span class="sxs-lookup"><span data-stu-id="e22c7-131">UserId</span></span>|
|<span data-ttu-id="e22c7-132">userName</span><span class="sxs-lookup"><span data-stu-id="e22c7-132">userName</span></span>|<span data-ttu-id="e22c7-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e22c7-133">String</span></span>|<span data-ttu-id="e22c7-134">UserName</span><span class="sxs-lookup"><span data-stu-id="e22c7-134">UserName</span></span>|
|<span data-ttu-id="e22c7-135">userEmail</span><span class="sxs-lookup"><span data-stu-id="e22c7-135">userEmail</span></span>|<span data-ttu-id="e22c7-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e22c7-136">String</span></span>|<span data-ttu-id="e22c7-137">UserEmail</span><span class="sxs-lookup"><span data-stu-id="e22c7-137">UserEmail</span></span>|
|<span data-ttu-id="e22c7-138">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="e22c7-138">userPrincipalName</span></span>|<span data-ttu-id="e22c7-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e22c7-139">String</span></span>|<span data-ttu-id="e22c7-140">UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="e22c7-140">UserPrincipalName.</span></span>|
|<span data-ttu-id="e22c7-141">sources</span><span class="sxs-lookup"><span data-stu-id="e22c7-141">sources</span></span>|<span data-ttu-id="e22c7-142">Coleção [settingSource](../resources/intune-deviceconfig-settingsource.md)</span><span class="sxs-lookup"><span data-stu-id="e22c7-142">[settingSource](../resources/intune-deviceconfig-settingsource.md) collection</span></span>|<span data-ttu-id="e22c7-143">Políticas colaboradoras</span><span class="sxs-lookup"><span data-stu-id="e22c7-143">Contributing policies</span></span>|
|<span data-ttu-id="e22c7-144">currentValue</span><span class="sxs-lookup"><span data-stu-id="e22c7-144">currentValue</span></span>|<span data-ttu-id="e22c7-145">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e22c7-145">String</span></span>|<span data-ttu-id="e22c7-146">Valor atual da configuração no dispositivo</span><span class="sxs-lookup"><span data-stu-id="e22c7-146">Current value of setting on device</span></span>|

## <a name="relationships"></a><span data-ttu-id="e22c7-147">Relações</span><span class="sxs-lookup"><span data-stu-id="e22c7-147">Relationships</span></span>
<span data-ttu-id="e22c7-148">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e22c7-148">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="e22c7-149">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e22c7-149">JSON Representation</span></span>
<span data-ttu-id="e22c7-150">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e22c7-150">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceCompliancePolicySettingState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicySettingState",
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
  "currentValue": "String"
}
```



