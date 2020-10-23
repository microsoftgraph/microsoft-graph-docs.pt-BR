---
title: tipo de recurso managedDeviceMobileAppConfigurationSettingState
description: Estado da configuração do aplicativo móvel do dispositivo gerenciado para um determinado dispositivo.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: e760b026f775abcec54f2cd34922de56f202ab2e
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48710031"
---
# <a name="manageddevicemobileappconfigurationsettingstate-resource-type"></a><span data-ttu-id="121d5-103">tipo de recurso managedDeviceMobileAppConfigurationSettingState</span><span class="sxs-lookup"><span data-stu-id="121d5-103">managedDeviceMobileAppConfigurationSettingState resource type</span></span>

<span data-ttu-id="121d5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="121d5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="121d5-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="121d5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="121d5-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="121d5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="121d5-107">Estado da configuração do aplicativo móvel do dispositivo gerenciado para um determinado dispositivo.</span><span class="sxs-lookup"><span data-stu-id="121d5-107">Managed Device Mobile App Configuration Setting State for a given device.</span></span>

## <a name="properties"></a><span data-ttu-id="121d5-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="121d5-108">Properties</span></span>
|<span data-ttu-id="121d5-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="121d5-109">Property</span></span>|<span data-ttu-id="121d5-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="121d5-110">Type</span></span>|<span data-ttu-id="121d5-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="121d5-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="121d5-112">configuração</span><span class="sxs-lookup"><span data-stu-id="121d5-112">setting</span></span>|<span data-ttu-id="121d5-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="121d5-113">String</span></span>|<span data-ttu-id="121d5-114">A configuração que é relatada</span><span class="sxs-lookup"><span data-stu-id="121d5-114">The setting that is being reported</span></span>|
|<span data-ttu-id="121d5-115">settingName</span><span class="sxs-lookup"><span data-stu-id="121d5-115">settingName</span></span>|<span data-ttu-id="121d5-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="121d5-116">String</span></span>|<span data-ttu-id="121d5-117">Nome de configuração localizada/de usuário que é relatada</span><span class="sxs-lookup"><span data-stu-id="121d5-117">Localized/user friendly setting name that is being reported</span></span>|
|<span data-ttu-id="121d5-118">instanceDisplayName</span><span class="sxs-lookup"><span data-stu-id="121d5-118">instanceDisplayName</span></span>|<span data-ttu-id="121d5-119">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="121d5-119">String</span></span>|<span data-ttu-id="121d5-120">Nome da instância de configuração que é relatada.</span><span class="sxs-lookup"><span data-stu-id="121d5-120">Name of setting instance that is being reported.</span></span>|
|<span data-ttu-id="121d5-121">state</span><span class="sxs-lookup"><span data-stu-id="121d5-121">state</span></span>|[<span data-ttu-id="121d5-122">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="121d5-122">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="121d5-123">O estado de conformidade da configuração.</span><span class="sxs-lookup"><span data-stu-id="121d5-123">The compliance state of the setting.</span></span> <span data-ttu-id="121d5-124">Os valores possíveis são: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="121d5-124">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="121d5-125">errorCode</span><span class="sxs-lookup"><span data-stu-id="121d5-125">errorCode</span></span>|<span data-ttu-id="121d5-126">Int64</span><span class="sxs-lookup"><span data-stu-id="121d5-126">Int64</span></span>|<span data-ttu-id="121d5-127">Código de erro da configuração</span><span class="sxs-lookup"><span data-stu-id="121d5-127">Error code for the setting</span></span>|
|<span data-ttu-id="121d5-128">errorDescription</span><span class="sxs-lookup"><span data-stu-id="121d5-128">errorDescription</span></span>|<span data-ttu-id="121d5-129">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="121d5-129">String</span></span>|<span data-ttu-id="121d5-130">Descrição de erro</span><span class="sxs-lookup"><span data-stu-id="121d5-130">Error description</span></span>|
|<span data-ttu-id="121d5-131">userId</span><span class="sxs-lookup"><span data-stu-id="121d5-131">userId</span></span>|<span data-ttu-id="121d5-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="121d5-132">String</span></span>|<span data-ttu-id="121d5-133">UserId</span><span class="sxs-lookup"><span data-stu-id="121d5-133">UserId</span></span>|
|<span data-ttu-id="121d5-134">userName</span><span class="sxs-lookup"><span data-stu-id="121d5-134">userName</span></span>|<span data-ttu-id="121d5-135">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="121d5-135">String</span></span>|<span data-ttu-id="121d5-136">UserName</span><span class="sxs-lookup"><span data-stu-id="121d5-136">UserName</span></span>|
|<span data-ttu-id="121d5-137">userEmail</span><span class="sxs-lookup"><span data-stu-id="121d5-137">userEmail</span></span>|<span data-ttu-id="121d5-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="121d5-138">String</span></span>|<span data-ttu-id="121d5-139">UserEmail</span><span class="sxs-lookup"><span data-stu-id="121d5-139">UserEmail</span></span>|
|<span data-ttu-id="121d5-140">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="121d5-140">userPrincipalName</span></span>|<span data-ttu-id="121d5-141">String</span><span class="sxs-lookup"><span data-stu-id="121d5-141">String</span></span>|<span data-ttu-id="121d5-142">UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="121d5-142">UserPrincipalName.</span></span>|
|<span data-ttu-id="121d5-143">fontes</span><span class="sxs-lookup"><span data-stu-id="121d5-143">sources</span></span>|<span data-ttu-id="121d5-144">Conjunto [settingSource](../resources/intune-deviceconfig-settingsource.md)</span><span class="sxs-lookup"><span data-stu-id="121d5-144">[settingSource](../resources/intune-deviceconfig-settingsource.md) collection</span></span>|<span data-ttu-id="121d5-145">Políticas de colaboração</span><span class="sxs-lookup"><span data-stu-id="121d5-145">Contributing policies</span></span>|
|<span data-ttu-id="121d5-146">currentValue</span><span class="sxs-lookup"><span data-stu-id="121d5-146">currentValue</span></span>|<span data-ttu-id="121d5-147">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="121d5-147">String</span></span>|<span data-ttu-id="121d5-148">Valor atual da configuração em um dispositivo</span><span class="sxs-lookup"><span data-stu-id="121d5-148">Current value of setting on device</span></span>|
|<span data-ttu-id="121d5-149">settingInstanceId</span><span class="sxs-lookup"><span data-stu-id="121d5-149">settingInstanceId</span></span>|<span data-ttu-id="121d5-150">String</span><span class="sxs-lookup"><span data-stu-id="121d5-150">String</span></span>|<span data-ttu-id="121d5-151">SettingInstanceId</span><span class="sxs-lookup"><span data-stu-id="121d5-151">SettingInstanceId</span></span>|

## <a name="relationships"></a><span data-ttu-id="121d5-152">Relações</span><span class="sxs-lookup"><span data-stu-id="121d5-152">Relationships</span></span>
<span data-ttu-id="121d5-153">Nenhum</span><span class="sxs-lookup"><span data-stu-id="121d5-153">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="121d5-154">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="121d5-154">JSON Representation</span></span>
<span data-ttu-id="121d5-155">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="121d5-155">Here is a JSON representation of the resource.</span></span>
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
      "displayName": "String",
      "sourceType": "String"
    }
  ],
  "currentValue": "String",
  "settingInstanceId": "String"
}
```





