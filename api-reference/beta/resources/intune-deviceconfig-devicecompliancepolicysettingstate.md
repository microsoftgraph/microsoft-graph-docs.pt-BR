---
title: Tipo de recurso deviceCompliancePolicySettingState
description: Estado da configuração da política de conformidade de dispositivo para um determinado dispositivo.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 8c508f7b936f4a04d929fe429b46ec679d7110eb
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27822782"
---
# <a name="devicecompliancepolicysettingstate-resource-type"></a><span data-ttu-id="5810c-103">Tipo de recurso deviceCompliancePolicySettingState</span><span class="sxs-lookup"><span data-stu-id="5810c-103">deviceCompliancePolicySettingState resource type</span></span>

> <span data-ttu-id="5810c-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="5810c-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5810c-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="5810c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5810c-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="5810c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5810c-107">Estado da configuração da política de conformidade de dispositivo para um determinado dispositivo.</span><span class="sxs-lookup"><span data-stu-id="5810c-107">Device Compilance Policy Setting State for a given device.</span></span>
## <a name="properties"></a><span data-ttu-id="5810c-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5810c-108">Properties</span></span>
|<span data-ttu-id="5810c-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5810c-109">Property</span></span>|<span data-ttu-id="5810c-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="5810c-110">Type</span></span>|<span data-ttu-id="5810c-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="5810c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5810c-112">configuração</span><span class="sxs-lookup"><span data-stu-id="5810c-112">setting</span></span>|<span data-ttu-id="5810c-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5810c-113">String</span></span>|<span data-ttu-id="5810c-114">A configuração que está sendo relatada</span><span class="sxs-lookup"><span data-stu-id="5810c-114">The setting that is being reported</span></span>|
|<span data-ttu-id="5810c-115">settingName</span><span class="sxs-lookup"><span data-stu-id="5810c-115">settingName</span></span>|<span data-ttu-id="5810c-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5810c-116">String</span></span>|<span data-ttu-id="5810c-117">Nome traduzido/amigável para o usuário da configuração que está sendo relatada</span><span class="sxs-lookup"><span data-stu-id="5810c-117">Localized/user friendly setting name that is being reported</span></span>|
|<span data-ttu-id="5810c-118">instanceDisplayName</span><span class="sxs-lookup"><span data-stu-id="5810c-118">instanceDisplayName</span></span>|<span data-ttu-id="5810c-119">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5810c-119">String</span></span>|<span data-ttu-id="5810c-120">Nome da instância de configuração está sendo relatada.</span><span class="sxs-lookup"><span data-stu-id="5810c-120">Name of setting instance that is being reported.</span></span>|
|<span data-ttu-id="5810c-121">estado</span><span class="sxs-lookup"><span data-stu-id="5810c-121">state</span></span>|[<span data-ttu-id="5810c-122">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="5810c-122">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="5810c-123">O estado de conformidade da configuração.</span><span class="sxs-lookup"><span data-stu-id="5810c-123">The compliance state of the setting.</span></span> <span data-ttu-id="5810c-124">Os valores possíveis são: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="5810c-124">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="5810c-125">errorCode</span><span class="sxs-lookup"><span data-stu-id="5810c-125">errorCode</span></span>|<span data-ttu-id="5810c-126">Int64</span><span class="sxs-lookup"><span data-stu-id="5810c-126">Int64</span></span>|<span data-ttu-id="5810c-127">Código de erro da configuração</span><span class="sxs-lookup"><span data-stu-id="5810c-127">Error code for the setting</span></span>|
|<span data-ttu-id="5810c-128">errorDescription</span><span class="sxs-lookup"><span data-stu-id="5810c-128">errorDescription</span></span>|<span data-ttu-id="5810c-129">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5810c-129">String</span></span>|<span data-ttu-id="5810c-130">Descrição do erro</span><span class="sxs-lookup"><span data-stu-id="5810c-130">Error description</span></span>|
|<span data-ttu-id="5810c-131">userId</span><span class="sxs-lookup"><span data-stu-id="5810c-131">userId</span></span>|<span data-ttu-id="5810c-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5810c-132">String</span></span>|<span data-ttu-id="5810c-133">UserId</span><span class="sxs-lookup"><span data-stu-id="5810c-133">UserId</span></span>|
|<span data-ttu-id="5810c-134">userName</span><span class="sxs-lookup"><span data-stu-id="5810c-134">userName</span></span>|<span data-ttu-id="5810c-135">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5810c-135">String</span></span>|<span data-ttu-id="5810c-136">UserName</span><span class="sxs-lookup"><span data-stu-id="5810c-136">UserName</span></span>|
|<span data-ttu-id="5810c-137">userEmail</span><span class="sxs-lookup"><span data-stu-id="5810c-137">userEmail</span></span>|<span data-ttu-id="5810c-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5810c-138">String</span></span>|<span data-ttu-id="5810c-139">UserEmail</span><span class="sxs-lookup"><span data-stu-id="5810c-139">UserEmail</span></span>|
|<span data-ttu-id="5810c-140">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="5810c-140">userPrincipalName</span></span>|<span data-ttu-id="5810c-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5810c-141">String</span></span>|<span data-ttu-id="5810c-142">UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="5810c-142">UserPrincipalName.</span></span>|
|<span data-ttu-id="5810c-143">sources</span><span class="sxs-lookup"><span data-stu-id="5810c-143">sources</span></span>|<span data-ttu-id="5810c-144">Coleção [settingSource](../resources/intune-deviceconfig-settingsource.md)</span><span class="sxs-lookup"><span data-stu-id="5810c-144">[settingSource](../resources/intune-deviceconfig-settingsource.md) collection</span></span>|<span data-ttu-id="5810c-145">Políticas colaboradoras</span><span class="sxs-lookup"><span data-stu-id="5810c-145">Contributing policies</span></span>|
|<span data-ttu-id="5810c-146">currentValue</span><span class="sxs-lookup"><span data-stu-id="5810c-146">currentValue</span></span>|<span data-ttu-id="5810c-147">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5810c-147">String</span></span>|<span data-ttu-id="5810c-148">Valor atual da configuração no dispositivo</span><span class="sxs-lookup"><span data-stu-id="5810c-148">Current value of setting on device</span></span>|

## <a name="relationships"></a><span data-ttu-id="5810c-149">Relações</span><span class="sxs-lookup"><span data-stu-id="5810c-149">Relationships</span></span>
<span data-ttu-id="5810c-150">Nenhum</span><span class="sxs-lookup"><span data-stu-id="5810c-150">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="5810c-151">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5810c-151">JSON Representation</span></span>
<span data-ttu-id="5810c-152">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="5810c-152">Here is a JSON representation of the resource.</span></span>
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





