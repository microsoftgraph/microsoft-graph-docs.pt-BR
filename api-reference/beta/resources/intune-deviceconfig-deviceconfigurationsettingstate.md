---
title: tipo de recurso deviceConfigurationSettingState
description: Estado da definição de configuração de um determinado dispositivo.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0acfcd697815ee9403e6144c5da34dd824022de3
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30165881"
---
# <a name="deviceconfigurationsettingstate-resource-type"></a><span data-ttu-id="760a3-103">tipo de recurso deviceConfigurationSettingState</span><span class="sxs-lookup"><span data-stu-id="760a3-103">deviceConfigurationSettingState resource type</span></span>

> <span data-ttu-id="760a3-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="760a3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="760a3-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="760a3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="760a3-106">Estado da definição de configuração de um determinado dispositivo.</span><span class="sxs-lookup"><span data-stu-id="760a3-106">Device Configuration Setting State for a given device.</span></span>

## <a name="properties"></a><span data-ttu-id="760a3-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="760a3-107">Properties</span></span>
|<span data-ttu-id="760a3-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="760a3-108">Property</span></span>|<span data-ttu-id="760a3-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="760a3-109">Type</span></span>|<span data-ttu-id="760a3-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="760a3-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="760a3-111">configuração</span><span class="sxs-lookup"><span data-stu-id="760a3-111">setting</span></span>|<span data-ttu-id="760a3-112">String</span><span class="sxs-lookup"><span data-stu-id="760a3-112">String</span></span>|<span data-ttu-id="760a3-113">A configuração que está sendo relatada</span><span class="sxs-lookup"><span data-stu-id="760a3-113">The setting that is being reported</span></span>|
|<span data-ttu-id="760a3-114">settingName</span><span class="sxs-lookup"><span data-stu-id="760a3-114">settingName</span></span>|<span data-ttu-id="760a3-115">String</span><span class="sxs-lookup"><span data-stu-id="760a3-115">String</span></span>|<span data-ttu-id="760a3-116">Nome traduzido/amigável para o usuário da configuração que está sendo relatada</span><span class="sxs-lookup"><span data-stu-id="760a3-116">Localized/user friendly setting name that is being reported</span></span>|
|<span data-ttu-id="760a3-117">instanceDisplayName</span><span class="sxs-lookup"><span data-stu-id="760a3-117">instanceDisplayName</span></span>|<span data-ttu-id="760a3-118">String</span><span class="sxs-lookup"><span data-stu-id="760a3-118">String</span></span>|<span data-ttu-id="760a3-119">Nome da instância de configuração está sendo relatada.</span><span class="sxs-lookup"><span data-stu-id="760a3-119">Name of setting instance that is being reported.</span></span>|
|<span data-ttu-id="760a3-120">state</span><span class="sxs-lookup"><span data-stu-id="760a3-120">state</span></span>|[<span data-ttu-id="760a3-121">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="760a3-121">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="760a3-122">O estado de conformidade da configuração.</span><span class="sxs-lookup"><span data-stu-id="760a3-122">The compliance state of the setting.</span></span> <span data-ttu-id="760a3-123">Os valores possíveis são: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="760a3-123">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="760a3-124">errorCode</span><span class="sxs-lookup"><span data-stu-id="760a3-124">errorCode</span></span>|<span data-ttu-id="760a3-125">Int64</span><span class="sxs-lookup"><span data-stu-id="760a3-125">Int64</span></span>|<span data-ttu-id="760a3-126">Código de erro da configuração</span><span class="sxs-lookup"><span data-stu-id="760a3-126">Error code for the setting</span></span>|
|<span data-ttu-id="760a3-127">errorDescription</span><span class="sxs-lookup"><span data-stu-id="760a3-127">errorDescription</span></span>|<span data-ttu-id="760a3-128">String</span><span class="sxs-lookup"><span data-stu-id="760a3-128">String</span></span>|<span data-ttu-id="760a3-129">Descrição do erro</span><span class="sxs-lookup"><span data-stu-id="760a3-129">Error description</span></span>|
|<span data-ttu-id="760a3-130">userId</span><span class="sxs-lookup"><span data-stu-id="760a3-130">userId</span></span>|<span data-ttu-id="760a3-131">String</span><span class="sxs-lookup"><span data-stu-id="760a3-131">String</span></span>|<span data-ttu-id="760a3-132">UserId</span><span class="sxs-lookup"><span data-stu-id="760a3-132">UserId</span></span>|
|<span data-ttu-id="760a3-133">userName</span><span class="sxs-lookup"><span data-stu-id="760a3-133">userName</span></span>|<span data-ttu-id="760a3-134">String</span><span class="sxs-lookup"><span data-stu-id="760a3-134">String</span></span>|<span data-ttu-id="760a3-135">UserName</span><span class="sxs-lookup"><span data-stu-id="760a3-135">UserName</span></span>|
|<span data-ttu-id="760a3-136">userEmail</span><span class="sxs-lookup"><span data-stu-id="760a3-136">userEmail</span></span>|<span data-ttu-id="760a3-137">String</span><span class="sxs-lookup"><span data-stu-id="760a3-137">String</span></span>|<span data-ttu-id="760a3-138">UserEmail</span><span class="sxs-lookup"><span data-stu-id="760a3-138">UserEmail</span></span>|
|<span data-ttu-id="760a3-139">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="760a3-139">userPrincipalName</span></span>|<span data-ttu-id="760a3-140">String</span><span class="sxs-lookup"><span data-stu-id="760a3-140">String</span></span>|<span data-ttu-id="760a3-141">UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="760a3-141">UserPrincipalName.</span></span>|
|<span data-ttu-id="760a3-142">sources</span><span class="sxs-lookup"><span data-stu-id="760a3-142">sources</span></span>|<span data-ttu-id="760a3-143">Coleção [settingSource](../resources/intune-deviceconfig-settingsource.md)</span><span class="sxs-lookup"><span data-stu-id="760a3-143">[settingSource](../resources/intune-deviceconfig-settingsource.md) collection</span></span>|<span data-ttu-id="760a3-144">Políticas colaboradoras</span><span class="sxs-lookup"><span data-stu-id="760a3-144">Contributing policies</span></span>|
|<span data-ttu-id="760a3-145">currentValue</span><span class="sxs-lookup"><span data-stu-id="760a3-145">currentValue</span></span>|<span data-ttu-id="760a3-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="760a3-146">String</span></span>|<span data-ttu-id="760a3-147">Valor atual da configuração no dispositivo</span><span class="sxs-lookup"><span data-stu-id="760a3-147">Current value of setting on device</span></span>|

## <a name="relationships"></a><span data-ttu-id="760a3-148">Relações</span><span class="sxs-lookup"><span data-stu-id="760a3-148">Relationships</span></span>
<span data-ttu-id="760a3-149">Nenhum</span><span class="sxs-lookup"><span data-stu-id="760a3-149">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="760a3-150">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="760a3-150">JSON Representation</span></span>
<span data-ttu-id="760a3-151">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="760a3-151">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceConfigurationSettingState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceConfigurationSettingState",
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




