---
title: Tipo de recurso deviceCompliancePolicySettingState
description: Estado da configuração da política de conformidade de dispositivo para um determinado dispositivo.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: a15aa7494c4580c1b69eebf7499066a153ce7f63
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49260338"
---
# <a name="devicecompliancepolicysettingstate-resource-type"></a><span data-ttu-id="4cfce-103">Tipo de recurso deviceCompliancePolicySettingState</span><span class="sxs-lookup"><span data-stu-id="4cfce-103">deviceCompliancePolicySettingState resource type</span></span>

<span data-ttu-id="4cfce-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4cfce-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4cfce-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="4cfce-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4cfce-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="4cfce-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4cfce-107">Estado da configuração da política de conformidade de dispositivo para um determinado dispositivo.</span><span class="sxs-lookup"><span data-stu-id="4cfce-107">Device Compilance Policy Setting State for a given device.</span></span>

## <a name="properties"></a><span data-ttu-id="4cfce-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4cfce-108">Properties</span></span>
|<span data-ttu-id="4cfce-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4cfce-109">Property</span></span>|<span data-ttu-id="4cfce-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="4cfce-110">Type</span></span>|<span data-ttu-id="4cfce-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="4cfce-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4cfce-112">configuração</span><span class="sxs-lookup"><span data-stu-id="4cfce-112">setting</span></span>|<span data-ttu-id="4cfce-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4cfce-113">String</span></span>|<span data-ttu-id="4cfce-114">A configuração que é relatada</span><span class="sxs-lookup"><span data-stu-id="4cfce-114">The setting that is being reported</span></span>|
|<span data-ttu-id="4cfce-115">settingName</span><span class="sxs-lookup"><span data-stu-id="4cfce-115">settingName</span></span>|<span data-ttu-id="4cfce-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4cfce-116">String</span></span>|<span data-ttu-id="4cfce-117">Nome de configuração localizada/de usuário que é relatada</span><span class="sxs-lookup"><span data-stu-id="4cfce-117">Localized/user friendly setting name that is being reported</span></span>|
|<span data-ttu-id="4cfce-118">instanceDisplayName</span><span class="sxs-lookup"><span data-stu-id="4cfce-118">instanceDisplayName</span></span>|<span data-ttu-id="4cfce-119">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4cfce-119">String</span></span>|<span data-ttu-id="4cfce-120">Nome da instância de configuração que é relatada.</span><span class="sxs-lookup"><span data-stu-id="4cfce-120">Name of setting instance that is being reported.</span></span>|
|<span data-ttu-id="4cfce-121">state</span><span class="sxs-lookup"><span data-stu-id="4cfce-121">state</span></span>|[<span data-ttu-id="4cfce-122">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="4cfce-122">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="4cfce-123">O estado de conformidade da configuração.</span><span class="sxs-lookup"><span data-stu-id="4cfce-123">The compliance state of the setting.</span></span> <span data-ttu-id="4cfce-124">Os valores possíveis são: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="4cfce-124">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="4cfce-125">errorCode</span><span class="sxs-lookup"><span data-stu-id="4cfce-125">errorCode</span></span>|<span data-ttu-id="4cfce-126">Int64</span><span class="sxs-lookup"><span data-stu-id="4cfce-126">Int64</span></span>|<span data-ttu-id="4cfce-127">Código de erro da configuração</span><span class="sxs-lookup"><span data-stu-id="4cfce-127">Error code for the setting</span></span>|
|<span data-ttu-id="4cfce-128">errorDescription</span><span class="sxs-lookup"><span data-stu-id="4cfce-128">errorDescription</span></span>|<span data-ttu-id="4cfce-129">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4cfce-129">String</span></span>|<span data-ttu-id="4cfce-130">Descrição de erro</span><span class="sxs-lookup"><span data-stu-id="4cfce-130">Error description</span></span>|
|<span data-ttu-id="4cfce-131">userId</span><span class="sxs-lookup"><span data-stu-id="4cfce-131">userId</span></span>|<span data-ttu-id="4cfce-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4cfce-132">String</span></span>|<span data-ttu-id="4cfce-133">UserId</span><span class="sxs-lookup"><span data-stu-id="4cfce-133">UserId</span></span>|
|<span data-ttu-id="4cfce-134">userName</span><span class="sxs-lookup"><span data-stu-id="4cfce-134">userName</span></span>|<span data-ttu-id="4cfce-135">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4cfce-135">String</span></span>|<span data-ttu-id="4cfce-136">UserName</span><span class="sxs-lookup"><span data-stu-id="4cfce-136">UserName</span></span>|
|<span data-ttu-id="4cfce-137">userEmail</span><span class="sxs-lookup"><span data-stu-id="4cfce-137">userEmail</span></span>|<span data-ttu-id="4cfce-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4cfce-138">String</span></span>|<span data-ttu-id="4cfce-139">UserEmail</span><span class="sxs-lookup"><span data-stu-id="4cfce-139">UserEmail</span></span>|
|<span data-ttu-id="4cfce-140">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="4cfce-140">userPrincipalName</span></span>|<span data-ttu-id="4cfce-141">String</span><span class="sxs-lookup"><span data-stu-id="4cfce-141">String</span></span>|<span data-ttu-id="4cfce-142">UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="4cfce-142">UserPrincipalName.</span></span>|
|<span data-ttu-id="4cfce-143">fontes</span><span class="sxs-lookup"><span data-stu-id="4cfce-143">sources</span></span>|<span data-ttu-id="4cfce-144">Conjunto [settingSource](../resources/intune-deviceconfig-settingsource.md)</span><span class="sxs-lookup"><span data-stu-id="4cfce-144">[settingSource](../resources/intune-deviceconfig-settingsource.md) collection</span></span>|<span data-ttu-id="4cfce-145">Políticas de colaboração</span><span class="sxs-lookup"><span data-stu-id="4cfce-145">Contributing policies</span></span>|
|<span data-ttu-id="4cfce-146">currentValue</span><span class="sxs-lookup"><span data-stu-id="4cfce-146">currentValue</span></span>|<span data-ttu-id="4cfce-147">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4cfce-147">String</span></span>|<span data-ttu-id="4cfce-148">Valor atual da configuração em um dispositivo</span><span class="sxs-lookup"><span data-stu-id="4cfce-148">Current value of setting on device</span></span>|
|<span data-ttu-id="4cfce-149">settingInstanceId</span><span class="sxs-lookup"><span data-stu-id="4cfce-149">settingInstanceId</span></span>|<span data-ttu-id="4cfce-150">String</span><span class="sxs-lookup"><span data-stu-id="4cfce-150">String</span></span>|<span data-ttu-id="4cfce-151">SettingInstanceId</span><span class="sxs-lookup"><span data-stu-id="4cfce-151">SettingInstanceId</span></span>|

## <a name="relationships"></a><span data-ttu-id="4cfce-152">Relações</span><span class="sxs-lookup"><span data-stu-id="4cfce-152">Relationships</span></span>
<span data-ttu-id="4cfce-153">Nenhum</span><span class="sxs-lookup"><span data-stu-id="4cfce-153">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4cfce-154">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4cfce-154">JSON Representation</span></span>
<span data-ttu-id="4cfce-155">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4cfce-155">Here is a JSON representation of the resource.</span></span>
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




