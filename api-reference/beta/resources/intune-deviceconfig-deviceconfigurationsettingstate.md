---
title: tipo de recurso deviceConfigurationSettingState
description: Estado da definição de configuração de um determinado dispositivo.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: fc19501be107d4b63d1bd9fe9e579070f392ba79
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33947005"
---
# <a name="deviceconfigurationsettingstate-resource-type"></a><span data-ttu-id="81351-103">tipo de recurso deviceConfigurationSettingState</span><span class="sxs-lookup"><span data-stu-id="81351-103">deviceConfigurationSettingState resource type</span></span>

> <span data-ttu-id="81351-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="81351-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="81351-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="81351-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="81351-106">Estado da definição de configuração de um determinado dispositivo.</span><span class="sxs-lookup"><span data-stu-id="81351-106">Device Configuration Setting State for a given device.</span></span>

## <a name="properties"></a><span data-ttu-id="81351-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="81351-107">Properties</span></span>
|<span data-ttu-id="81351-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="81351-108">Property</span></span>|<span data-ttu-id="81351-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="81351-109">Type</span></span>|<span data-ttu-id="81351-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="81351-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="81351-111">configuração</span><span class="sxs-lookup"><span data-stu-id="81351-111">setting</span></span>|<span data-ttu-id="81351-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="81351-112">String</span></span>|<span data-ttu-id="81351-113">A configuração que é relatada</span><span class="sxs-lookup"><span data-stu-id="81351-113">The setting that is being reported</span></span>|
|<span data-ttu-id="81351-114">settingName</span><span class="sxs-lookup"><span data-stu-id="81351-114">settingName</span></span>|<span data-ttu-id="81351-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="81351-115">String</span></span>|<span data-ttu-id="81351-116">Nome de configuração localizada/de usuário que é relatada</span><span class="sxs-lookup"><span data-stu-id="81351-116">Localized/user friendly setting name that is being reported</span></span>|
|<span data-ttu-id="81351-117">instanceDisplayName</span><span class="sxs-lookup"><span data-stu-id="81351-117">instanceDisplayName</span></span>|<span data-ttu-id="81351-118">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="81351-118">String</span></span>|<span data-ttu-id="81351-119">Nome da instância de configuração que é relatada.</span><span class="sxs-lookup"><span data-stu-id="81351-119">Name of setting instance that is being reported.</span></span>|
|<span data-ttu-id="81351-120">state</span><span class="sxs-lookup"><span data-stu-id="81351-120">state</span></span>|[<span data-ttu-id="81351-121">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="81351-121">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="81351-122">O estado de conformidade da configuração.</span><span class="sxs-lookup"><span data-stu-id="81351-122">The compliance state of the setting.</span></span> <span data-ttu-id="81351-123">Os valores possíveis são: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="81351-123">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="81351-124">errorCode</span><span class="sxs-lookup"><span data-stu-id="81351-124">errorCode</span></span>|<span data-ttu-id="81351-125">Int64</span><span class="sxs-lookup"><span data-stu-id="81351-125">Int64</span></span>|<span data-ttu-id="81351-126">Código de erro da configuração</span><span class="sxs-lookup"><span data-stu-id="81351-126">Error code for the setting</span></span>|
|<span data-ttu-id="81351-127">errorDescription</span><span class="sxs-lookup"><span data-stu-id="81351-127">errorDescription</span></span>|<span data-ttu-id="81351-128">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="81351-128">String</span></span>|<span data-ttu-id="81351-129">Descrição de erro</span><span class="sxs-lookup"><span data-stu-id="81351-129">Error description</span></span>|
|<span data-ttu-id="81351-130">userId</span><span class="sxs-lookup"><span data-stu-id="81351-130">userId</span></span>|<span data-ttu-id="81351-131">String</span><span class="sxs-lookup"><span data-stu-id="81351-131">String</span></span>|<span data-ttu-id="81351-132">UserId</span><span class="sxs-lookup"><span data-stu-id="81351-132">UserId</span></span>|
|<span data-ttu-id="81351-133">userName</span><span class="sxs-lookup"><span data-stu-id="81351-133">userName</span></span>|<span data-ttu-id="81351-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="81351-134">String</span></span>|<span data-ttu-id="81351-135">UserName</span><span class="sxs-lookup"><span data-stu-id="81351-135">UserName</span></span>|
|<span data-ttu-id="81351-136">userEmail</span><span class="sxs-lookup"><span data-stu-id="81351-136">userEmail</span></span>|<span data-ttu-id="81351-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="81351-137">String</span></span>|<span data-ttu-id="81351-138">UserEmail</span><span class="sxs-lookup"><span data-stu-id="81351-138">UserEmail</span></span>|
|<span data-ttu-id="81351-139">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="81351-139">userPrincipalName</span></span>|<span data-ttu-id="81351-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="81351-140">String</span></span>|<span data-ttu-id="81351-141">UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="81351-141">UserPrincipalName.</span></span>|
|<span data-ttu-id="81351-142">fontes</span><span class="sxs-lookup"><span data-stu-id="81351-142">sources</span></span>|<span data-ttu-id="81351-143">Conjunto [settingSource](../resources/intune-deviceconfig-settingsource.md)</span><span class="sxs-lookup"><span data-stu-id="81351-143">[settingSource](../resources/intune-deviceconfig-settingsource.md) collection</span></span>|<span data-ttu-id="81351-144">Políticas de colaboração</span><span class="sxs-lookup"><span data-stu-id="81351-144">Contributing policies</span></span>|
|<span data-ttu-id="81351-145">currentValue</span><span class="sxs-lookup"><span data-stu-id="81351-145">currentValue</span></span>|<span data-ttu-id="81351-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="81351-146">String</span></span>|<span data-ttu-id="81351-147">Valor atual da configuração em um dispositivo</span><span class="sxs-lookup"><span data-stu-id="81351-147">Current value of setting on device</span></span>|

## <a name="relationships"></a><span data-ttu-id="81351-148">Relações</span><span class="sxs-lookup"><span data-stu-id="81351-148">Relationships</span></span>
<span data-ttu-id="81351-149">Nenhum</span><span class="sxs-lookup"><span data-stu-id="81351-149">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="81351-150">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="81351-150">JSON Representation</span></span>
<span data-ttu-id="81351-151">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="81351-151">Here is a JSON representation of the resource.</span></span>
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




