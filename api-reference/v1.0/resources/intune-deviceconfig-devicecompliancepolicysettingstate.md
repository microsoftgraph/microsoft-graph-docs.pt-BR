---
title: Tipo de recurso deviceCompliancePolicySettingState
description: Estado da configuração da política de conformidade de dispositivo para um determinado dispositivo.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c4d291f84a8c4404ff5b4425680260997b6b452f
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32572413"
---
# <a name="devicecompliancepolicysettingstate-resource-type"></a><span data-ttu-id="a8b71-103">Tipo de recurso deviceCompliancePolicySettingState</span><span class="sxs-lookup"><span data-stu-id="a8b71-103">deviceCompliancePolicySettingState resource type</span></span>

> <span data-ttu-id="a8b71-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a8b71-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a8b71-105">Estado da configuração da política de conformidade de dispositivo para um determinado dispositivo.</span><span class="sxs-lookup"><span data-stu-id="a8b71-105">Device Compilance Policy Setting State for a given device.</span></span>

## <a name="properties"></a><span data-ttu-id="a8b71-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a8b71-106">Properties</span></span>
|<span data-ttu-id="a8b71-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a8b71-107">Property</span></span>|<span data-ttu-id="a8b71-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="a8b71-108">Type</span></span>|<span data-ttu-id="a8b71-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="a8b71-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a8b71-110">configuração</span><span class="sxs-lookup"><span data-stu-id="a8b71-110">setting</span></span>|<span data-ttu-id="a8b71-111">String</span><span class="sxs-lookup"><span data-stu-id="a8b71-111">String</span></span>|<span data-ttu-id="a8b71-112">A configuração que é relatada</span><span class="sxs-lookup"><span data-stu-id="a8b71-112">The setting that is being reported</span></span>|
|<span data-ttu-id="a8b71-113">settingName</span><span class="sxs-lookup"><span data-stu-id="a8b71-113">settingName</span></span>|<span data-ttu-id="a8b71-114">String</span><span class="sxs-lookup"><span data-stu-id="a8b71-114">String</span></span>|<span data-ttu-id="a8b71-115">Nome de configuração localizada/de usuário que é relatada</span><span class="sxs-lookup"><span data-stu-id="a8b71-115">Localized/user friendly setting name that is being reported</span></span>|
|<span data-ttu-id="a8b71-116">instanceDisplayName</span><span class="sxs-lookup"><span data-stu-id="a8b71-116">instanceDisplayName</span></span>|<span data-ttu-id="a8b71-117">String</span><span class="sxs-lookup"><span data-stu-id="a8b71-117">String</span></span>|<span data-ttu-id="a8b71-118">Nome da instância de configuração que é relatada.</span><span class="sxs-lookup"><span data-stu-id="a8b71-118">Name of setting instance that is being reported.</span></span>|
|<span data-ttu-id="a8b71-119">state</span><span class="sxs-lookup"><span data-stu-id="a8b71-119">state</span></span>|[<span data-ttu-id="a8b71-120">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="a8b71-120">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="a8b71-121">O estado de conformidade da configuração.</span><span class="sxs-lookup"><span data-stu-id="a8b71-121">The compliance state of the setting.</span></span> <span data-ttu-id="a8b71-122">Os valores possíveis são: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="a8b71-122">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="a8b71-123">errorCode</span><span class="sxs-lookup"><span data-stu-id="a8b71-123">errorCode</span></span>|<span data-ttu-id="a8b71-124">Int64</span><span class="sxs-lookup"><span data-stu-id="a8b71-124">Int64</span></span>|<span data-ttu-id="a8b71-125">Código de erro da configuração</span><span class="sxs-lookup"><span data-stu-id="a8b71-125">Error code for the setting</span></span>|
|<span data-ttu-id="a8b71-126">errorDescription</span><span class="sxs-lookup"><span data-stu-id="a8b71-126">errorDescription</span></span>|<span data-ttu-id="a8b71-127">String</span><span class="sxs-lookup"><span data-stu-id="a8b71-127">String</span></span>|<span data-ttu-id="a8b71-128">Descrição de erro</span><span class="sxs-lookup"><span data-stu-id="a8b71-128">Error description</span></span>|
|<span data-ttu-id="a8b71-129">userId</span><span class="sxs-lookup"><span data-stu-id="a8b71-129">userId</span></span>|<span data-ttu-id="a8b71-130">String</span><span class="sxs-lookup"><span data-stu-id="a8b71-130">String</span></span>|<span data-ttu-id="a8b71-131">UserId</span><span class="sxs-lookup"><span data-stu-id="a8b71-131">UserId</span></span>|
|<span data-ttu-id="a8b71-132">userName</span><span class="sxs-lookup"><span data-stu-id="a8b71-132">userName</span></span>|<span data-ttu-id="a8b71-133">String</span><span class="sxs-lookup"><span data-stu-id="a8b71-133">String</span></span>|<span data-ttu-id="a8b71-134">UserName</span><span class="sxs-lookup"><span data-stu-id="a8b71-134">UserName</span></span>|
|<span data-ttu-id="a8b71-135">userEmail</span><span class="sxs-lookup"><span data-stu-id="a8b71-135">userEmail</span></span>|<span data-ttu-id="a8b71-136">String</span><span class="sxs-lookup"><span data-stu-id="a8b71-136">String</span></span>|<span data-ttu-id="a8b71-137">UserEmail</span><span class="sxs-lookup"><span data-stu-id="a8b71-137">UserEmail</span></span>|
|<span data-ttu-id="a8b71-138">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="a8b71-138">userPrincipalName</span></span>|<span data-ttu-id="a8b71-139">String</span><span class="sxs-lookup"><span data-stu-id="a8b71-139">String</span></span>|<span data-ttu-id="a8b71-140">UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="a8b71-140">UserPrincipalName.</span></span>|
|<span data-ttu-id="a8b71-141">fontes</span><span class="sxs-lookup"><span data-stu-id="a8b71-141">sources</span></span>|<span data-ttu-id="a8b71-142">Conjunto [settingSource](../resources/intune-deviceconfig-settingsource.md)</span><span class="sxs-lookup"><span data-stu-id="a8b71-142">[settingSource](../resources/intune-deviceconfig-settingsource.md) collection</span></span>|<span data-ttu-id="a8b71-143">Políticas de colaboração</span><span class="sxs-lookup"><span data-stu-id="a8b71-143">Contributing policies</span></span>|
|<span data-ttu-id="a8b71-144">currentValue</span><span class="sxs-lookup"><span data-stu-id="a8b71-144">currentValue</span></span>|<span data-ttu-id="a8b71-145">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a8b71-145">String</span></span>|<span data-ttu-id="a8b71-146">Valor atual da configuração em um dispositivo</span><span class="sxs-lookup"><span data-stu-id="a8b71-146">Current value of setting on device</span></span>|

## <a name="relationships"></a><span data-ttu-id="a8b71-147">Relações</span><span class="sxs-lookup"><span data-stu-id="a8b71-147">Relationships</span></span>
<span data-ttu-id="a8b71-148">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a8b71-148">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a8b71-149">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a8b71-149">JSON Representation</span></span>
<span data-ttu-id="a8b71-150">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a8b71-150">Here is a JSON representation of the resource.</span></span>
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



