---
title: Tipo de recurso deviceCompliancePolicySettingState
description: Estado da configuração da política de conformidade de dispositivo para um determinado dispositivo.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: b5f0d171854bbd0b7bd67effdb04438e44e0f14b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35970532"
---
# <a name="devicecompliancepolicysettingstate-resource-type"></a><span data-ttu-id="20cd9-103">Tipo de recurso deviceCompliancePolicySettingState</span><span class="sxs-lookup"><span data-stu-id="20cd9-103">deviceCompliancePolicySettingState resource type</span></span>

> <span data-ttu-id="20cd9-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="20cd9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="20cd9-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="20cd9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="20cd9-106">Estado da configuração da política de conformidade de dispositivo para um determinado dispositivo.</span><span class="sxs-lookup"><span data-stu-id="20cd9-106">Device Compilance Policy Setting State for a given device.</span></span>

## <a name="properties"></a><span data-ttu-id="20cd9-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="20cd9-107">Properties</span></span>
|<span data-ttu-id="20cd9-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="20cd9-108">Property</span></span>|<span data-ttu-id="20cd9-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="20cd9-109">Type</span></span>|<span data-ttu-id="20cd9-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="20cd9-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="20cd9-111">configuração</span><span class="sxs-lookup"><span data-stu-id="20cd9-111">setting</span></span>|<span data-ttu-id="20cd9-112">String</span><span class="sxs-lookup"><span data-stu-id="20cd9-112">String</span></span>|<span data-ttu-id="20cd9-113">A configuração que é relatada</span><span class="sxs-lookup"><span data-stu-id="20cd9-113">The setting that is being reported</span></span>|
|<span data-ttu-id="20cd9-114">settingName</span><span class="sxs-lookup"><span data-stu-id="20cd9-114">settingName</span></span>|<span data-ttu-id="20cd9-115">String</span><span class="sxs-lookup"><span data-stu-id="20cd9-115">String</span></span>|<span data-ttu-id="20cd9-116">Nome de configuração localizada/de usuário que é relatada</span><span class="sxs-lookup"><span data-stu-id="20cd9-116">Localized/user friendly setting name that is being reported</span></span>|
|<span data-ttu-id="20cd9-117">instanceDisplayName</span><span class="sxs-lookup"><span data-stu-id="20cd9-117">instanceDisplayName</span></span>|<span data-ttu-id="20cd9-118">String</span><span class="sxs-lookup"><span data-stu-id="20cd9-118">String</span></span>|<span data-ttu-id="20cd9-119">Nome da instância de configuração que é relatada.</span><span class="sxs-lookup"><span data-stu-id="20cd9-119">Name of setting instance that is being reported.</span></span>|
|<span data-ttu-id="20cd9-120">state</span><span class="sxs-lookup"><span data-stu-id="20cd9-120">state</span></span>|[<span data-ttu-id="20cd9-121">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="20cd9-121">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="20cd9-122">O estado de conformidade da configuração.</span><span class="sxs-lookup"><span data-stu-id="20cd9-122">The compliance state of the setting.</span></span> <span data-ttu-id="20cd9-123">Os valores possíveis são: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="20cd9-123">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="20cd9-124">errorCode</span><span class="sxs-lookup"><span data-stu-id="20cd9-124">errorCode</span></span>|<span data-ttu-id="20cd9-125">Int64</span><span class="sxs-lookup"><span data-stu-id="20cd9-125">Int64</span></span>|<span data-ttu-id="20cd9-126">Código de erro da configuração</span><span class="sxs-lookup"><span data-stu-id="20cd9-126">Error code for the setting</span></span>|
|<span data-ttu-id="20cd9-127">errorDescription</span><span class="sxs-lookup"><span data-stu-id="20cd9-127">errorDescription</span></span>|<span data-ttu-id="20cd9-128">String</span><span class="sxs-lookup"><span data-stu-id="20cd9-128">String</span></span>|<span data-ttu-id="20cd9-129">Descrição de erro</span><span class="sxs-lookup"><span data-stu-id="20cd9-129">Error description</span></span>|
|<span data-ttu-id="20cd9-130">userId</span><span class="sxs-lookup"><span data-stu-id="20cd9-130">userId</span></span>|<span data-ttu-id="20cd9-131">String</span><span class="sxs-lookup"><span data-stu-id="20cd9-131">String</span></span>|<span data-ttu-id="20cd9-132">UserId</span><span class="sxs-lookup"><span data-stu-id="20cd9-132">UserId</span></span>|
|<span data-ttu-id="20cd9-133">userName</span><span class="sxs-lookup"><span data-stu-id="20cd9-133">userName</span></span>|<span data-ttu-id="20cd9-134">String</span><span class="sxs-lookup"><span data-stu-id="20cd9-134">String</span></span>|<span data-ttu-id="20cd9-135">UserName</span><span class="sxs-lookup"><span data-stu-id="20cd9-135">UserName</span></span>|
|<span data-ttu-id="20cd9-136">userEmail</span><span class="sxs-lookup"><span data-stu-id="20cd9-136">userEmail</span></span>|<span data-ttu-id="20cd9-137">String</span><span class="sxs-lookup"><span data-stu-id="20cd9-137">String</span></span>|<span data-ttu-id="20cd9-138">UserEmail</span><span class="sxs-lookup"><span data-stu-id="20cd9-138">UserEmail</span></span>|
|<span data-ttu-id="20cd9-139">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="20cd9-139">userPrincipalName</span></span>|<span data-ttu-id="20cd9-140">String</span><span class="sxs-lookup"><span data-stu-id="20cd9-140">String</span></span>|<span data-ttu-id="20cd9-141">UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="20cd9-141">UserPrincipalName.</span></span>|
|<span data-ttu-id="20cd9-142">fontes</span><span class="sxs-lookup"><span data-stu-id="20cd9-142">sources</span></span>|<span data-ttu-id="20cd9-143">Conjunto [settingSource](../resources/intune-deviceconfig-settingsource.md)</span><span class="sxs-lookup"><span data-stu-id="20cd9-143">[settingSource](../resources/intune-deviceconfig-settingsource.md) collection</span></span>|<span data-ttu-id="20cd9-144">Políticas de colaboração</span><span class="sxs-lookup"><span data-stu-id="20cd9-144">Contributing policies</span></span>|
|<span data-ttu-id="20cd9-145">currentValue</span><span class="sxs-lookup"><span data-stu-id="20cd9-145">currentValue</span></span>|<span data-ttu-id="20cd9-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="20cd9-146">String</span></span>|<span data-ttu-id="20cd9-147">Valor atual da configuração em um dispositivo</span><span class="sxs-lookup"><span data-stu-id="20cd9-147">Current value of setting on device</span></span>|

## <a name="relationships"></a><span data-ttu-id="20cd9-148">Relações</span><span class="sxs-lookup"><span data-stu-id="20cd9-148">Relationships</span></span>
<span data-ttu-id="20cd9-149">Nenhum</span><span class="sxs-lookup"><span data-stu-id="20cd9-149">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="20cd9-150">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="20cd9-150">JSON Representation</span></span>
<span data-ttu-id="20cd9-151">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="20cd9-151">Here is a JSON representation of the resource.</span></span>
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





