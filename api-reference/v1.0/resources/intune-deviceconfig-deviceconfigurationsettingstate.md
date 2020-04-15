---
title: tipo de recurso deviceConfigurationSettingState
description: Estado da definição de configuração de um determinado dispositivo.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 4b613ae365d0842079485171b41c7d37580a66b4
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43445975"
---
# <a name="deviceconfigurationsettingstate-resource-type"></a><span data-ttu-id="3743b-103">tipo de recurso deviceConfigurationSettingState</span><span class="sxs-lookup"><span data-stu-id="3743b-103">deviceConfigurationSettingState resource type</span></span>

<span data-ttu-id="3743b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3743b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3743b-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3743b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3743b-106">Estado da definição de configuração de um determinado dispositivo.</span><span class="sxs-lookup"><span data-stu-id="3743b-106">Device Configuration Setting State for a given device.</span></span>

## <a name="properties"></a><span data-ttu-id="3743b-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3743b-107">Properties</span></span>
|<span data-ttu-id="3743b-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3743b-108">Property</span></span>|<span data-ttu-id="3743b-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="3743b-109">Type</span></span>|<span data-ttu-id="3743b-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="3743b-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3743b-111">configuração</span><span class="sxs-lookup"><span data-stu-id="3743b-111">setting</span></span>|<span data-ttu-id="3743b-112">String</span><span class="sxs-lookup"><span data-stu-id="3743b-112">String</span></span>|<span data-ttu-id="3743b-113">A configuração que é relatada</span><span class="sxs-lookup"><span data-stu-id="3743b-113">The setting that is being reported</span></span>|
|<span data-ttu-id="3743b-114">settingName</span><span class="sxs-lookup"><span data-stu-id="3743b-114">settingName</span></span>|<span data-ttu-id="3743b-115">String</span><span class="sxs-lookup"><span data-stu-id="3743b-115">String</span></span>|<span data-ttu-id="3743b-116">Nome de configuração localizada/de usuário que é relatada</span><span class="sxs-lookup"><span data-stu-id="3743b-116">Localized/user friendly setting name that is being reported</span></span>|
|<span data-ttu-id="3743b-117">instanceDisplayName</span><span class="sxs-lookup"><span data-stu-id="3743b-117">instanceDisplayName</span></span>|<span data-ttu-id="3743b-118">String</span><span class="sxs-lookup"><span data-stu-id="3743b-118">String</span></span>|<span data-ttu-id="3743b-119">Nome da instância de configuração que é relatada.</span><span class="sxs-lookup"><span data-stu-id="3743b-119">Name of setting instance that is being reported.</span></span>|
|<span data-ttu-id="3743b-120">state</span><span class="sxs-lookup"><span data-stu-id="3743b-120">state</span></span>|[<span data-ttu-id="3743b-121">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="3743b-121">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="3743b-122">O estado de conformidade da configuração.</span><span class="sxs-lookup"><span data-stu-id="3743b-122">The compliance state of the setting.</span></span> <span data-ttu-id="3743b-123">Os valores possíveis são: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="3743b-123">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="3743b-124">errorCode</span><span class="sxs-lookup"><span data-stu-id="3743b-124">errorCode</span></span>|<span data-ttu-id="3743b-125">Int64</span><span class="sxs-lookup"><span data-stu-id="3743b-125">Int64</span></span>|<span data-ttu-id="3743b-126">Código de erro da configuração</span><span class="sxs-lookup"><span data-stu-id="3743b-126">Error code for the setting</span></span>|
|<span data-ttu-id="3743b-127">errorDescription</span><span class="sxs-lookup"><span data-stu-id="3743b-127">errorDescription</span></span>|<span data-ttu-id="3743b-128">String</span><span class="sxs-lookup"><span data-stu-id="3743b-128">String</span></span>|<span data-ttu-id="3743b-129">Descrição de erro</span><span class="sxs-lookup"><span data-stu-id="3743b-129">Error description</span></span>|
|<span data-ttu-id="3743b-130">userId</span><span class="sxs-lookup"><span data-stu-id="3743b-130">userId</span></span>|<span data-ttu-id="3743b-131">String</span><span class="sxs-lookup"><span data-stu-id="3743b-131">String</span></span>|<span data-ttu-id="3743b-132">UserId</span><span class="sxs-lookup"><span data-stu-id="3743b-132">UserId</span></span>|
|<span data-ttu-id="3743b-133">userName</span><span class="sxs-lookup"><span data-stu-id="3743b-133">userName</span></span>|<span data-ttu-id="3743b-134">String</span><span class="sxs-lookup"><span data-stu-id="3743b-134">String</span></span>|<span data-ttu-id="3743b-135">UserName</span><span class="sxs-lookup"><span data-stu-id="3743b-135">UserName</span></span>|
|<span data-ttu-id="3743b-136">userEmail</span><span class="sxs-lookup"><span data-stu-id="3743b-136">userEmail</span></span>|<span data-ttu-id="3743b-137">String</span><span class="sxs-lookup"><span data-stu-id="3743b-137">String</span></span>|<span data-ttu-id="3743b-138">UserEmail</span><span class="sxs-lookup"><span data-stu-id="3743b-138">UserEmail</span></span>|
|<span data-ttu-id="3743b-139">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="3743b-139">userPrincipalName</span></span>|<span data-ttu-id="3743b-140">String</span><span class="sxs-lookup"><span data-stu-id="3743b-140">String</span></span>|<span data-ttu-id="3743b-141">UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="3743b-141">UserPrincipalName.</span></span>|
|<span data-ttu-id="3743b-142">fontes</span><span class="sxs-lookup"><span data-stu-id="3743b-142">sources</span></span>|<span data-ttu-id="3743b-143">Conjunto [settingSource](../resources/intune-deviceconfig-settingsource.md)</span><span class="sxs-lookup"><span data-stu-id="3743b-143">[settingSource](../resources/intune-deviceconfig-settingsource.md) collection</span></span>|<span data-ttu-id="3743b-144">Políticas de colaboração</span><span class="sxs-lookup"><span data-stu-id="3743b-144">Contributing policies</span></span>|
|<span data-ttu-id="3743b-145">currentValue</span><span class="sxs-lookup"><span data-stu-id="3743b-145">currentValue</span></span>|<span data-ttu-id="3743b-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3743b-146">String</span></span>|<span data-ttu-id="3743b-147">Valor atual da configuração em um dispositivo</span><span class="sxs-lookup"><span data-stu-id="3743b-147">Current value of setting on device</span></span>|

## <a name="relationships"></a><span data-ttu-id="3743b-148">Relações</span><span class="sxs-lookup"><span data-stu-id="3743b-148">Relationships</span></span>
<span data-ttu-id="3743b-149">Nenhum</span><span class="sxs-lookup"><span data-stu-id="3743b-149">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3743b-150">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3743b-150">JSON Representation</span></span>
<span data-ttu-id="3743b-151">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3743b-151">Here is a JSON representation of the resource.</span></span>
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







