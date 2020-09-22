---
title: Tipo de recurso deviceCompliancePolicySettingState
description: Estado da configuração da política de conformidade de dispositivo para um determinado dispositivo.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 1d2b4a1dafaca68c39864f825c872f1bcf5ab50e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47989301"
---
# <a name="devicecompliancepolicysettingstate-resource-type"></a><span data-ttu-id="2e7d9-103">Tipo de recurso deviceCompliancePolicySettingState</span><span class="sxs-lookup"><span data-stu-id="2e7d9-103">deviceCompliancePolicySettingState resource type</span></span>

<span data-ttu-id="2e7d9-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2e7d9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2e7d9-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="2e7d9-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2e7d9-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2e7d9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2e7d9-107">Estado da configuração da política de conformidade de dispositivo para um determinado dispositivo.</span><span class="sxs-lookup"><span data-stu-id="2e7d9-107">Device Compilance Policy Setting State for a given device.</span></span>

## <a name="properties"></a><span data-ttu-id="2e7d9-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2e7d9-108">Properties</span></span>
|<span data-ttu-id="2e7d9-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2e7d9-109">Property</span></span>|<span data-ttu-id="2e7d9-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="2e7d9-110">Type</span></span>|<span data-ttu-id="2e7d9-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="2e7d9-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2e7d9-112">configuração</span><span class="sxs-lookup"><span data-stu-id="2e7d9-112">setting</span></span>|<span data-ttu-id="2e7d9-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2e7d9-113">String</span></span>|<span data-ttu-id="2e7d9-114">A configuração que é relatada</span><span class="sxs-lookup"><span data-stu-id="2e7d9-114">The setting that is being reported</span></span>|
|<span data-ttu-id="2e7d9-115">settingName</span><span class="sxs-lookup"><span data-stu-id="2e7d9-115">settingName</span></span>|<span data-ttu-id="2e7d9-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2e7d9-116">String</span></span>|<span data-ttu-id="2e7d9-117">Nome de configuração localizada/de usuário que é relatada</span><span class="sxs-lookup"><span data-stu-id="2e7d9-117">Localized/user friendly setting name that is being reported</span></span>|
|<span data-ttu-id="2e7d9-118">instanceDisplayName</span><span class="sxs-lookup"><span data-stu-id="2e7d9-118">instanceDisplayName</span></span>|<span data-ttu-id="2e7d9-119">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2e7d9-119">String</span></span>|<span data-ttu-id="2e7d9-120">Nome da instância de configuração que é relatada.</span><span class="sxs-lookup"><span data-stu-id="2e7d9-120">Name of setting instance that is being reported.</span></span>|
|<span data-ttu-id="2e7d9-121">state</span><span class="sxs-lookup"><span data-stu-id="2e7d9-121">state</span></span>|[<span data-ttu-id="2e7d9-122">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="2e7d9-122">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="2e7d9-123">O estado de conformidade da configuração.</span><span class="sxs-lookup"><span data-stu-id="2e7d9-123">The compliance state of the setting.</span></span> <span data-ttu-id="2e7d9-124">Os valores possíveis são: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="2e7d9-124">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="2e7d9-125">errorCode</span><span class="sxs-lookup"><span data-stu-id="2e7d9-125">errorCode</span></span>|<span data-ttu-id="2e7d9-126">Int64</span><span class="sxs-lookup"><span data-stu-id="2e7d9-126">Int64</span></span>|<span data-ttu-id="2e7d9-127">Código de erro da configuração</span><span class="sxs-lookup"><span data-stu-id="2e7d9-127">Error code for the setting</span></span>|
|<span data-ttu-id="2e7d9-128">errorDescription</span><span class="sxs-lookup"><span data-stu-id="2e7d9-128">errorDescription</span></span>|<span data-ttu-id="2e7d9-129">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2e7d9-129">String</span></span>|<span data-ttu-id="2e7d9-130">Descrição de erro</span><span class="sxs-lookup"><span data-stu-id="2e7d9-130">Error description</span></span>|
|<span data-ttu-id="2e7d9-131">userId</span><span class="sxs-lookup"><span data-stu-id="2e7d9-131">userId</span></span>|<span data-ttu-id="2e7d9-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2e7d9-132">String</span></span>|<span data-ttu-id="2e7d9-133">UserId</span><span class="sxs-lookup"><span data-stu-id="2e7d9-133">UserId</span></span>|
|<span data-ttu-id="2e7d9-134">userName</span><span class="sxs-lookup"><span data-stu-id="2e7d9-134">userName</span></span>|<span data-ttu-id="2e7d9-135">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2e7d9-135">String</span></span>|<span data-ttu-id="2e7d9-136">UserName</span><span class="sxs-lookup"><span data-stu-id="2e7d9-136">UserName</span></span>|
|<span data-ttu-id="2e7d9-137">userEmail</span><span class="sxs-lookup"><span data-stu-id="2e7d9-137">userEmail</span></span>|<span data-ttu-id="2e7d9-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2e7d9-138">String</span></span>|<span data-ttu-id="2e7d9-139">UserEmail</span><span class="sxs-lookup"><span data-stu-id="2e7d9-139">UserEmail</span></span>|
|<span data-ttu-id="2e7d9-140">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="2e7d9-140">userPrincipalName</span></span>|<span data-ttu-id="2e7d9-141">String</span><span class="sxs-lookup"><span data-stu-id="2e7d9-141">String</span></span>|<span data-ttu-id="2e7d9-142">UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="2e7d9-142">UserPrincipalName.</span></span>|
|<span data-ttu-id="2e7d9-143">fontes</span><span class="sxs-lookup"><span data-stu-id="2e7d9-143">sources</span></span>|<span data-ttu-id="2e7d9-144">Conjunto [settingSource](../resources/intune-deviceconfig-settingsource.md)</span><span class="sxs-lookup"><span data-stu-id="2e7d9-144">[settingSource](../resources/intune-deviceconfig-settingsource.md) collection</span></span>|<span data-ttu-id="2e7d9-145">Políticas de colaboração</span><span class="sxs-lookup"><span data-stu-id="2e7d9-145">Contributing policies</span></span>|
|<span data-ttu-id="2e7d9-146">currentValue</span><span class="sxs-lookup"><span data-stu-id="2e7d9-146">currentValue</span></span>|<span data-ttu-id="2e7d9-147">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2e7d9-147">String</span></span>|<span data-ttu-id="2e7d9-148">Valor atual da configuração em um dispositivo</span><span class="sxs-lookup"><span data-stu-id="2e7d9-148">Current value of setting on device</span></span>|
|<span data-ttu-id="2e7d9-149">settingInstanceId</span><span class="sxs-lookup"><span data-stu-id="2e7d9-149">settingInstanceId</span></span>|<span data-ttu-id="2e7d9-150">String</span><span class="sxs-lookup"><span data-stu-id="2e7d9-150">String</span></span>|<span data-ttu-id="2e7d9-151">SettingInstanceId</span><span class="sxs-lookup"><span data-stu-id="2e7d9-151">SettingInstanceId</span></span>|

## <a name="relationships"></a><span data-ttu-id="2e7d9-152">Relações</span><span class="sxs-lookup"><span data-stu-id="2e7d9-152">Relationships</span></span>
<span data-ttu-id="2e7d9-153">Nenhum</span><span class="sxs-lookup"><span data-stu-id="2e7d9-153">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2e7d9-154">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2e7d9-154">JSON Representation</span></span>
<span data-ttu-id="2e7d9-155">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2e7d9-155">Here is a JSON representation of the resource.</span></span>
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
  "currentValue": "String",
  "settingInstanceId": "String"
}
```






