---
title: tipo de recurso deviceConfigurationSettingState
description: Estado da definição de configuração de um determinado dispositivo.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 6d5f75077fbfd29853b52adc6fc2d07b5c325905
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42526626"
---
# <a name="deviceconfigurationsettingstate-resource-type"></a><span data-ttu-id="860b8-103">tipo de recurso deviceConfigurationSettingState</span><span class="sxs-lookup"><span data-stu-id="860b8-103">deviceConfigurationSettingState resource type</span></span>

<span data-ttu-id="860b8-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="860b8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="860b8-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="860b8-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="860b8-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="860b8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="860b8-107">Estado da definição de configuração de um determinado dispositivo.</span><span class="sxs-lookup"><span data-stu-id="860b8-107">Device Configuration Setting State for a given device.</span></span>

## <a name="properties"></a><span data-ttu-id="860b8-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="860b8-108">Properties</span></span>
|<span data-ttu-id="860b8-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="860b8-109">Property</span></span>|<span data-ttu-id="860b8-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="860b8-110">Type</span></span>|<span data-ttu-id="860b8-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="860b8-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="860b8-112">configuração</span><span class="sxs-lookup"><span data-stu-id="860b8-112">setting</span></span>|<span data-ttu-id="860b8-113">String</span><span class="sxs-lookup"><span data-stu-id="860b8-113">String</span></span>|<span data-ttu-id="860b8-114">A configuração que é relatada</span><span class="sxs-lookup"><span data-stu-id="860b8-114">The setting that is being reported</span></span>|
|<span data-ttu-id="860b8-115">settingName</span><span class="sxs-lookup"><span data-stu-id="860b8-115">settingName</span></span>|<span data-ttu-id="860b8-116">String</span><span class="sxs-lookup"><span data-stu-id="860b8-116">String</span></span>|<span data-ttu-id="860b8-117">Nome de configuração localizada/de usuário que é relatada</span><span class="sxs-lookup"><span data-stu-id="860b8-117">Localized/user friendly setting name that is being reported</span></span>|
|<span data-ttu-id="860b8-118">instanceDisplayName</span><span class="sxs-lookup"><span data-stu-id="860b8-118">instanceDisplayName</span></span>|<span data-ttu-id="860b8-119">String</span><span class="sxs-lookup"><span data-stu-id="860b8-119">String</span></span>|<span data-ttu-id="860b8-120">Nome da instância de configuração que é relatada.</span><span class="sxs-lookup"><span data-stu-id="860b8-120">Name of setting instance that is being reported.</span></span>|
|<span data-ttu-id="860b8-121">state</span><span class="sxs-lookup"><span data-stu-id="860b8-121">state</span></span>|[<span data-ttu-id="860b8-122">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="860b8-122">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="860b8-123">O estado de conformidade da configuração.</span><span class="sxs-lookup"><span data-stu-id="860b8-123">The compliance state of the setting.</span></span> <span data-ttu-id="860b8-124">Os valores possíveis são: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="860b8-124">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="860b8-125">errorCode</span><span class="sxs-lookup"><span data-stu-id="860b8-125">errorCode</span></span>|<span data-ttu-id="860b8-126">Int64</span><span class="sxs-lookup"><span data-stu-id="860b8-126">Int64</span></span>|<span data-ttu-id="860b8-127">Código de erro da configuração</span><span class="sxs-lookup"><span data-stu-id="860b8-127">Error code for the setting</span></span>|
|<span data-ttu-id="860b8-128">errorDescription</span><span class="sxs-lookup"><span data-stu-id="860b8-128">errorDescription</span></span>|<span data-ttu-id="860b8-129">String</span><span class="sxs-lookup"><span data-stu-id="860b8-129">String</span></span>|<span data-ttu-id="860b8-130">Descrição de erro</span><span class="sxs-lookup"><span data-stu-id="860b8-130">Error description</span></span>|
|<span data-ttu-id="860b8-131">userId</span><span class="sxs-lookup"><span data-stu-id="860b8-131">userId</span></span>|<span data-ttu-id="860b8-132">String</span><span class="sxs-lookup"><span data-stu-id="860b8-132">String</span></span>|<span data-ttu-id="860b8-133">UserId</span><span class="sxs-lookup"><span data-stu-id="860b8-133">UserId</span></span>|
|<span data-ttu-id="860b8-134">userName</span><span class="sxs-lookup"><span data-stu-id="860b8-134">userName</span></span>|<span data-ttu-id="860b8-135">String</span><span class="sxs-lookup"><span data-stu-id="860b8-135">String</span></span>|<span data-ttu-id="860b8-136">UserName</span><span class="sxs-lookup"><span data-stu-id="860b8-136">UserName</span></span>|
|<span data-ttu-id="860b8-137">userEmail</span><span class="sxs-lookup"><span data-stu-id="860b8-137">userEmail</span></span>|<span data-ttu-id="860b8-138">String</span><span class="sxs-lookup"><span data-stu-id="860b8-138">String</span></span>|<span data-ttu-id="860b8-139">UserEmail</span><span class="sxs-lookup"><span data-stu-id="860b8-139">UserEmail</span></span>|
|<span data-ttu-id="860b8-140">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="860b8-140">userPrincipalName</span></span>|<span data-ttu-id="860b8-141">String</span><span class="sxs-lookup"><span data-stu-id="860b8-141">String</span></span>|<span data-ttu-id="860b8-142">UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="860b8-142">UserPrincipalName.</span></span>|
|<span data-ttu-id="860b8-143">fontes</span><span class="sxs-lookup"><span data-stu-id="860b8-143">sources</span></span>|<span data-ttu-id="860b8-144">Conjunto [settingSource](../resources/intune-deviceconfig-settingsource.md)</span><span class="sxs-lookup"><span data-stu-id="860b8-144">[settingSource](../resources/intune-deviceconfig-settingsource.md) collection</span></span>|<span data-ttu-id="860b8-145">Políticas de colaboração</span><span class="sxs-lookup"><span data-stu-id="860b8-145">Contributing policies</span></span>|
|<span data-ttu-id="860b8-146">currentValue</span><span class="sxs-lookup"><span data-stu-id="860b8-146">currentValue</span></span>|<span data-ttu-id="860b8-147">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="860b8-147">String</span></span>|<span data-ttu-id="860b8-148">Valor atual da configuração em um dispositivo</span><span class="sxs-lookup"><span data-stu-id="860b8-148">Current value of setting on device</span></span>|

## <a name="relationships"></a><span data-ttu-id="860b8-149">Relações</span><span class="sxs-lookup"><span data-stu-id="860b8-149">Relationships</span></span>
<span data-ttu-id="860b8-150">Nenhum</span><span class="sxs-lookup"><span data-stu-id="860b8-150">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="860b8-151">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="860b8-151">JSON Representation</span></span>
<span data-ttu-id="860b8-152">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="860b8-152">Here is a JSON representation of the resource.</span></span>
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



