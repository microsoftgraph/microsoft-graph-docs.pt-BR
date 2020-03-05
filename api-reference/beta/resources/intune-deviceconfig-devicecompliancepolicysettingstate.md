---
title: Tipo de recurso deviceCompliancePolicySettingState
description: Estado da configuração da política de conformidade de dispositivo para um determinado dispositivo.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: f2700f348c8d2f1915e7cfd14221951894eb68f6
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42526684"
---
# <a name="devicecompliancepolicysettingstate-resource-type"></a><span data-ttu-id="b9375-103">Tipo de recurso deviceCompliancePolicySettingState</span><span class="sxs-lookup"><span data-stu-id="b9375-103">deviceCompliancePolicySettingState resource type</span></span>

<span data-ttu-id="b9375-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="b9375-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b9375-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b9375-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b9375-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b9375-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b9375-107">Estado da configuração da política de conformidade de dispositivo para um determinado dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b9375-107">Device Compilance Policy Setting State for a given device.</span></span>

## <a name="properties"></a><span data-ttu-id="b9375-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b9375-108">Properties</span></span>
|<span data-ttu-id="b9375-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b9375-109">Property</span></span>|<span data-ttu-id="b9375-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="b9375-110">Type</span></span>|<span data-ttu-id="b9375-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="b9375-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b9375-112">configuração</span><span class="sxs-lookup"><span data-stu-id="b9375-112">setting</span></span>|<span data-ttu-id="b9375-113">String</span><span class="sxs-lookup"><span data-stu-id="b9375-113">String</span></span>|<span data-ttu-id="b9375-114">A configuração que é relatada</span><span class="sxs-lookup"><span data-stu-id="b9375-114">The setting that is being reported</span></span>|
|<span data-ttu-id="b9375-115">settingName</span><span class="sxs-lookup"><span data-stu-id="b9375-115">settingName</span></span>|<span data-ttu-id="b9375-116">String</span><span class="sxs-lookup"><span data-stu-id="b9375-116">String</span></span>|<span data-ttu-id="b9375-117">Nome de configuração localizada/de usuário que é relatada</span><span class="sxs-lookup"><span data-stu-id="b9375-117">Localized/user friendly setting name that is being reported</span></span>|
|<span data-ttu-id="b9375-118">instanceDisplayName</span><span class="sxs-lookup"><span data-stu-id="b9375-118">instanceDisplayName</span></span>|<span data-ttu-id="b9375-119">String</span><span class="sxs-lookup"><span data-stu-id="b9375-119">String</span></span>|<span data-ttu-id="b9375-120">Nome da instância de configuração que é relatada.</span><span class="sxs-lookup"><span data-stu-id="b9375-120">Name of setting instance that is being reported.</span></span>|
|<span data-ttu-id="b9375-121">state</span><span class="sxs-lookup"><span data-stu-id="b9375-121">state</span></span>|[<span data-ttu-id="b9375-122">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="b9375-122">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="b9375-123">O estado de conformidade da configuração.</span><span class="sxs-lookup"><span data-stu-id="b9375-123">The compliance state of the setting.</span></span> <span data-ttu-id="b9375-124">Os valores possíveis são: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="b9375-124">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="b9375-125">errorCode</span><span class="sxs-lookup"><span data-stu-id="b9375-125">errorCode</span></span>|<span data-ttu-id="b9375-126">Int64</span><span class="sxs-lookup"><span data-stu-id="b9375-126">Int64</span></span>|<span data-ttu-id="b9375-127">Código de erro da configuração</span><span class="sxs-lookup"><span data-stu-id="b9375-127">Error code for the setting</span></span>|
|<span data-ttu-id="b9375-128">errorDescription</span><span class="sxs-lookup"><span data-stu-id="b9375-128">errorDescription</span></span>|<span data-ttu-id="b9375-129">String</span><span class="sxs-lookup"><span data-stu-id="b9375-129">String</span></span>|<span data-ttu-id="b9375-130">Descrição de erro</span><span class="sxs-lookup"><span data-stu-id="b9375-130">Error description</span></span>|
|<span data-ttu-id="b9375-131">userId</span><span class="sxs-lookup"><span data-stu-id="b9375-131">userId</span></span>|<span data-ttu-id="b9375-132">String</span><span class="sxs-lookup"><span data-stu-id="b9375-132">String</span></span>|<span data-ttu-id="b9375-133">UserId</span><span class="sxs-lookup"><span data-stu-id="b9375-133">UserId</span></span>|
|<span data-ttu-id="b9375-134">userName</span><span class="sxs-lookup"><span data-stu-id="b9375-134">userName</span></span>|<span data-ttu-id="b9375-135">String</span><span class="sxs-lookup"><span data-stu-id="b9375-135">String</span></span>|<span data-ttu-id="b9375-136">UserName</span><span class="sxs-lookup"><span data-stu-id="b9375-136">UserName</span></span>|
|<span data-ttu-id="b9375-137">userEmail</span><span class="sxs-lookup"><span data-stu-id="b9375-137">userEmail</span></span>|<span data-ttu-id="b9375-138">String</span><span class="sxs-lookup"><span data-stu-id="b9375-138">String</span></span>|<span data-ttu-id="b9375-139">UserEmail</span><span class="sxs-lookup"><span data-stu-id="b9375-139">UserEmail</span></span>|
|<span data-ttu-id="b9375-140">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="b9375-140">userPrincipalName</span></span>|<span data-ttu-id="b9375-141">String</span><span class="sxs-lookup"><span data-stu-id="b9375-141">String</span></span>|<span data-ttu-id="b9375-142">UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="b9375-142">UserPrincipalName.</span></span>|
|<span data-ttu-id="b9375-143">fontes</span><span class="sxs-lookup"><span data-stu-id="b9375-143">sources</span></span>|<span data-ttu-id="b9375-144">Conjunto [settingSource](../resources/intune-deviceconfig-settingsource.md)</span><span class="sxs-lookup"><span data-stu-id="b9375-144">[settingSource](../resources/intune-deviceconfig-settingsource.md) collection</span></span>|<span data-ttu-id="b9375-145">Políticas de colaboração</span><span class="sxs-lookup"><span data-stu-id="b9375-145">Contributing policies</span></span>|
|<span data-ttu-id="b9375-146">currentValue</span><span class="sxs-lookup"><span data-stu-id="b9375-146">currentValue</span></span>|<span data-ttu-id="b9375-147">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b9375-147">String</span></span>|<span data-ttu-id="b9375-148">Valor atual da configuração em um dispositivo</span><span class="sxs-lookup"><span data-stu-id="b9375-148">Current value of setting on device</span></span>|

## <a name="relationships"></a><span data-ttu-id="b9375-149">Relações</span><span class="sxs-lookup"><span data-stu-id="b9375-149">Relationships</span></span>
<span data-ttu-id="b9375-150">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b9375-150">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b9375-151">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b9375-151">JSON Representation</span></span>
<span data-ttu-id="b9375-152">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b9375-152">Here is a JSON representation of the resource.</span></span>
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



