---
title: tipo de recurso deviceConfigurationSettingState
description: Estado da definição de configuração de um determinado dispositivo.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 4601ba80d9ba4c67785848421e457107c7701159
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43469371"
---
# <a name="deviceconfigurationsettingstate-resource-type"></a><span data-ttu-id="1e5b2-103">tipo de recurso deviceConfigurationSettingState</span><span class="sxs-lookup"><span data-stu-id="1e5b2-103">deviceConfigurationSettingState resource type</span></span>

<span data-ttu-id="1e5b2-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1e5b2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1e5b2-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="1e5b2-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1e5b2-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1e5b2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1e5b2-107">Estado da definição de configuração de um determinado dispositivo.</span><span class="sxs-lookup"><span data-stu-id="1e5b2-107">Device Configuration Setting State for a given device.</span></span>

## <a name="properties"></a><span data-ttu-id="1e5b2-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1e5b2-108">Properties</span></span>
|<span data-ttu-id="1e5b2-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1e5b2-109">Property</span></span>|<span data-ttu-id="1e5b2-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="1e5b2-110">Type</span></span>|<span data-ttu-id="1e5b2-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="1e5b2-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1e5b2-112">configuração</span><span class="sxs-lookup"><span data-stu-id="1e5b2-112">setting</span></span>|<span data-ttu-id="1e5b2-113">String</span><span class="sxs-lookup"><span data-stu-id="1e5b2-113">String</span></span>|<span data-ttu-id="1e5b2-114">A configuração que é relatada</span><span class="sxs-lookup"><span data-stu-id="1e5b2-114">The setting that is being reported</span></span>|
|<span data-ttu-id="1e5b2-115">settingName</span><span class="sxs-lookup"><span data-stu-id="1e5b2-115">settingName</span></span>|<span data-ttu-id="1e5b2-116">String</span><span class="sxs-lookup"><span data-stu-id="1e5b2-116">String</span></span>|<span data-ttu-id="1e5b2-117">Nome de configuração localizada/de usuário que é relatada</span><span class="sxs-lookup"><span data-stu-id="1e5b2-117">Localized/user friendly setting name that is being reported</span></span>|
|<span data-ttu-id="1e5b2-118">instanceDisplayName</span><span class="sxs-lookup"><span data-stu-id="1e5b2-118">instanceDisplayName</span></span>|<span data-ttu-id="1e5b2-119">String</span><span class="sxs-lookup"><span data-stu-id="1e5b2-119">String</span></span>|<span data-ttu-id="1e5b2-120">Nome da instância de configuração que é relatada.</span><span class="sxs-lookup"><span data-stu-id="1e5b2-120">Name of setting instance that is being reported.</span></span>|
|<span data-ttu-id="1e5b2-121">state</span><span class="sxs-lookup"><span data-stu-id="1e5b2-121">state</span></span>|[<span data-ttu-id="1e5b2-122">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="1e5b2-122">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="1e5b2-123">O estado de conformidade da configuração.</span><span class="sxs-lookup"><span data-stu-id="1e5b2-123">The compliance state of the setting.</span></span> <span data-ttu-id="1e5b2-124">Os valores possíveis são: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="1e5b2-124">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="1e5b2-125">errorCode</span><span class="sxs-lookup"><span data-stu-id="1e5b2-125">errorCode</span></span>|<span data-ttu-id="1e5b2-126">Int64</span><span class="sxs-lookup"><span data-stu-id="1e5b2-126">Int64</span></span>|<span data-ttu-id="1e5b2-127">Código de erro da configuração</span><span class="sxs-lookup"><span data-stu-id="1e5b2-127">Error code for the setting</span></span>|
|<span data-ttu-id="1e5b2-128">errorDescription</span><span class="sxs-lookup"><span data-stu-id="1e5b2-128">errorDescription</span></span>|<span data-ttu-id="1e5b2-129">String</span><span class="sxs-lookup"><span data-stu-id="1e5b2-129">String</span></span>|<span data-ttu-id="1e5b2-130">Descrição de erro</span><span class="sxs-lookup"><span data-stu-id="1e5b2-130">Error description</span></span>|
|<span data-ttu-id="1e5b2-131">userId</span><span class="sxs-lookup"><span data-stu-id="1e5b2-131">userId</span></span>|<span data-ttu-id="1e5b2-132">String</span><span class="sxs-lookup"><span data-stu-id="1e5b2-132">String</span></span>|<span data-ttu-id="1e5b2-133">UserId</span><span class="sxs-lookup"><span data-stu-id="1e5b2-133">UserId</span></span>|
|<span data-ttu-id="1e5b2-134">userName</span><span class="sxs-lookup"><span data-stu-id="1e5b2-134">userName</span></span>|<span data-ttu-id="1e5b2-135">String</span><span class="sxs-lookup"><span data-stu-id="1e5b2-135">String</span></span>|<span data-ttu-id="1e5b2-136">UserName</span><span class="sxs-lookup"><span data-stu-id="1e5b2-136">UserName</span></span>|
|<span data-ttu-id="1e5b2-137">userEmail</span><span class="sxs-lookup"><span data-stu-id="1e5b2-137">userEmail</span></span>|<span data-ttu-id="1e5b2-138">String</span><span class="sxs-lookup"><span data-stu-id="1e5b2-138">String</span></span>|<span data-ttu-id="1e5b2-139">UserEmail</span><span class="sxs-lookup"><span data-stu-id="1e5b2-139">UserEmail</span></span>|
|<span data-ttu-id="1e5b2-140">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="1e5b2-140">userPrincipalName</span></span>|<span data-ttu-id="1e5b2-141">String</span><span class="sxs-lookup"><span data-stu-id="1e5b2-141">String</span></span>|<span data-ttu-id="1e5b2-142">UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="1e5b2-142">UserPrincipalName.</span></span>|
|<span data-ttu-id="1e5b2-143">fontes</span><span class="sxs-lookup"><span data-stu-id="1e5b2-143">sources</span></span>|<span data-ttu-id="1e5b2-144">Conjunto [settingSource](../resources/intune-deviceconfig-settingsource.md)</span><span class="sxs-lookup"><span data-stu-id="1e5b2-144">[settingSource](../resources/intune-deviceconfig-settingsource.md) collection</span></span>|<span data-ttu-id="1e5b2-145">Políticas de colaboração</span><span class="sxs-lookup"><span data-stu-id="1e5b2-145">Contributing policies</span></span>|
|<span data-ttu-id="1e5b2-146">currentValue</span><span class="sxs-lookup"><span data-stu-id="1e5b2-146">currentValue</span></span>|<span data-ttu-id="1e5b2-147">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1e5b2-147">String</span></span>|<span data-ttu-id="1e5b2-148">Valor atual da configuração em um dispositivo</span><span class="sxs-lookup"><span data-stu-id="1e5b2-148">Current value of setting on device</span></span>|
|<span data-ttu-id="1e5b2-149">settingInstanceId</span><span class="sxs-lookup"><span data-stu-id="1e5b2-149">settingInstanceId</span></span>|<span data-ttu-id="1e5b2-150">String</span><span class="sxs-lookup"><span data-stu-id="1e5b2-150">String</span></span>|<span data-ttu-id="1e5b2-151">SettingInstanceId</span><span class="sxs-lookup"><span data-stu-id="1e5b2-151">SettingInstanceId</span></span>|

## <a name="relationships"></a><span data-ttu-id="1e5b2-152">Relações</span><span class="sxs-lookup"><span data-stu-id="1e5b2-152">Relationships</span></span>
<span data-ttu-id="1e5b2-153">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1e5b2-153">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1e5b2-154">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1e5b2-154">JSON Representation</span></span>
<span data-ttu-id="1e5b2-155">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1e5b2-155">Here is a JSON representation of the resource.</span></span>
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
  "currentValue": "String",
  "settingInstanceId": "String"
}
```



