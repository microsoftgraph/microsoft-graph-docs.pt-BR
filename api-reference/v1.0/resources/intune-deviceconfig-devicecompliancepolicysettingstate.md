---
title: Tipo de recurso deviceCompliancePolicySettingState
description: Estado da configuração da política de conformidade de dispositivo para um determinado dispositivo.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 1d75c82cfdd53d1df51537980487e7f7ed780414
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42530815"
---
# <a name="devicecompliancepolicysettingstate-resource-type"></a><span data-ttu-id="54a27-103">Tipo de recurso deviceCompliancePolicySettingState</span><span class="sxs-lookup"><span data-stu-id="54a27-103">deviceCompliancePolicySettingState resource type</span></span>

<span data-ttu-id="54a27-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="54a27-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="54a27-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="54a27-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="54a27-106">Estado da configuração da política de conformidade de dispositivo para um determinado dispositivo.</span><span class="sxs-lookup"><span data-stu-id="54a27-106">Device Compilance Policy Setting State for a given device.</span></span>

## <a name="properties"></a><span data-ttu-id="54a27-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="54a27-107">Properties</span></span>
|<span data-ttu-id="54a27-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="54a27-108">Property</span></span>|<span data-ttu-id="54a27-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="54a27-109">Type</span></span>|<span data-ttu-id="54a27-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="54a27-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="54a27-111">configuração</span><span class="sxs-lookup"><span data-stu-id="54a27-111">setting</span></span>|<span data-ttu-id="54a27-112">String</span><span class="sxs-lookup"><span data-stu-id="54a27-112">String</span></span>|<span data-ttu-id="54a27-113">A configuração que é relatada</span><span class="sxs-lookup"><span data-stu-id="54a27-113">The setting that is being reported</span></span>|
|<span data-ttu-id="54a27-114">settingName</span><span class="sxs-lookup"><span data-stu-id="54a27-114">settingName</span></span>|<span data-ttu-id="54a27-115">String</span><span class="sxs-lookup"><span data-stu-id="54a27-115">String</span></span>|<span data-ttu-id="54a27-116">Nome de configuração localizada/de usuário que é relatada</span><span class="sxs-lookup"><span data-stu-id="54a27-116">Localized/user friendly setting name that is being reported</span></span>|
|<span data-ttu-id="54a27-117">instanceDisplayName</span><span class="sxs-lookup"><span data-stu-id="54a27-117">instanceDisplayName</span></span>|<span data-ttu-id="54a27-118">String</span><span class="sxs-lookup"><span data-stu-id="54a27-118">String</span></span>|<span data-ttu-id="54a27-119">Nome da instância de configuração que é relatada.</span><span class="sxs-lookup"><span data-stu-id="54a27-119">Name of setting instance that is being reported.</span></span>|
|<span data-ttu-id="54a27-120">state</span><span class="sxs-lookup"><span data-stu-id="54a27-120">state</span></span>|[<span data-ttu-id="54a27-121">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="54a27-121">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="54a27-122">O estado de conformidade da configuração.</span><span class="sxs-lookup"><span data-stu-id="54a27-122">The compliance state of the setting.</span></span> <span data-ttu-id="54a27-123">Os valores possíveis são: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="54a27-123">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="54a27-124">errorCode</span><span class="sxs-lookup"><span data-stu-id="54a27-124">errorCode</span></span>|<span data-ttu-id="54a27-125">Int64</span><span class="sxs-lookup"><span data-stu-id="54a27-125">Int64</span></span>|<span data-ttu-id="54a27-126">Código de erro da configuração</span><span class="sxs-lookup"><span data-stu-id="54a27-126">Error code for the setting</span></span>|
|<span data-ttu-id="54a27-127">errorDescription</span><span class="sxs-lookup"><span data-stu-id="54a27-127">errorDescription</span></span>|<span data-ttu-id="54a27-128">String</span><span class="sxs-lookup"><span data-stu-id="54a27-128">String</span></span>|<span data-ttu-id="54a27-129">Descrição de erro</span><span class="sxs-lookup"><span data-stu-id="54a27-129">Error description</span></span>|
|<span data-ttu-id="54a27-130">userId</span><span class="sxs-lookup"><span data-stu-id="54a27-130">userId</span></span>|<span data-ttu-id="54a27-131">String</span><span class="sxs-lookup"><span data-stu-id="54a27-131">String</span></span>|<span data-ttu-id="54a27-132">UserId</span><span class="sxs-lookup"><span data-stu-id="54a27-132">UserId</span></span>|
|<span data-ttu-id="54a27-133">userName</span><span class="sxs-lookup"><span data-stu-id="54a27-133">userName</span></span>|<span data-ttu-id="54a27-134">String</span><span class="sxs-lookup"><span data-stu-id="54a27-134">String</span></span>|<span data-ttu-id="54a27-135">UserName</span><span class="sxs-lookup"><span data-stu-id="54a27-135">UserName</span></span>|
|<span data-ttu-id="54a27-136">userEmail</span><span class="sxs-lookup"><span data-stu-id="54a27-136">userEmail</span></span>|<span data-ttu-id="54a27-137">String</span><span class="sxs-lookup"><span data-stu-id="54a27-137">String</span></span>|<span data-ttu-id="54a27-138">UserEmail</span><span class="sxs-lookup"><span data-stu-id="54a27-138">UserEmail</span></span>|
|<span data-ttu-id="54a27-139">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="54a27-139">userPrincipalName</span></span>|<span data-ttu-id="54a27-140">String</span><span class="sxs-lookup"><span data-stu-id="54a27-140">String</span></span>|<span data-ttu-id="54a27-141">UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="54a27-141">UserPrincipalName.</span></span>|
|<span data-ttu-id="54a27-142">fontes</span><span class="sxs-lookup"><span data-stu-id="54a27-142">sources</span></span>|<span data-ttu-id="54a27-143">Conjunto [settingSource](../resources/intune-deviceconfig-settingsource.md)</span><span class="sxs-lookup"><span data-stu-id="54a27-143">[settingSource](../resources/intune-deviceconfig-settingsource.md) collection</span></span>|<span data-ttu-id="54a27-144">Políticas de colaboração</span><span class="sxs-lookup"><span data-stu-id="54a27-144">Contributing policies</span></span>|
|<span data-ttu-id="54a27-145">currentValue</span><span class="sxs-lookup"><span data-stu-id="54a27-145">currentValue</span></span>|<span data-ttu-id="54a27-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="54a27-146">String</span></span>|<span data-ttu-id="54a27-147">Valor atual da configuração em um dispositivo</span><span class="sxs-lookup"><span data-stu-id="54a27-147">Current value of setting on device</span></span>|

## <a name="relationships"></a><span data-ttu-id="54a27-148">Relações</span><span class="sxs-lookup"><span data-stu-id="54a27-148">Relationships</span></span>
<span data-ttu-id="54a27-149">Nenhum</span><span class="sxs-lookup"><span data-stu-id="54a27-149">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="54a27-150">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="54a27-150">JSON Representation</span></span>
<span data-ttu-id="54a27-151">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="54a27-151">Here is a JSON representation of the resource.</span></span>
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




