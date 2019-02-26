---
title: Tipo de recurso deviceCompliancePolicySettingState
description: Estado da configuração da política de conformidade de dispositivo para um determinado dispositivo.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c4d291f84a8c4404ff5b4425680260997b6b452f
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/26/2019
ms.locfileid: "30261744"
---
# <a name="devicecompliancepolicysettingstate-resource-type"></a><span data-ttu-id="e1eb5-103">Tipo de recurso deviceCompliancePolicySettingState</span><span class="sxs-lookup"><span data-stu-id="e1eb5-103">deviceCompliancePolicySettingState resource type</span></span>

> <span data-ttu-id="e1eb5-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e1eb5-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e1eb5-105">Estado da configuração da política de conformidade de dispositivo para um determinado dispositivo.</span><span class="sxs-lookup"><span data-stu-id="e1eb5-105">Device Compilance Policy Setting State for a given device.</span></span>

## <a name="properties"></a><span data-ttu-id="e1eb5-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e1eb5-106">Properties</span></span>
|<span data-ttu-id="e1eb5-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e1eb5-107">Property</span></span>|<span data-ttu-id="e1eb5-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="e1eb5-108">Type</span></span>|<span data-ttu-id="e1eb5-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="e1eb5-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e1eb5-110">configuração</span><span class="sxs-lookup"><span data-stu-id="e1eb5-110">setting</span></span>|<span data-ttu-id="e1eb5-111">String</span><span class="sxs-lookup"><span data-stu-id="e1eb5-111">String</span></span>|<span data-ttu-id="e1eb5-112">A configuração que está sendo relatada</span><span class="sxs-lookup"><span data-stu-id="e1eb5-112">The setting that is being reported</span></span>|
|<span data-ttu-id="e1eb5-113">settingName</span><span class="sxs-lookup"><span data-stu-id="e1eb5-113">settingName</span></span>|<span data-ttu-id="e1eb5-114">String</span><span class="sxs-lookup"><span data-stu-id="e1eb5-114">String</span></span>|<span data-ttu-id="e1eb5-115">Nome traduzido/amigável para o usuário da configuração que está sendo relatada</span><span class="sxs-lookup"><span data-stu-id="e1eb5-115">Localized/user friendly setting name that is being reported</span></span>|
|<span data-ttu-id="e1eb5-116">instanceDisplayName</span><span class="sxs-lookup"><span data-stu-id="e1eb5-116">instanceDisplayName</span></span>|<span data-ttu-id="e1eb5-117">String</span><span class="sxs-lookup"><span data-stu-id="e1eb5-117">String</span></span>|<span data-ttu-id="e1eb5-118">Nome da instância de configuração está sendo relatada.</span><span class="sxs-lookup"><span data-stu-id="e1eb5-118">Name of setting instance that is being reported.</span></span>|
|<span data-ttu-id="e1eb5-119">state</span><span class="sxs-lookup"><span data-stu-id="e1eb5-119">state</span></span>|[<span data-ttu-id="e1eb5-120">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="e1eb5-120">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="e1eb5-121">O estado de conformidade da configuração.</span><span class="sxs-lookup"><span data-stu-id="e1eb5-121">The compliance state of the setting.</span></span> <span data-ttu-id="e1eb5-122">Os valores possíveis são: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="e1eb5-122">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="e1eb5-123">errorCode</span><span class="sxs-lookup"><span data-stu-id="e1eb5-123">errorCode</span></span>|<span data-ttu-id="e1eb5-124">Int64</span><span class="sxs-lookup"><span data-stu-id="e1eb5-124">Int64</span></span>|<span data-ttu-id="e1eb5-125">Código de erro da configuração</span><span class="sxs-lookup"><span data-stu-id="e1eb5-125">Error code for the setting</span></span>|
|<span data-ttu-id="e1eb5-126">errorDescription</span><span class="sxs-lookup"><span data-stu-id="e1eb5-126">errorDescription</span></span>|<span data-ttu-id="e1eb5-127">String</span><span class="sxs-lookup"><span data-stu-id="e1eb5-127">String</span></span>|<span data-ttu-id="e1eb5-128">Descrição do erro</span><span class="sxs-lookup"><span data-stu-id="e1eb5-128">Error description</span></span>|
|<span data-ttu-id="e1eb5-129">userId</span><span class="sxs-lookup"><span data-stu-id="e1eb5-129">userId</span></span>|<span data-ttu-id="e1eb5-130">String</span><span class="sxs-lookup"><span data-stu-id="e1eb5-130">String</span></span>|<span data-ttu-id="e1eb5-131">UserId</span><span class="sxs-lookup"><span data-stu-id="e1eb5-131">UserId</span></span>|
|<span data-ttu-id="e1eb5-132">userName</span><span class="sxs-lookup"><span data-stu-id="e1eb5-132">userName</span></span>|<span data-ttu-id="e1eb5-133">String</span><span class="sxs-lookup"><span data-stu-id="e1eb5-133">String</span></span>|<span data-ttu-id="e1eb5-134">UserName</span><span class="sxs-lookup"><span data-stu-id="e1eb5-134">UserName</span></span>|
|<span data-ttu-id="e1eb5-135">userEmail</span><span class="sxs-lookup"><span data-stu-id="e1eb5-135">userEmail</span></span>|<span data-ttu-id="e1eb5-136">String</span><span class="sxs-lookup"><span data-stu-id="e1eb5-136">String</span></span>|<span data-ttu-id="e1eb5-137">UserEmail</span><span class="sxs-lookup"><span data-stu-id="e1eb5-137">UserEmail</span></span>|
|<span data-ttu-id="e1eb5-138">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="e1eb5-138">userPrincipalName</span></span>|<span data-ttu-id="e1eb5-139">String</span><span class="sxs-lookup"><span data-stu-id="e1eb5-139">String</span></span>|<span data-ttu-id="e1eb5-140">UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="e1eb5-140">UserPrincipalName.</span></span>|
|<span data-ttu-id="e1eb5-141">sources</span><span class="sxs-lookup"><span data-stu-id="e1eb5-141">sources</span></span>|<span data-ttu-id="e1eb5-142">Coleção [settingSource](../resources/intune-deviceconfig-settingsource.md)</span><span class="sxs-lookup"><span data-stu-id="e1eb5-142">[settingSource](../resources/intune-deviceconfig-settingsource.md) collection</span></span>|<span data-ttu-id="e1eb5-143">Políticas colaboradoras</span><span class="sxs-lookup"><span data-stu-id="e1eb5-143">Contributing policies</span></span>|
|<span data-ttu-id="e1eb5-144">currentValue</span><span class="sxs-lookup"><span data-stu-id="e1eb5-144">currentValue</span></span>|<span data-ttu-id="e1eb5-145">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e1eb5-145">String</span></span>|<span data-ttu-id="e1eb5-146">Valor atual da configuração no dispositivo</span><span class="sxs-lookup"><span data-stu-id="e1eb5-146">Current value of setting on device</span></span>|

## <a name="relationships"></a><span data-ttu-id="e1eb5-147">Relações</span><span class="sxs-lookup"><span data-stu-id="e1eb5-147">Relationships</span></span>
<span data-ttu-id="e1eb5-148">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e1eb5-148">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e1eb5-149">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e1eb5-149">JSON Representation</span></span>
<span data-ttu-id="e1eb5-150">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e1eb5-150">Here is a JSON representation of the resource.</span></span>
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



