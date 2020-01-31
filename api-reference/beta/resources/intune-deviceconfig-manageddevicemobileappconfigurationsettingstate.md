---
title: tipo de recurso managedDeviceMobileAppConfigurationSettingState
description: Estado da configuração do aplicativo móvel do dispositivo gerenciado para um determinado dispositivo.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: d828b57e6ae76e3a0babcc2b27a009e60f7a6407
ms.sourcegitcommit: b12904a27b6d0e197f562aca0dac5e74cd7bd3a1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/31/2020
ms.locfileid: "41636014"
---
# <a name="manageddevicemobileappconfigurationsettingstate-resource-type"></a><span data-ttu-id="a853f-103">tipo de recurso managedDeviceMobileAppConfigurationSettingState</span><span class="sxs-lookup"><span data-stu-id="a853f-103">managedDeviceMobileAppConfigurationSettingState resource type</span></span>

> <span data-ttu-id="a853f-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a853f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a853f-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a853f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a853f-106">Estado da configuração do aplicativo móvel do dispositivo gerenciado para um determinado dispositivo.</span><span class="sxs-lookup"><span data-stu-id="a853f-106">Managed Device Mobile App Configuration Setting State for a given device.</span></span>

## <a name="properties"></a><span data-ttu-id="a853f-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a853f-107">Properties</span></span>
|<span data-ttu-id="a853f-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a853f-108">Property</span></span>|<span data-ttu-id="a853f-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="a853f-109">Type</span></span>|<span data-ttu-id="a853f-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="a853f-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a853f-111">configuração</span><span class="sxs-lookup"><span data-stu-id="a853f-111">setting</span></span>|<span data-ttu-id="a853f-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a853f-112">String</span></span>|<span data-ttu-id="a853f-113">A configuração que é relatada</span><span class="sxs-lookup"><span data-stu-id="a853f-113">The setting that is being reported</span></span>|
|<span data-ttu-id="a853f-114">settingName</span><span class="sxs-lookup"><span data-stu-id="a853f-114">settingName</span></span>|<span data-ttu-id="a853f-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a853f-115">String</span></span>|<span data-ttu-id="a853f-116">Nome de configuração localizada/de usuário que é relatada</span><span class="sxs-lookup"><span data-stu-id="a853f-116">Localized/user friendly setting name that is being reported</span></span>|
|<span data-ttu-id="a853f-117">instanceDisplayName</span><span class="sxs-lookup"><span data-stu-id="a853f-117">instanceDisplayName</span></span>|<span data-ttu-id="a853f-118">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a853f-118">String</span></span>|<span data-ttu-id="a853f-119">Nome da instância de configuração que é relatada.</span><span class="sxs-lookup"><span data-stu-id="a853f-119">Name of setting instance that is being reported.</span></span>|
|<span data-ttu-id="a853f-120">state</span><span class="sxs-lookup"><span data-stu-id="a853f-120">state</span></span>|[<span data-ttu-id="a853f-121">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="a853f-121">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="a853f-122">O estado de conformidade da configuração.</span><span class="sxs-lookup"><span data-stu-id="a853f-122">The compliance state of the setting.</span></span> <span data-ttu-id="a853f-123">Os valores possíveis são: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="a853f-123">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="a853f-124">errorCode</span><span class="sxs-lookup"><span data-stu-id="a853f-124">errorCode</span></span>|<span data-ttu-id="a853f-125">Int64</span><span class="sxs-lookup"><span data-stu-id="a853f-125">Int64</span></span>|<span data-ttu-id="a853f-126">Código de erro da configuração</span><span class="sxs-lookup"><span data-stu-id="a853f-126">Error code for the setting</span></span>|
|<span data-ttu-id="a853f-127">errorDescription</span><span class="sxs-lookup"><span data-stu-id="a853f-127">errorDescription</span></span>|<span data-ttu-id="a853f-128">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a853f-128">String</span></span>|<span data-ttu-id="a853f-129">Descrição de erro</span><span class="sxs-lookup"><span data-stu-id="a853f-129">Error description</span></span>|
|<span data-ttu-id="a853f-130">userId</span><span class="sxs-lookup"><span data-stu-id="a853f-130">userId</span></span>|<span data-ttu-id="a853f-131">String</span><span class="sxs-lookup"><span data-stu-id="a853f-131">String</span></span>|<span data-ttu-id="a853f-132">UserId</span><span class="sxs-lookup"><span data-stu-id="a853f-132">UserId</span></span>|
|<span data-ttu-id="a853f-133">userName</span><span class="sxs-lookup"><span data-stu-id="a853f-133">userName</span></span>|<span data-ttu-id="a853f-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a853f-134">String</span></span>|<span data-ttu-id="a853f-135">UserName</span><span class="sxs-lookup"><span data-stu-id="a853f-135">UserName</span></span>|
|<span data-ttu-id="a853f-136">userEmail</span><span class="sxs-lookup"><span data-stu-id="a853f-136">userEmail</span></span>|<span data-ttu-id="a853f-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a853f-137">String</span></span>|<span data-ttu-id="a853f-138">UserEmail</span><span class="sxs-lookup"><span data-stu-id="a853f-138">UserEmail</span></span>|
|<span data-ttu-id="a853f-139">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="a853f-139">userPrincipalName</span></span>|<span data-ttu-id="a853f-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a853f-140">String</span></span>|<span data-ttu-id="a853f-141">UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="a853f-141">UserPrincipalName.</span></span>|
|<span data-ttu-id="a853f-142">fontes</span><span class="sxs-lookup"><span data-stu-id="a853f-142">sources</span></span>|<span data-ttu-id="a853f-143">Conjunto [settingSource](../resources/intune-deviceconfig-settingsource.md)</span><span class="sxs-lookup"><span data-stu-id="a853f-143">[settingSource](../resources/intune-deviceconfig-settingsource.md) collection</span></span>|<span data-ttu-id="a853f-144">Políticas de colaboração</span><span class="sxs-lookup"><span data-stu-id="a853f-144">Contributing policies</span></span>|
|<span data-ttu-id="a853f-145">currentValue</span><span class="sxs-lookup"><span data-stu-id="a853f-145">currentValue</span></span>|<span data-ttu-id="a853f-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a853f-146">String</span></span>|<span data-ttu-id="a853f-147">Valor atual da configuração em um dispositivo</span><span class="sxs-lookup"><span data-stu-id="a853f-147">Current value of setting on device</span></span>|

## <a name="relationships"></a><span data-ttu-id="a853f-148">Relações</span><span class="sxs-lookup"><span data-stu-id="a853f-148">Relationships</span></span>
<span data-ttu-id="a853f-149">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a853f-149">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a853f-150">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a853f-150">JSON Representation</span></span>
<span data-ttu-id="a853f-151">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a853f-151">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managedDeviceMobileAppConfigurationSettingState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationSettingState",
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



