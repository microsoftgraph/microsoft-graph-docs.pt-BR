---
title: Tipo de recurso deviceCompliancePolicySettingState
description: Estado da configuração da política de conformidade de dispositivo para um determinado dispositivo.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: b17930161f66ca83d59e3f2f62777a79f82b79f0
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425733"
---
# <a name="devicecompliancepolicysettingstate-resource-type"></a><span data-ttu-id="cb225-103">Tipo de recurso deviceCompliancePolicySettingState</span><span class="sxs-lookup"><span data-stu-id="cb225-103">deviceCompliancePolicySettingState resource type</span></span>

> <span data-ttu-id="cb225-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="cb225-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="cb225-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="cb225-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="cb225-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="cb225-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cb225-107">Estado da configuração da política de conformidade de dispositivo para um determinado dispositivo.</span><span class="sxs-lookup"><span data-stu-id="cb225-107">Device Compilance Policy Setting State for a given device.</span></span>

## <a name="properties"></a><span data-ttu-id="cb225-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="cb225-108">Properties</span></span>
|<span data-ttu-id="cb225-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cb225-109">Property</span></span>|<span data-ttu-id="cb225-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="cb225-110">Type</span></span>|<span data-ttu-id="cb225-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="cb225-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cb225-112">configuração</span><span class="sxs-lookup"><span data-stu-id="cb225-112">setting</span></span>|<span data-ttu-id="cb225-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cb225-113">String</span></span>|<span data-ttu-id="cb225-114">A configuração que está sendo relatada</span><span class="sxs-lookup"><span data-stu-id="cb225-114">The setting that is being reported</span></span>|
|<span data-ttu-id="cb225-115">settingName</span><span class="sxs-lookup"><span data-stu-id="cb225-115">settingName</span></span>|<span data-ttu-id="cb225-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cb225-116">String</span></span>|<span data-ttu-id="cb225-117">Nome traduzido/amigável para o usuário da configuração que está sendo relatada</span><span class="sxs-lookup"><span data-stu-id="cb225-117">Localized/user friendly setting name that is being reported</span></span>|
|<span data-ttu-id="cb225-118">instanceDisplayName</span><span class="sxs-lookup"><span data-stu-id="cb225-118">instanceDisplayName</span></span>|<span data-ttu-id="cb225-119">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cb225-119">String</span></span>|<span data-ttu-id="cb225-120">Nome da instância de configuração está sendo relatada.</span><span class="sxs-lookup"><span data-stu-id="cb225-120">Name of setting instance that is being reported.</span></span>|
|<span data-ttu-id="cb225-121">estado</span><span class="sxs-lookup"><span data-stu-id="cb225-121">state</span></span>|[<span data-ttu-id="cb225-122">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="cb225-122">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="cb225-123">O estado de conformidade da configuração.</span><span class="sxs-lookup"><span data-stu-id="cb225-123">The compliance state of the setting.</span></span> <span data-ttu-id="cb225-124">Os valores possíveis são: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="cb225-124">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="cb225-125">errorCode</span><span class="sxs-lookup"><span data-stu-id="cb225-125">errorCode</span></span>|<span data-ttu-id="cb225-126">Int64</span><span class="sxs-lookup"><span data-stu-id="cb225-126">Int64</span></span>|<span data-ttu-id="cb225-127">Código de erro da configuração</span><span class="sxs-lookup"><span data-stu-id="cb225-127">Error code for the setting</span></span>|
|<span data-ttu-id="cb225-128">errorDescription</span><span class="sxs-lookup"><span data-stu-id="cb225-128">errorDescription</span></span>|<span data-ttu-id="cb225-129">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cb225-129">String</span></span>|<span data-ttu-id="cb225-130">Descrição do erro</span><span class="sxs-lookup"><span data-stu-id="cb225-130">Error description</span></span>|
|<span data-ttu-id="cb225-131">userId</span><span class="sxs-lookup"><span data-stu-id="cb225-131">userId</span></span>|<span data-ttu-id="cb225-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cb225-132">String</span></span>|<span data-ttu-id="cb225-133">UserId</span><span class="sxs-lookup"><span data-stu-id="cb225-133">UserId</span></span>|
|<span data-ttu-id="cb225-134">userName</span><span class="sxs-lookup"><span data-stu-id="cb225-134">userName</span></span>|<span data-ttu-id="cb225-135">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cb225-135">String</span></span>|<span data-ttu-id="cb225-136">UserName</span><span class="sxs-lookup"><span data-stu-id="cb225-136">UserName</span></span>|
|<span data-ttu-id="cb225-137">userEmail</span><span class="sxs-lookup"><span data-stu-id="cb225-137">userEmail</span></span>|<span data-ttu-id="cb225-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cb225-138">String</span></span>|<span data-ttu-id="cb225-139">UserEmail</span><span class="sxs-lookup"><span data-stu-id="cb225-139">UserEmail</span></span>|
|<span data-ttu-id="cb225-140">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="cb225-140">userPrincipalName</span></span>|<span data-ttu-id="cb225-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cb225-141">String</span></span>|<span data-ttu-id="cb225-142">UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="cb225-142">UserPrincipalName.</span></span>|
|<span data-ttu-id="cb225-143">sources</span><span class="sxs-lookup"><span data-stu-id="cb225-143">sources</span></span>|<span data-ttu-id="cb225-144">Coleção [settingSource](../resources/intune-deviceconfig-settingsource.md)</span><span class="sxs-lookup"><span data-stu-id="cb225-144">[settingSource](../resources/intune-deviceconfig-settingsource.md) collection</span></span>|<span data-ttu-id="cb225-145">Políticas colaboradoras</span><span class="sxs-lookup"><span data-stu-id="cb225-145">Contributing policies</span></span>|
|<span data-ttu-id="cb225-146">currentValue</span><span class="sxs-lookup"><span data-stu-id="cb225-146">currentValue</span></span>|<span data-ttu-id="cb225-147">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cb225-147">String</span></span>|<span data-ttu-id="cb225-148">Valor atual da configuração no dispositivo</span><span class="sxs-lookup"><span data-stu-id="cb225-148">Current value of setting on device</span></span>|

## <a name="relationships"></a><span data-ttu-id="cb225-149">Relações</span><span class="sxs-lookup"><span data-stu-id="cb225-149">Relationships</span></span>
<span data-ttu-id="cb225-150">Nenhum</span><span class="sxs-lookup"><span data-stu-id="cb225-150">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="cb225-151">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="cb225-151">JSON Representation</span></span>
<span data-ttu-id="cb225-152">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="cb225-152">Here is a JSON representation of the resource.</span></span>
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




