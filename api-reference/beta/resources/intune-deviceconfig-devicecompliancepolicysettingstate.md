---
title: Tipo de recurso deviceCompliancePolicySettingState
description: Estado da configuração da política de conformidade de dispositivo para um determinado dispositivo.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b6c204294190f2f585ad19f7cad4f68e2f7fcc03
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32565818"
---
# <a name="devicecompliancepolicysettingstate-resource-type"></a><span data-ttu-id="310f6-103">Tipo de recurso deviceCompliancePolicySettingState</span><span class="sxs-lookup"><span data-stu-id="310f6-103">deviceCompliancePolicySettingState resource type</span></span>

> <span data-ttu-id="310f6-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="310f6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="310f6-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="310f6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="310f6-106">Estado da configuração da política de conformidade de dispositivo para um determinado dispositivo.</span><span class="sxs-lookup"><span data-stu-id="310f6-106">Device Compilance Policy Setting State for a given device.</span></span>

## <a name="properties"></a><span data-ttu-id="310f6-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="310f6-107">Properties</span></span>
|<span data-ttu-id="310f6-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="310f6-108">Property</span></span>|<span data-ttu-id="310f6-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="310f6-109">Type</span></span>|<span data-ttu-id="310f6-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="310f6-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="310f6-111">configuração</span><span class="sxs-lookup"><span data-stu-id="310f6-111">setting</span></span>|<span data-ttu-id="310f6-112">String</span><span class="sxs-lookup"><span data-stu-id="310f6-112">String</span></span>|<span data-ttu-id="310f6-113">A configuração que é relatada</span><span class="sxs-lookup"><span data-stu-id="310f6-113">The setting that is being reported</span></span>|
|<span data-ttu-id="310f6-114">settingName</span><span class="sxs-lookup"><span data-stu-id="310f6-114">settingName</span></span>|<span data-ttu-id="310f6-115">String</span><span class="sxs-lookup"><span data-stu-id="310f6-115">String</span></span>|<span data-ttu-id="310f6-116">Nome de configuração localizada/de usuário que é relatada</span><span class="sxs-lookup"><span data-stu-id="310f6-116">Localized/user friendly setting name that is being reported</span></span>|
|<span data-ttu-id="310f6-117">instanceDisplayName</span><span class="sxs-lookup"><span data-stu-id="310f6-117">instanceDisplayName</span></span>|<span data-ttu-id="310f6-118">String</span><span class="sxs-lookup"><span data-stu-id="310f6-118">String</span></span>|<span data-ttu-id="310f6-119">Nome da instância de configuração que é relatada.</span><span class="sxs-lookup"><span data-stu-id="310f6-119">Name of setting instance that is being reported.</span></span>|
|<span data-ttu-id="310f6-120">state</span><span class="sxs-lookup"><span data-stu-id="310f6-120">state</span></span>|[<span data-ttu-id="310f6-121">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="310f6-121">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="310f6-122">O estado de conformidade da configuração.</span><span class="sxs-lookup"><span data-stu-id="310f6-122">The compliance state of the setting.</span></span> <span data-ttu-id="310f6-123">Os valores possíveis são: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="310f6-123">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="310f6-124">errorCode</span><span class="sxs-lookup"><span data-stu-id="310f6-124">errorCode</span></span>|<span data-ttu-id="310f6-125">Int64</span><span class="sxs-lookup"><span data-stu-id="310f6-125">Int64</span></span>|<span data-ttu-id="310f6-126">Código de erro da configuração</span><span class="sxs-lookup"><span data-stu-id="310f6-126">Error code for the setting</span></span>|
|<span data-ttu-id="310f6-127">errorDescription</span><span class="sxs-lookup"><span data-stu-id="310f6-127">errorDescription</span></span>|<span data-ttu-id="310f6-128">String</span><span class="sxs-lookup"><span data-stu-id="310f6-128">String</span></span>|<span data-ttu-id="310f6-129">Descrição de erro</span><span class="sxs-lookup"><span data-stu-id="310f6-129">Error description</span></span>|
|<span data-ttu-id="310f6-130">userId</span><span class="sxs-lookup"><span data-stu-id="310f6-130">userId</span></span>|<span data-ttu-id="310f6-131">String</span><span class="sxs-lookup"><span data-stu-id="310f6-131">String</span></span>|<span data-ttu-id="310f6-132">UserId</span><span class="sxs-lookup"><span data-stu-id="310f6-132">UserId</span></span>|
|<span data-ttu-id="310f6-133">userName</span><span class="sxs-lookup"><span data-stu-id="310f6-133">userName</span></span>|<span data-ttu-id="310f6-134">String</span><span class="sxs-lookup"><span data-stu-id="310f6-134">String</span></span>|<span data-ttu-id="310f6-135">UserName</span><span class="sxs-lookup"><span data-stu-id="310f6-135">UserName</span></span>|
|<span data-ttu-id="310f6-136">userEmail</span><span class="sxs-lookup"><span data-stu-id="310f6-136">userEmail</span></span>|<span data-ttu-id="310f6-137">String</span><span class="sxs-lookup"><span data-stu-id="310f6-137">String</span></span>|<span data-ttu-id="310f6-138">UserEmail</span><span class="sxs-lookup"><span data-stu-id="310f6-138">UserEmail</span></span>|
|<span data-ttu-id="310f6-139">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="310f6-139">userPrincipalName</span></span>|<span data-ttu-id="310f6-140">String</span><span class="sxs-lookup"><span data-stu-id="310f6-140">String</span></span>|<span data-ttu-id="310f6-141">UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="310f6-141">UserPrincipalName.</span></span>|
|<span data-ttu-id="310f6-142">fontes</span><span class="sxs-lookup"><span data-stu-id="310f6-142">sources</span></span>|<span data-ttu-id="310f6-143">Conjunto [settingSource](../resources/intune-deviceconfig-settingsource.md)</span><span class="sxs-lookup"><span data-stu-id="310f6-143">[settingSource](../resources/intune-deviceconfig-settingsource.md) collection</span></span>|<span data-ttu-id="310f6-144">Políticas de colaboração</span><span class="sxs-lookup"><span data-stu-id="310f6-144">Contributing policies</span></span>|
|<span data-ttu-id="310f6-145">currentValue</span><span class="sxs-lookup"><span data-stu-id="310f6-145">currentValue</span></span>|<span data-ttu-id="310f6-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="310f6-146">String</span></span>|<span data-ttu-id="310f6-147">Valor atual da configuração em um dispositivo</span><span class="sxs-lookup"><span data-stu-id="310f6-147">Current value of setting on device</span></span>|

## <a name="relationships"></a><span data-ttu-id="310f6-148">Relações</span><span class="sxs-lookup"><span data-stu-id="310f6-148">Relationships</span></span>
<span data-ttu-id="310f6-149">Nenhum</span><span class="sxs-lookup"><span data-stu-id="310f6-149">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="310f6-150">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="310f6-150">JSON Representation</span></span>
<span data-ttu-id="310f6-151">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="310f6-151">Here is a JSON representation of the resource.</span></span>
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





