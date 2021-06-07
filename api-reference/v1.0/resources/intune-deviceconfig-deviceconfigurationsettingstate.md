---
title: tipo de recurso deviceConfigurationSettingState
description: Estado da definição de configuração de um determinado dispositivo.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 4cb43529217ef6c129d06548e37800a501fcef55
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52757798"
---
# <a name="deviceconfigurationsettingstate-resource-type"></a><span data-ttu-id="5f098-103">tipo de recurso deviceConfigurationSettingState</span><span class="sxs-lookup"><span data-stu-id="5f098-103">deviceConfigurationSettingState resource type</span></span>

<span data-ttu-id="5f098-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5f098-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5f098-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="5f098-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5f098-106">Estado da definição de configuração de um determinado dispositivo.</span><span class="sxs-lookup"><span data-stu-id="5f098-106">Device Configuration Setting State for a given device.</span></span>

## <a name="properties"></a><span data-ttu-id="5f098-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5f098-107">Properties</span></span>
|<span data-ttu-id="5f098-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5f098-108">Property</span></span>|<span data-ttu-id="5f098-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="5f098-109">Type</span></span>|<span data-ttu-id="5f098-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="5f098-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5f098-111">configuração</span><span class="sxs-lookup"><span data-stu-id="5f098-111">setting</span></span>|<span data-ttu-id="5f098-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5f098-112">String</span></span>|<span data-ttu-id="5f098-113">A configuração que é relatada</span><span class="sxs-lookup"><span data-stu-id="5f098-113">The setting that is being reported</span></span>|
|<span data-ttu-id="5f098-114">settingName</span><span class="sxs-lookup"><span data-stu-id="5f098-114">settingName</span></span>|<span data-ttu-id="5f098-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5f098-115">String</span></span>|<span data-ttu-id="5f098-116">Nome de configuração localizada/de usuário que é relatada</span><span class="sxs-lookup"><span data-stu-id="5f098-116">Localized/user friendly setting name that is being reported</span></span>|
|<span data-ttu-id="5f098-117">instanceDisplayName</span><span class="sxs-lookup"><span data-stu-id="5f098-117">instanceDisplayName</span></span>|<span data-ttu-id="5f098-118">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5f098-118">String</span></span>|<span data-ttu-id="5f098-119">Nome da instância de configuração que é relatada.</span><span class="sxs-lookup"><span data-stu-id="5f098-119">Name of setting instance that is being reported.</span></span>|
|<span data-ttu-id="5f098-120">state</span><span class="sxs-lookup"><span data-stu-id="5f098-120">state</span></span>|[<span data-ttu-id="5f098-121">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="5f098-121">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="5f098-122">O estado de conformidade da configuração.</span><span class="sxs-lookup"><span data-stu-id="5f098-122">The compliance state of the setting.</span></span> <span data-ttu-id="5f098-123">Os valores possíveis são: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="5f098-123">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="5f098-124">errorCode</span><span class="sxs-lookup"><span data-stu-id="5f098-124">errorCode</span></span>|<span data-ttu-id="5f098-125">Int64</span><span class="sxs-lookup"><span data-stu-id="5f098-125">Int64</span></span>|<span data-ttu-id="5f098-126">Código de erro da configuração</span><span class="sxs-lookup"><span data-stu-id="5f098-126">Error code for the setting</span></span>|
|<span data-ttu-id="5f098-127">errorDescription</span><span class="sxs-lookup"><span data-stu-id="5f098-127">errorDescription</span></span>|<span data-ttu-id="5f098-128">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5f098-128">String</span></span>|<span data-ttu-id="5f098-129">Descrição de erro</span><span class="sxs-lookup"><span data-stu-id="5f098-129">Error description</span></span>|
|<span data-ttu-id="5f098-130">userId</span><span class="sxs-lookup"><span data-stu-id="5f098-130">userId</span></span>|<span data-ttu-id="5f098-131">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5f098-131">String</span></span>|<span data-ttu-id="5f098-132">UserId</span><span class="sxs-lookup"><span data-stu-id="5f098-132">UserId</span></span>|
|<span data-ttu-id="5f098-133">userName</span><span class="sxs-lookup"><span data-stu-id="5f098-133">userName</span></span>|<span data-ttu-id="5f098-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5f098-134">String</span></span>|<span data-ttu-id="5f098-135">UserName</span><span class="sxs-lookup"><span data-stu-id="5f098-135">UserName</span></span>|
|<span data-ttu-id="5f098-136">userEmail</span><span class="sxs-lookup"><span data-stu-id="5f098-136">userEmail</span></span>|<span data-ttu-id="5f098-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5f098-137">String</span></span>|<span data-ttu-id="5f098-138">UserEmail</span><span class="sxs-lookup"><span data-stu-id="5f098-138">UserEmail</span></span>|
|<span data-ttu-id="5f098-139">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="5f098-139">userPrincipalName</span></span>|<span data-ttu-id="5f098-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5f098-140">String</span></span>|<span data-ttu-id="5f098-141">UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="5f098-141">UserPrincipalName.</span></span>|
|<span data-ttu-id="5f098-142">fontes</span><span class="sxs-lookup"><span data-stu-id="5f098-142">sources</span></span>|<span data-ttu-id="5f098-143">Conjunto [settingSource](../resources/intune-deviceconfig-settingsource.md)</span><span class="sxs-lookup"><span data-stu-id="5f098-143">[settingSource](../resources/intune-deviceconfig-settingsource.md) collection</span></span>|<span data-ttu-id="5f098-144">Políticas de colaboração</span><span class="sxs-lookup"><span data-stu-id="5f098-144">Contributing policies</span></span>|
|<span data-ttu-id="5f098-145">currentValue</span><span class="sxs-lookup"><span data-stu-id="5f098-145">currentValue</span></span>|<span data-ttu-id="5f098-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5f098-146">String</span></span>|<span data-ttu-id="5f098-147">Valor atual da configuração em um dispositivo</span><span class="sxs-lookup"><span data-stu-id="5f098-147">Current value of setting on device</span></span>|

## <a name="relationships"></a><span data-ttu-id="5f098-148">Relações</span><span class="sxs-lookup"><span data-stu-id="5f098-148">Relationships</span></span>
<span data-ttu-id="5f098-149">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="5f098-149">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5f098-150">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5f098-150">JSON Representation</span></span>
<span data-ttu-id="5f098-151">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="5f098-151">Here is a JSON representation of the resource.</span></span>
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
      "displayName": "String",
      "sourceType": "String"
    }
  ],
  "currentValue": "String"
}
```




