---
title: Tipo de recurso deviceCompliancePolicySettingState
description: Estado da configuração da política de conformidade de dispositivo para um determinado dispositivo.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 05f79a5967ae97eb825d85732f207682d9add645
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36028459"
---
# <a name="devicecompliancepolicysettingstate-resource-type"></a><span data-ttu-id="1fe9f-103">Tipo de recurso deviceCompliancePolicySettingState</span><span class="sxs-lookup"><span data-stu-id="1fe9f-103">deviceCompliancePolicySettingState resource type</span></span>

> <span data-ttu-id="1fe9f-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1fe9f-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1fe9f-105">Estado da configuração da política de conformidade de dispositivo para um determinado dispositivo.</span><span class="sxs-lookup"><span data-stu-id="1fe9f-105">Device Compilance Policy Setting State for a given device.</span></span>

## <a name="properties"></a><span data-ttu-id="1fe9f-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1fe9f-106">Properties</span></span>
|<span data-ttu-id="1fe9f-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1fe9f-107">Property</span></span>|<span data-ttu-id="1fe9f-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="1fe9f-108">Type</span></span>|<span data-ttu-id="1fe9f-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="1fe9f-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1fe9f-110">configuração</span><span class="sxs-lookup"><span data-stu-id="1fe9f-110">setting</span></span>|<span data-ttu-id="1fe9f-111">String</span><span class="sxs-lookup"><span data-stu-id="1fe9f-111">String</span></span>|<span data-ttu-id="1fe9f-112">A configuração que é relatada</span><span class="sxs-lookup"><span data-stu-id="1fe9f-112">The setting that is being reported</span></span>|
|<span data-ttu-id="1fe9f-113">settingName</span><span class="sxs-lookup"><span data-stu-id="1fe9f-113">settingName</span></span>|<span data-ttu-id="1fe9f-114">String</span><span class="sxs-lookup"><span data-stu-id="1fe9f-114">String</span></span>|<span data-ttu-id="1fe9f-115">Nome de configuração localizada/de usuário que é relatada</span><span class="sxs-lookup"><span data-stu-id="1fe9f-115">Localized/user friendly setting name that is being reported</span></span>|
|<span data-ttu-id="1fe9f-116">instanceDisplayName</span><span class="sxs-lookup"><span data-stu-id="1fe9f-116">instanceDisplayName</span></span>|<span data-ttu-id="1fe9f-117">String</span><span class="sxs-lookup"><span data-stu-id="1fe9f-117">String</span></span>|<span data-ttu-id="1fe9f-118">Nome da instância de configuração que é relatada.</span><span class="sxs-lookup"><span data-stu-id="1fe9f-118">Name of setting instance that is being reported.</span></span>|
|<span data-ttu-id="1fe9f-119">state</span><span class="sxs-lookup"><span data-stu-id="1fe9f-119">state</span></span>|[<span data-ttu-id="1fe9f-120">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="1fe9f-120">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="1fe9f-121">O estado de conformidade da configuração.</span><span class="sxs-lookup"><span data-stu-id="1fe9f-121">The compliance state of the setting.</span></span> <span data-ttu-id="1fe9f-122">Os valores possíveis são: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="1fe9f-122">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="1fe9f-123">errorCode</span><span class="sxs-lookup"><span data-stu-id="1fe9f-123">errorCode</span></span>|<span data-ttu-id="1fe9f-124">Int64</span><span class="sxs-lookup"><span data-stu-id="1fe9f-124">Int64</span></span>|<span data-ttu-id="1fe9f-125">Código de erro da configuração</span><span class="sxs-lookup"><span data-stu-id="1fe9f-125">Error code for the setting</span></span>|
|<span data-ttu-id="1fe9f-126">errorDescription</span><span class="sxs-lookup"><span data-stu-id="1fe9f-126">errorDescription</span></span>|<span data-ttu-id="1fe9f-127">String</span><span class="sxs-lookup"><span data-stu-id="1fe9f-127">String</span></span>|<span data-ttu-id="1fe9f-128">Descrição de erro</span><span class="sxs-lookup"><span data-stu-id="1fe9f-128">Error description</span></span>|
|<span data-ttu-id="1fe9f-129">userId</span><span class="sxs-lookup"><span data-stu-id="1fe9f-129">userId</span></span>|<span data-ttu-id="1fe9f-130">String</span><span class="sxs-lookup"><span data-stu-id="1fe9f-130">String</span></span>|<span data-ttu-id="1fe9f-131">UserId</span><span class="sxs-lookup"><span data-stu-id="1fe9f-131">UserId</span></span>|
|<span data-ttu-id="1fe9f-132">userName</span><span class="sxs-lookup"><span data-stu-id="1fe9f-132">userName</span></span>|<span data-ttu-id="1fe9f-133">String</span><span class="sxs-lookup"><span data-stu-id="1fe9f-133">String</span></span>|<span data-ttu-id="1fe9f-134">UserName</span><span class="sxs-lookup"><span data-stu-id="1fe9f-134">UserName</span></span>|
|<span data-ttu-id="1fe9f-135">userEmail</span><span class="sxs-lookup"><span data-stu-id="1fe9f-135">userEmail</span></span>|<span data-ttu-id="1fe9f-136">String</span><span class="sxs-lookup"><span data-stu-id="1fe9f-136">String</span></span>|<span data-ttu-id="1fe9f-137">UserEmail</span><span class="sxs-lookup"><span data-stu-id="1fe9f-137">UserEmail</span></span>|
|<span data-ttu-id="1fe9f-138">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="1fe9f-138">userPrincipalName</span></span>|<span data-ttu-id="1fe9f-139">String</span><span class="sxs-lookup"><span data-stu-id="1fe9f-139">String</span></span>|<span data-ttu-id="1fe9f-140">UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="1fe9f-140">UserPrincipalName.</span></span>|
|<span data-ttu-id="1fe9f-141">fontes</span><span class="sxs-lookup"><span data-stu-id="1fe9f-141">sources</span></span>|<span data-ttu-id="1fe9f-142">Conjunto [settingSource](../resources/intune-deviceconfig-settingsource.md)</span><span class="sxs-lookup"><span data-stu-id="1fe9f-142">[settingSource](../resources/intune-deviceconfig-settingsource.md) collection</span></span>|<span data-ttu-id="1fe9f-143">Políticas de colaboração</span><span class="sxs-lookup"><span data-stu-id="1fe9f-143">Contributing policies</span></span>|
|<span data-ttu-id="1fe9f-144">currentValue</span><span class="sxs-lookup"><span data-stu-id="1fe9f-144">currentValue</span></span>|<span data-ttu-id="1fe9f-145">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1fe9f-145">String</span></span>|<span data-ttu-id="1fe9f-146">Valor atual da configuração em um dispositivo</span><span class="sxs-lookup"><span data-stu-id="1fe9f-146">Current value of setting on device</span></span>|

## <a name="relationships"></a><span data-ttu-id="1fe9f-147">Relações</span><span class="sxs-lookup"><span data-stu-id="1fe9f-147">Relationships</span></span>
<span data-ttu-id="1fe9f-148">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1fe9f-148">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1fe9f-149">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1fe9f-149">JSON Representation</span></span>
<span data-ttu-id="1fe9f-150">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1fe9f-150">Here is a JSON representation of the resource.</span></span>
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



