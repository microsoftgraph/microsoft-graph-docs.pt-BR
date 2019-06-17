---
title: tipo de recurso deviceConfigurationSettingState
description: Estado da definição de configuração de um determinado dispositivo.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3e5c62cbd5ef1daa3adf0ba03931bc65b2b6d9b2
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34995949"
---
# <a name="deviceconfigurationsettingstate-resource-type"></a><span data-ttu-id="199db-103">tipo de recurso deviceConfigurationSettingState</span><span class="sxs-lookup"><span data-stu-id="199db-103">deviceConfigurationSettingState resource type</span></span>

> <span data-ttu-id="199db-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="199db-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="199db-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="199db-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="199db-106">Estado da definição de configuração de um determinado dispositivo.</span><span class="sxs-lookup"><span data-stu-id="199db-106">Device Configuration Setting State for a given device.</span></span>

## <a name="properties"></a><span data-ttu-id="199db-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="199db-107">Properties</span></span>
|<span data-ttu-id="199db-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="199db-108">Property</span></span>|<span data-ttu-id="199db-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="199db-109">Type</span></span>|<span data-ttu-id="199db-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="199db-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="199db-111">configuração</span><span class="sxs-lookup"><span data-stu-id="199db-111">setting</span></span>|<span data-ttu-id="199db-112">String</span><span class="sxs-lookup"><span data-stu-id="199db-112">String</span></span>|<span data-ttu-id="199db-113">A configuração que é relatada</span><span class="sxs-lookup"><span data-stu-id="199db-113">The setting that is being reported</span></span>|
|<span data-ttu-id="199db-114">settingName</span><span class="sxs-lookup"><span data-stu-id="199db-114">settingName</span></span>|<span data-ttu-id="199db-115">String</span><span class="sxs-lookup"><span data-stu-id="199db-115">String</span></span>|<span data-ttu-id="199db-116">Nome de configuração localizada/de usuário que é relatada</span><span class="sxs-lookup"><span data-stu-id="199db-116">Localized/user friendly setting name that is being reported</span></span>|
|<span data-ttu-id="199db-117">instanceDisplayName</span><span class="sxs-lookup"><span data-stu-id="199db-117">instanceDisplayName</span></span>|<span data-ttu-id="199db-118">String</span><span class="sxs-lookup"><span data-stu-id="199db-118">String</span></span>|<span data-ttu-id="199db-119">Nome da instância de configuração que é relatada.</span><span class="sxs-lookup"><span data-stu-id="199db-119">Name of setting instance that is being reported.</span></span>|
|<span data-ttu-id="199db-120">state</span><span class="sxs-lookup"><span data-stu-id="199db-120">state</span></span>|[<span data-ttu-id="199db-121">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="199db-121">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="199db-122">O estado de conformidade da configuração.</span><span class="sxs-lookup"><span data-stu-id="199db-122">The compliance state of the setting.</span></span> <span data-ttu-id="199db-123">Os valores possíveis são: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="199db-123">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="199db-124">errorCode</span><span class="sxs-lookup"><span data-stu-id="199db-124">errorCode</span></span>|<span data-ttu-id="199db-125">Int64</span><span class="sxs-lookup"><span data-stu-id="199db-125">Int64</span></span>|<span data-ttu-id="199db-126">Código de erro da configuração</span><span class="sxs-lookup"><span data-stu-id="199db-126">Error code for the setting</span></span>|
|<span data-ttu-id="199db-127">errorDescription</span><span class="sxs-lookup"><span data-stu-id="199db-127">errorDescription</span></span>|<span data-ttu-id="199db-128">String</span><span class="sxs-lookup"><span data-stu-id="199db-128">String</span></span>|<span data-ttu-id="199db-129">Descrição de erro</span><span class="sxs-lookup"><span data-stu-id="199db-129">Error description</span></span>|
|<span data-ttu-id="199db-130">userId</span><span class="sxs-lookup"><span data-stu-id="199db-130">userId</span></span>|<span data-ttu-id="199db-131">String</span><span class="sxs-lookup"><span data-stu-id="199db-131">String</span></span>|<span data-ttu-id="199db-132">UserId</span><span class="sxs-lookup"><span data-stu-id="199db-132">UserId</span></span>|
|<span data-ttu-id="199db-133">userName</span><span class="sxs-lookup"><span data-stu-id="199db-133">userName</span></span>|<span data-ttu-id="199db-134">String</span><span class="sxs-lookup"><span data-stu-id="199db-134">String</span></span>|<span data-ttu-id="199db-135">UserName</span><span class="sxs-lookup"><span data-stu-id="199db-135">UserName</span></span>|
|<span data-ttu-id="199db-136">userEmail</span><span class="sxs-lookup"><span data-stu-id="199db-136">userEmail</span></span>|<span data-ttu-id="199db-137">String</span><span class="sxs-lookup"><span data-stu-id="199db-137">String</span></span>|<span data-ttu-id="199db-138">UserEmail</span><span class="sxs-lookup"><span data-stu-id="199db-138">UserEmail</span></span>|
|<span data-ttu-id="199db-139">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="199db-139">userPrincipalName</span></span>|<span data-ttu-id="199db-140">String</span><span class="sxs-lookup"><span data-stu-id="199db-140">String</span></span>|<span data-ttu-id="199db-141">UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="199db-141">UserPrincipalName.</span></span>|
|<span data-ttu-id="199db-142">fontes</span><span class="sxs-lookup"><span data-stu-id="199db-142">sources</span></span>|<span data-ttu-id="199db-143">Conjunto [settingSource](../resources/intune-deviceconfig-settingsource.md)</span><span class="sxs-lookup"><span data-stu-id="199db-143">[settingSource](../resources/intune-deviceconfig-settingsource.md) collection</span></span>|<span data-ttu-id="199db-144">Políticas de colaboração</span><span class="sxs-lookup"><span data-stu-id="199db-144">Contributing policies</span></span>|
|<span data-ttu-id="199db-145">currentValue</span><span class="sxs-lookup"><span data-stu-id="199db-145">currentValue</span></span>|<span data-ttu-id="199db-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="199db-146">String</span></span>|<span data-ttu-id="199db-147">Valor atual da configuração em um dispositivo</span><span class="sxs-lookup"><span data-stu-id="199db-147">Current value of setting on device</span></span>|

## <a name="relationships"></a><span data-ttu-id="199db-148">Relações</span><span class="sxs-lookup"><span data-stu-id="199db-148">Relationships</span></span>
<span data-ttu-id="199db-149">Nenhum</span><span class="sxs-lookup"><span data-stu-id="199db-149">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="199db-150">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="199db-150">JSON Representation</span></span>
<span data-ttu-id="199db-151">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="199db-151">Here is a JSON representation of the resource.</span></span>
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





