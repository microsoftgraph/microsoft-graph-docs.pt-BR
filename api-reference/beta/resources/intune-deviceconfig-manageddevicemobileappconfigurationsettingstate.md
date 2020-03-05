---
title: tipo de recurso managedDeviceMobileAppConfigurationSettingState
description: Estado da configuração do aplicativo móvel do dispositivo gerenciado para um determinado dispositivo.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 4b044565f0ec87570bbf9584b37217c0f4881839
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42529645"
---
# <a name="manageddevicemobileappconfigurationsettingstate-resource-type"></a><span data-ttu-id="943e5-103">tipo de recurso managedDeviceMobileAppConfigurationSettingState</span><span class="sxs-lookup"><span data-stu-id="943e5-103">managedDeviceMobileAppConfigurationSettingState resource type</span></span>

<span data-ttu-id="943e5-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="943e5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="943e5-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="943e5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="943e5-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="943e5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="943e5-107">Estado da configuração do aplicativo móvel do dispositivo gerenciado para um determinado dispositivo.</span><span class="sxs-lookup"><span data-stu-id="943e5-107">Managed Device Mobile App Configuration Setting State for a given device.</span></span>

## <a name="properties"></a><span data-ttu-id="943e5-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="943e5-108">Properties</span></span>
|<span data-ttu-id="943e5-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="943e5-109">Property</span></span>|<span data-ttu-id="943e5-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="943e5-110">Type</span></span>|<span data-ttu-id="943e5-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="943e5-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="943e5-112">configuração</span><span class="sxs-lookup"><span data-stu-id="943e5-112">setting</span></span>|<span data-ttu-id="943e5-113">String</span><span class="sxs-lookup"><span data-stu-id="943e5-113">String</span></span>|<span data-ttu-id="943e5-114">A configuração que é relatada</span><span class="sxs-lookup"><span data-stu-id="943e5-114">The setting that is being reported</span></span>|
|<span data-ttu-id="943e5-115">settingName</span><span class="sxs-lookup"><span data-stu-id="943e5-115">settingName</span></span>|<span data-ttu-id="943e5-116">String</span><span class="sxs-lookup"><span data-stu-id="943e5-116">String</span></span>|<span data-ttu-id="943e5-117">Nome de configuração localizada/de usuário que é relatada</span><span class="sxs-lookup"><span data-stu-id="943e5-117">Localized/user friendly setting name that is being reported</span></span>|
|<span data-ttu-id="943e5-118">instanceDisplayName</span><span class="sxs-lookup"><span data-stu-id="943e5-118">instanceDisplayName</span></span>|<span data-ttu-id="943e5-119">String</span><span class="sxs-lookup"><span data-stu-id="943e5-119">String</span></span>|<span data-ttu-id="943e5-120">Nome da instância de configuração que é relatada.</span><span class="sxs-lookup"><span data-stu-id="943e5-120">Name of setting instance that is being reported.</span></span>|
|<span data-ttu-id="943e5-121">state</span><span class="sxs-lookup"><span data-stu-id="943e5-121">state</span></span>|[<span data-ttu-id="943e5-122">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="943e5-122">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="943e5-123">O estado de conformidade da configuração.</span><span class="sxs-lookup"><span data-stu-id="943e5-123">The compliance state of the setting.</span></span> <span data-ttu-id="943e5-124">Os valores possíveis são: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="943e5-124">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="943e5-125">errorCode</span><span class="sxs-lookup"><span data-stu-id="943e5-125">errorCode</span></span>|<span data-ttu-id="943e5-126">Int64</span><span class="sxs-lookup"><span data-stu-id="943e5-126">Int64</span></span>|<span data-ttu-id="943e5-127">Código de erro da configuração</span><span class="sxs-lookup"><span data-stu-id="943e5-127">Error code for the setting</span></span>|
|<span data-ttu-id="943e5-128">errorDescription</span><span class="sxs-lookup"><span data-stu-id="943e5-128">errorDescription</span></span>|<span data-ttu-id="943e5-129">String</span><span class="sxs-lookup"><span data-stu-id="943e5-129">String</span></span>|<span data-ttu-id="943e5-130">Descrição de erro</span><span class="sxs-lookup"><span data-stu-id="943e5-130">Error description</span></span>|
|<span data-ttu-id="943e5-131">userId</span><span class="sxs-lookup"><span data-stu-id="943e5-131">userId</span></span>|<span data-ttu-id="943e5-132">String</span><span class="sxs-lookup"><span data-stu-id="943e5-132">String</span></span>|<span data-ttu-id="943e5-133">UserId</span><span class="sxs-lookup"><span data-stu-id="943e5-133">UserId</span></span>|
|<span data-ttu-id="943e5-134">userName</span><span class="sxs-lookup"><span data-stu-id="943e5-134">userName</span></span>|<span data-ttu-id="943e5-135">String</span><span class="sxs-lookup"><span data-stu-id="943e5-135">String</span></span>|<span data-ttu-id="943e5-136">UserName</span><span class="sxs-lookup"><span data-stu-id="943e5-136">UserName</span></span>|
|<span data-ttu-id="943e5-137">userEmail</span><span class="sxs-lookup"><span data-stu-id="943e5-137">userEmail</span></span>|<span data-ttu-id="943e5-138">String</span><span class="sxs-lookup"><span data-stu-id="943e5-138">String</span></span>|<span data-ttu-id="943e5-139">UserEmail</span><span class="sxs-lookup"><span data-stu-id="943e5-139">UserEmail</span></span>|
|<span data-ttu-id="943e5-140">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="943e5-140">userPrincipalName</span></span>|<span data-ttu-id="943e5-141">String</span><span class="sxs-lookup"><span data-stu-id="943e5-141">String</span></span>|<span data-ttu-id="943e5-142">UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="943e5-142">UserPrincipalName.</span></span>|
|<span data-ttu-id="943e5-143">fontes</span><span class="sxs-lookup"><span data-stu-id="943e5-143">sources</span></span>|<span data-ttu-id="943e5-144">Conjunto [settingSource](../resources/intune-deviceconfig-settingsource.md)</span><span class="sxs-lookup"><span data-stu-id="943e5-144">[settingSource](../resources/intune-deviceconfig-settingsource.md) collection</span></span>|<span data-ttu-id="943e5-145">Políticas de colaboração</span><span class="sxs-lookup"><span data-stu-id="943e5-145">Contributing policies</span></span>|
|<span data-ttu-id="943e5-146">currentValue</span><span class="sxs-lookup"><span data-stu-id="943e5-146">currentValue</span></span>|<span data-ttu-id="943e5-147">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="943e5-147">String</span></span>|<span data-ttu-id="943e5-148">Valor atual da configuração em um dispositivo</span><span class="sxs-lookup"><span data-stu-id="943e5-148">Current value of setting on device</span></span>|

## <a name="relationships"></a><span data-ttu-id="943e5-149">Relações</span><span class="sxs-lookup"><span data-stu-id="943e5-149">Relationships</span></span>
<span data-ttu-id="943e5-150">Nenhum</span><span class="sxs-lookup"><span data-stu-id="943e5-150">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="943e5-151">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="943e5-151">JSON Representation</span></span>
<span data-ttu-id="943e5-152">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="943e5-152">Here is a JSON representation of the resource.</span></span>
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



