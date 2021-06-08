---
title: Tipo de recurso deviceCompliancePolicySettingState
description: Estado da configuração da política de conformidade de dispositivo para um determinado dispositivo.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 0a7bdee8183ad86306234b446813c9272137113d
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52760110"
---
# <a name="devicecompliancepolicysettingstate-resource-type"></a><span data-ttu-id="19a1d-103">Tipo de recurso deviceCompliancePolicySettingState</span><span class="sxs-lookup"><span data-stu-id="19a1d-103">deviceCompliancePolicySettingState resource type</span></span>

<span data-ttu-id="19a1d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="19a1d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="19a1d-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="19a1d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="19a1d-106">Estado da configuração da política de conformidade de dispositivo para um determinado dispositivo.</span><span class="sxs-lookup"><span data-stu-id="19a1d-106">Device Compilance Policy Setting State for a given device.</span></span>

## <a name="properties"></a><span data-ttu-id="19a1d-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="19a1d-107">Properties</span></span>
|<span data-ttu-id="19a1d-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="19a1d-108">Property</span></span>|<span data-ttu-id="19a1d-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="19a1d-109">Type</span></span>|<span data-ttu-id="19a1d-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="19a1d-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="19a1d-111">configuração</span><span class="sxs-lookup"><span data-stu-id="19a1d-111">setting</span></span>|<span data-ttu-id="19a1d-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="19a1d-112">String</span></span>|<span data-ttu-id="19a1d-113">A configuração que é relatada</span><span class="sxs-lookup"><span data-stu-id="19a1d-113">The setting that is being reported</span></span>|
|<span data-ttu-id="19a1d-114">settingName</span><span class="sxs-lookup"><span data-stu-id="19a1d-114">settingName</span></span>|<span data-ttu-id="19a1d-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="19a1d-115">String</span></span>|<span data-ttu-id="19a1d-116">Nome de configuração localizada/de usuário que é relatada</span><span class="sxs-lookup"><span data-stu-id="19a1d-116">Localized/user friendly setting name that is being reported</span></span>|
|<span data-ttu-id="19a1d-117">instanceDisplayName</span><span class="sxs-lookup"><span data-stu-id="19a1d-117">instanceDisplayName</span></span>|<span data-ttu-id="19a1d-118">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="19a1d-118">String</span></span>|<span data-ttu-id="19a1d-119">Nome da instância de configuração que é relatada.</span><span class="sxs-lookup"><span data-stu-id="19a1d-119">Name of setting instance that is being reported.</span></span>|
|<span data-ttu-id="19a1d-120">state</span><span class="sxs-lookup"><span data-stu-id="19a1d-120">state</span></span>|[<span data-ttu-id="19a1d-121">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="19a1d-121">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="19a1d-122">O estado de conformidade da configuração.</span><span class="sxs-lookup"><span data-stu-id="19a1d-122">The compliance state of the setting.</span></span> <span data-ttu-id="19a1d-123">Os valores possíveis são: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="19a1d-123">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="19a1d-124">errorCode</span><span class="sxs-lookup"><span data-stu-id="19a1d-124">errorCode</span></span>|<span data-ttu-id="19a1d-125">Int64</span><span class="sxs-lookup"><span data-stu-id="19a1d-125">Int64</span></span>|<span data-ttu-id="19a1d-126">Código de erro da configuração</span><span class="sxs-lookup"><span data-stu-id="19a1d-126">Error code for the setting</span></span>|
|<span data-ttu-id="19a1d-127">errorDescription</span><span class="sxs-lookup"><span data-stu-id="19a1d-127">errorDescription</span></span>|<span data-ttu-id="19a1d-128">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="19a1d-128">String</span></span>|<span data-ttu-id="19a1d-129">Descrição de erro</span><span class="sxs-lookup"><span data-stu-id="19a1d-129">Error description</span></span>|
|<span data-ttu-id="19a1d-130">userId</span><span class="sxs-lookup"><span data-stu-id="19a1d-130">userId</span></span>|<span data-ttu-id="19a1d-131">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="19a1d-131">String</span></span>|<span data-ttu-id="19a1d-132">UserId</span><span class="sxs-lookup"><span data-stu-id="19a1d-132">UserId</span></span>|
|<span data-ttu-id="19a1d-133">userName</span><span class="sxs-lookup"><span data-stu-id="19a1d-133">userName</span></span>|<span data-ttu-id="19a1d-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="19a1d-134">String</span></span>|<span data-ttu-id="19a1d-135">UserName</span><span class="sxs-lookup"><span data-stu-id="19a1d-135">UserName</span></span>|
|<span data-ttu-id="19a1d-136">userEmail</span><span class="sxs-lookup"><span data-stu-id="19a1d-136">userEmail</span></span>|<span data-ttu-id="19a1d-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="19a1d-137">String</span></span>|<span data-ttu-id="19a1d-138">UserEmail</span><span class="sxs-lookup"><span data-stu-id="19a1d-138">UserEmail</span></span>|
|<span data-ttu-id="19a1d-139">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="19a1d-139">userPrincipalName</span></span>|<span data-ttu-id="19a1d-140">String</span><span class="sxs-lookup"><span data-stu-id="19a1d-140">String</span></span>|<span data-ttu-id="19a1d-141">UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="19a1d-141">UserPrincipalName.</span></span>|
|<span data-ttu-id="19a1d-142">fontes</span><span class="sxs-lookup"><span data-stu-id="19a1d-142">sources</span></span>|<span data-ttu-id="19a1d-143">Conjunto [settingSource](../resources/intune-deviceconfig-settingsource.md)</span><span class="sxs-lookup"><span data-stu-id="19a1d-143">[settingSource](../resources/intune-deviceconfig-settingsource.md) collection</span></span>|<span data-ttu-id="19a1d-144">Políticas de colaboração</span><span class="sxs-lookup"><span data-stu-id="19a1d-144">Contributing policies</span></span>|
|<span data-ttu-id="19a1d-145">currentValue</span><span class="sxs-lookup"><span data-stu-id="19a1d-145">currentValue</span></span>|<span data-ttu-id="19a1d-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="19a1d-146">String</span></span>|<span data-ttu-id="19a1d-147">Valor atual da configuração em um dispositivo</span><span class="sxs-lookup"><span data-stu-id="19a1d-147">Current value of setting on device</span></span>|

## <a name="relationships"></a><span data-ttu-id="19a1d-148">Relações</span><span class="sxs-lookup"><span data-stu-id="19a1d-148">Relationships</span></span>
<span data-ttu-id="19a1d-149">Nenhum</span><span class="sxs-lookup"><span data-stu-id="19a1d-149">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="19a1d-150">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="19a1d-150">JSON Representation</span></span>
<span data-ttu-id="19a1d-151">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="19a1d-151">Here is a JSON representation of the resource.</span></span>
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
      "displayName": "String",
      "sourceType": "String"
    }
  ],
  "currentValue": "String"
}
```




