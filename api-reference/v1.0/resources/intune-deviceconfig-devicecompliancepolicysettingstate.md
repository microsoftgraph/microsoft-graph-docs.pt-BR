---
title: Tipo de recurso deviceCompliancePolicySettingState
description: Estado da configuração da política de conformidade de dispositivo para um determinado dispositivo.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 85de06b5baa9ff840ab0e1fd18cb70b0f5676e8b
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27962209"
---
# <a name="devicecompliancepolicysettingstate-resource-type"></a><span data-ttu-id="e4fd4-103">Tipo de recurso deviceCompliancePolicySettingState</span><span class="sxs-lookup"><span data-stu-id="e4fd4-103">deviceCompliancePolicySettingState resource type</span></span>

> <span data-ttu-id="e4fd4-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="e4fd4-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e4fd4-105">Estado da configuração da política de conformidade de dispositivo para um determinado dispositivo.</span><span class="sxs-lookup"><span data-stu-id="e4fd4-105">Device Compilance Policy Setting State for a given device.</span></span>
## <a name="properties"></a><span data-ttu-id="e4fd4-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e4fd4-106">Properties</span></span>
|<span data-ttu-id="e4fd4-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e4fd4-107">Property</span></span>|<span data-ttu-id="e4fd4-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="e4fd4-108">Type</span></span>|<span data-ttu-id="e4fd4-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="e4fd4-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e4fd4-110">configuração</span><span class="sxs-lookup"><span data-stu-id="e4fd4-110">setting</span></span>|<span data-ttu-id="e4fd4-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e4fd4-111">String</span></span>|<span data-ttu-id="e4fd4-112">A configuração que está sendo relatada</span><span class="sxs-lookup"><span data-stu-id="e4fd4-112">The setting that is being reported</span></span>|
|<span data-ttu-id="e4fd4-113">settingName</span><span class="sxs-lookup"><span data-stu-id="e4fd4-113">settingName</span></span>|<span data-ttu-id="e4fd4-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e4fd4-114">String</span></span>|<span data-ttu-id="e4fd4-115">Nome traduzido/amigável para o usuário da configuração que está sendo relatada</span><span class="sxs-lookup"><span data-stu-id="e4fd4-115">Localized/user friendly setting name that is being reported</span></span>|
|<span data-ttu-id="e4fd4-116">instanceDisplayName</span><span class="sxs-lookup"><span data-stu-id="e4fd4-116">instanceDisplayName</span></span>|<span data-ttu-id="e4fd4-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e4fd4-117">String</span></span>|<span data-ttu-id="e4fd4-118">Nome da instância de configuração está sendo relatada.</span><span class="sxs-lookup"><span data-stu-id="e4fd4-118">Name of setting instance that is being reported.</span></span>|
|<span data-ttu-id="e4fd4-119">estado</span><span class="sxs-lookup"><span data-stu-id="e4fd4-119">state</span></span>|[<span data-ttu-id="e4fd4-120">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="e4fd4-120">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="e4fd4-121">O estado de conformidade da configuração.</span><span class="sxs-lookup"><span data-stu-id="e4fd4-121">The compliance state of the setting.</span></span> <span data-ttu-id="e4fd4-122">Os valores possíveis são: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="e4fd4-122">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="e4fd4-123">errorCode</span><span class="sxs-lookup"><span data-stu-id="e4fd4-123">errorCode</span></span>|<span data-ttu-id="e4fd4-124">Int64</span><span class="sxs-lookup"><span data-stu-id="e4fd4-124">Int64</span></span>|<span data-ttu-id="e4fd4-125">Código de erro da configuração</span><span class="sxs-lookup"><span data-stu-id="e4fd4-125">Error code for the setting</span></span>|
|<span data-ttu-id="e4fd4-126">errorDescription</span><span class="sxs-lookup"><span data-stu-id="e4fd4-126">errorDescription</span></span>|<span data-ttu-id="e4fd4-127">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e4fd4-127">String</span></span>|<span data-ttu-id="e4fd4-128">Descrição do erro</span><span class="sxs-lookup"><span data-stu-id="e4fd4-128">Error description</span></span>|
|<span data-ttu-id="e4fd4-129">userId</span><span class="sxs-lookup"><span data-stu-id="e4fd4-129">userId</span></span>|<span data-ttu-id="e4fd4-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e4fd4-130">String</span></span>|<span data-ttu-id="e4fd4-131">UserId</span><span class="sxs-lookup"><span data-stu-id="e4fd4-131">UserId</span></span>|
|<span data-ttu-id="e4fd4-132">userName</span><span class="sxs-lookup"><span data-stu-id="e4fd4-132">userName</span></span>|<span data-ttu-id="e4fd4-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e4fd4-133">String</span></span>|<span data-ttu-id="e4fd4-134">UserName</span><span class="sxs-lookup"><span data-stu-id="e4fd4-134">UserName</span></span>|
|<span data-ttu-id="e4fd4-135">userEmail</span><span class="sxs-lookup"><span data-stu-id="e4fd4-135">userEmail</span></span>|<span data-ttu-id="e4fd4-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e4fd4-136">String</span></span>|<span data-ttu-id="e4fd4-137">UserEmail</span><span class="sxs-lookup"><span data-stu-id="e4fd4-137">UserEmail</span></span>|
|<span data-ttu-id="e4fd4-138">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="e4fd4-138">userPrincipalName</span></span>|<span data-ttu-id="e4fd4-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e4fd4-139">String</span></span>|<span data-ttu-id="e4fd4-140">UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="e4fd4-140">UserPrincipalName.</span></span>|
|<span data-ttu-id="e4fd4-141">sources</span><span class="sxs-lookup"><span data-stu-id="e4fd4-141">sources</span></span>|<span data-ttu-id="e4fd4-142">Coleção [settingSource](../resources/intune-deviceconfig-settingsource.md)</span><span class="sxs-lookup"><span data-stu-id="e4fd4-142">[settingSource](../resources/intune-deviceconfig-settingsource.md) collection</span></span>|<span data-ttu-id="e4fd4-143">Políticas colaboradoras</span><span class="sxs-lookup"><span data-stu-id="e4fd4-143">Contributing policies</span></span>|
|<span data-ttu-id="e4fd4-144">currentValue</span><span class="sxs-lookup"><span data-stu-id="e4fd4-144">currentValue</span></span>|<span data-ttu-id="e4fd4-145">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e4fd4-145">String</span></span>|<span data-ttu-id="e4fd4-146">Valor atual da configuração no dispositivo</span><span class="sxs-lookup"><span data-stu-id="e4fd4-146">Current value of setting on device</span></span>|

## <a name="relationships"></a><span data-ttu-id="e4fd4-147">Relações</span><span class="sxs-lookup"><span data-stu-id="e4fd4-147">Relationships</span></span>
<span data-ttu-id="e4fd4-148">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e4fd4-148">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="e4fd4-149">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e4fd4-149">JSON Representation</span></span>
<span data-ttu-id="e4fd4-150">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e4fd4-150">Here is a JSON representation of the resource.</span></span>
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



