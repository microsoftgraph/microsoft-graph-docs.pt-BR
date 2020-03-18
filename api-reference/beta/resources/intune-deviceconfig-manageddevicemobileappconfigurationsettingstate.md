---
title: tipo de recurso managedDeviceMobileAppConfigurationSettingState
description: Estado da configuração do aplicativo móvel do dispositivo gerenciado para um determinado dispositivo.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 740d2fe591810829080ed6da78e9c6fcc68e7d52
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42788615"
---
# <a name="manageddevicemobileappconfigurationsettingstate-resource-type"></a><span data-ttu-id="2dc98-103">tipo de recurso managedDeviceMobileAppConfigurationSettingState</span><span class="sxs-lookup"><span data-stu-id="2dc98-103">managedDeviceMobileAppConfigurationSettingState resource type</span></span>

> <span data-ttu-id="2dc98-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="2dc98-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2dc98-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2dc98-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2dc98-106">Estado da configuração do aplicativo móvel do dispositivo gerenciado para um determinado dispositivo.</span><span class="sxs-lookup"><span data-stu-id="2dc98-106">Managed Device Mobile App Configuration Setting State for a given device.</span></span>

## <a name="properties"></a><span data-ttu-id="2dc98-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2dc98-107">Properties</span></span>
|<span data-ttu-id="2dc98-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2dc98-108">Property</span></span>|<span data-ttu-id="2dc98-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="2dc98-109">Type</span></span>|<span data-ttu-id="2dc98-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="2dc98-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2dc98-111">configuração</span><span class="sxs-lookup"><span data-stu-id="2dc98-111">setting</span></span>|<span data-ttu-id="2dc98-112">String</span><span class="sxs-lookup"><span data-stu-id="2dc98-112">String</span></span>|<span data-ttu-id="2dc98-113">A configuração que é relatada</span><span class="sxs-lookup"><span data-stu-id="2dc98-113">The setting that is being reported</span></span>|
|<span data-ttu-id="2dc98-114">settingName</span><span class="sxs-lookup"><span data-stu-id="2dc98-114">settingName</span></span>|<span data-ttu-id="2dc98-115">String</span><span class="sxs-lookup"><span data-stu-id="2dc98-115">String</span></span>|<span data-ttu-id="2dc98-116">Nome de configuração localizada/de usuário que é relatada</span><span class="sxs-lookup"><span data-stu-id="2dc98-116">Localized/user friendly setting name that is being reported</span></span>|
|<span data-ttu-id="2dc98-117">instanceDisplayName</span><span class="sxs-lookup"><span data-stu-id="2dc98-117">instanceDisplayName</span></span>|<span data-ttu-id="2dc98-118">String</span><span class="sxs-lookup"><span data-stu-id="2dc98-118">String</span></span>|<span data-ttu-id="2dc98-119">Nome da instância de configuração que é relatada.</span><span class="sxs-lookup"><span data-stu-id="2dc98-119">Name of setting instance that is being reported.</span></span>|
|<span data-ttu-id="2dc98-120">state</span><span class="sxs-lookup"><span data-stu-id="2dc98-120">state</span></span>|[<span data-ttu-id="2dc98-121">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="2dc98-121">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="2dc98-122">O estado de conformidade da configuração.</span><span class="sxs-lookup"><span data-stu-id="2dc98-122">The compliance state of the setting.</span></span> <span data-ttu-id="2dc98-123">Os valores possíveis são: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="2dc98-123">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="2dc98-124">errorCode</span><span class="sxs-lookup"><span data-stu-id="2dc98-124">errorCode</span></span>|<span data-ttu-id="2dc98-125">Int64</span><span class="sxs-lookup"><span data-stu-id="2dc98-125">Int64</span></span>|<span data-ttu-id="2dc98-126">Código de erro da configuração</span><span class="sxs-lookup"><span data-stu-id="2dc98-126">Error code for the setting</span></span>|
|<span data-ttu-id="2dc98-127">errorDescription</span><span class="sxs-lookup"><span data-stu-id="2dc98-127">errorDescription</span></span>|<span data-ttu-id="2dc98-128">String</span><span class="sxs-lookup"><span data-stu-id="2dc98-128">String</span></span>|<span data-ttu-id="2dc98-129">Descrição de erro</span><span class="sxs-lookup"><span data-stu-id="2dc98-129">Error description</span></span>|
|<span data-ttu-id="2dc98-130">userId</span><span class="sxs-lookup"><span data-stu-id="2dc98-130">userId</span></span>|<span data-ttu-id="2dc98-131">String</span><span class="sxs-lookup"><span data-stu-id="2dc98-131">String</span></span>|<span data-ttu-id="2dc98-132">UserId</span><span class="sxs-lookup"><span data-stu-id="2dc98-132">UserId</span></span>|
|<span data-ttu-id="2dc98-133">userName</span><span class="sxs-lookup"><span data-stu-id="2dc98-133">userName</span></span>|<span data-ttu-id="2dc98-134">String</span><span class="sxs-lookup"><span data-stu-id="2dc98-134">String</span></span>|<span data-ttu-id="2dc98-135">UserName</span><span class="sxs-lookup"><span data-stu-id="2dc98-135">UserName</span></span>|
|<span data-ttu-id="2dc98-136">userEmail</span><span class="sxs-lookup"><span data-stu-id="2dc98-136">userEmail</span></span>|<span data-ttu-id="2dc98-137">String</span><span class="sxs-lookup"><span data-stu-id="2dc98-137">String</span></span>|<span data-ttu-id="2dc98-138">UserEmail</span><span class="sxs-lookup"><span data-stu-id="2dc98-138">UserEmail</span></span>|
|<span data-ttu-id="2dc98-139">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="2dc98-139">userPrincipalName</span></span>|<span data-ttu-id="2dc98-140">String</span><span class="sxs-lookup"><span data-stu-id="2dc98-140">String</span></span>|<span data-ttu-id="2dc98-141">UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="2dc98-141">UserPrincipalName.</span></span>|
|<span data-ttu-id="2dc98-142">fontes</span><span class="sxs-lookup"><span data-stu-id="2dc98-142">sources</span></span>|<span data-ttu-id="2dc98-143">Conjunto [settingSource](../resources/intune-deviceconfig-settingsource.md)</span><span class="sxs-lookup"><span data-stu-id="2dc98-143">[settingSource](../resources/intune-deviceconfig-settingsource.md) collection</span></span>|<span data-ttu-id="2dc98-144">Políticas de colaboração</span><span class="sxs-lookup"><span data-stu-id="2dc98-144">Contributing policies</span></span>|
|<span data-ttu-id="2dc98-145">currentValue</span><span class="sxs-lookup"><span data-stu-id="2dc98-145">currentValue</span></span>|<span data-ttu-id="2dc98-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2dc98-146">String</span></span>|<span data-ttu-id="2dc98-147">Valor atual da configuração em um dispositivo</span><span class="sxs-lookup"><span data-stu-id="2dc98-147">Current value of setting on device</span></span>|

## <a name="relationships"></a><span data-ttu-id="2dc98-148">Relações</span><span class="sxs-lookup"><span data-stu-id="2dc98-148">Relationships</span></span>
<span data-ttu-id="2dc98-149">Nenhum</span><span class="sxs-lookup"><span data-stu-id="2dc98-149">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2dc98-150">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2dc98-150">JSON Representation</span></span>
<span data-ttu-id="2dc98-151">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2dc98-151">Here is a JSON representation of the resource.</span></span>
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



