---
title: tipo de recurso deviceConfigurationSettingState
description: Estado da definição de configuração de um determinado dispositivo.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: c50ed17421b88f2cb6137458ff853bfa92796c2b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36031665"
---
# <a name="deviceconfigurationsettingstate-resource-type"></a><span data-ttu-id="ec26c-103">tipo de recurso deviceConfigurationSettingState</span><span class="sxs-lookup"><span data-stu-id="ec26c-103">deviceConfigurationSettingState resource type</span></span>

> <span data-ttu-id="ec26c-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ec26c-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ec26c-105">Estado da definição de configuração de um determinado dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ec26c-105">Device Configuration Setting State for a given device.</span></span>

## <a name="properties"></a><span data-ttu-id="ec26c-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ec26c-106">Properties</span></span>
|<span data-ttu-id="ec26c-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ec26c-107">Property</span></span>|<span data-ttu-id="ec26c-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="ec26c-108">Type</span></span>|<span data-ttu-id="ec26c-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="ec26c-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ec26c-110">configuração</span><span class="sxs-lookup"><span data-stu-id="ec26c-110">setting</span></span>|<span data-ttu-id="ec26c-111">String</span><span class="sxs-lookup"><span data-stu-id="ec26c-111">String</span></span>|<span data-ttu-id="ec26c-112">A configuração que é relatada</span><span class="sxs-lookup"><span data-stu-id="ec26c-112">The setting that is being reported</span></span>|
|<span data-ttu-id="ec26c-113">settingName</span><span class="sxs-lookup"><span data-stu-id="ec26c-113">settingName</span></span>|<span data-ttu-id="ec26c-114">String</span><span class="sxs-lookup"><span data-stu-id="ec26c-114">String</span></span>|<span data-ttu-id="ec26c-115">Nome de configuração localizada/de usuário que é relatada</span><span class="sxs-lookup"><span data-stu-id="ec26c-115">Localized/user friendly setting name that is being reported</span></span>|
|<span data-ttu-id="ec26c-116">instanceDisplayName</span><span class="sxs-lookup"><span data-stu-id="ec26c-116">instanceDisplayName</span></span>|<span data-ttu-id="ec26c-117">String</span><span class="sxs-lookup"><span data-stu-id="ec26c-117">String</span></span>|<span data-ttu-id="ec26c-118">Nome da instância de configuração que é relatada.</span><span class="sxs-lookup"><span data-stu-id="ec26c-118">Name of setting instance that is being reported.</span></span>|
|<span data-ttu-id="ec26c-119">state</span><span class="sxs-lookup"><span data-stu-id="ec26c-119">state</span></span>|[<span data-ttu-id="ec26c-120">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="ec26c-120">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="ec26c-121">O estado de conformidade da configuração.</span><span class="sxs-lookup"><span data-stu-id="ec26c-121">The compliance state of the setting.</span></span> <span data-ttu-id="ec26c-122">Os valores possíveis são: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="ec26c-122">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="ec26c-123">errorCode</span><span class="sxs-lookup"><span data-stu-id="ec26c-123">errorCode</span></span>|<span data-ttu-id="ec26c-124">Int64</span><span class="sxs-lookup"><span data-stu-id="ec26c-124">Int64</span></span>|<span data-ttu-id="ec26c-125">Código de erro da configuração</span><span class="sxs-lookup"><span data-stu-id="ec26c-125">Error code for the setting</span></span>|
|<span data-ttu-id="ec26c-126">errorDescription</span><span class="sxs-lookup"><span data-stu-id="ec26c-126">errorDescription</span></span>|<span data-ttu-id="ec26c-127">String</span><span class="sxs-lookup"><span data-stu-id="ec26c-127">String</span></span>|<span data-ttu-id="ec26c-128">Descrição de erro</span><span class="sxs-lookup"><span data-stu-id="ec26c-128">Error description</span></span>|
|<span data-ttu-id="ec26c-129">userId</span><span class="sxs-lookup"><span data-stu-id="ec26c-129">userId</span></span>|<span data-ttu-id="ec26c-130">String</span><span class="sxs-lookup"><span data-stu-id="ec26c-130">String</span></span>|<span data-ttu-id="ec26c-131">UserId</span><span class="sxs-lookup"><span data-stu-id="ec26c-131">UserId</span></span>|
|<span data-ttu-id="ec26c-132">userName</span><span class="sxs-lookup"><span data-stu-id="ec26c-132">userName</span></span>|<span data-ttu-id="ec26c-133">String</span><span class="sxs-lookup"><span data-stu-id="ec26c-133">String</span></span>|<span data-ttu-id="ec26c-134">UserName</span><span class="sxs-lookup"><span data-stu-id="ec26c-134">UserName</span></span>|
|<span data-ttu-id="ec26c-135">userEmail</span><span class="sxs-lookup"><span data-stu-id="ec26c-135">userEmail</span></span>|<span data-ttu-id="ec26c-136">String</span><span class="sxs-lookup"><span data-stu-id="ec26c-136">String</span></span>|<span data-ttu-id="ec26c-137">UserEmail</span><span class="sxs-lookup"><span data-stu-id="ec26c-137">UserEmail</span></span>|
|<span data-ttu-id="ec26c-138">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="ec26c-138">userPrincipalName</span></span>|<span data-ttu-id="ec26c-139">String</span><span class="sxs-lookup"><span data-stu-id="ec26c-139">String</span></span>|<span data-ttu-id="ec26c-140">UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="ec26c-140">UserPrincipalName.</span></span>|
|<span data-ttu-id="ec26c-141">fontes</span><span class="sxs-lookup"><span data-stu-id="ec26c-141">sources</span></span>|<span data-ttu-id="ec26c-142">Conjunto [settingSource](../resources/intune-deviceconfig-settingsource.md)</span><span class="sxs-lookup"><span data-stu-id="ec26c-142">[settingSource](../resources/intune-deviceconfig-settingsource.md) collection</span></span>|<span data-ttu-id="ec26c-143">Políticas de colaboração</span><span class="sxs-lookup"><span data-stu-id="ec26c-143">Contributing policies</span></span>|
|<span data-ttu-id="ec26c-144">currentValue</span><span class="sxs-lookup"><span data-stu-id="ec26c-144">currentValue</span></span>|<span data-ttu-id="ec26c-145">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ec26c-145">String</span></span>|<span data-ttu-id="ec26c-146">Valor atual da configuração em um dispositivo</span><span class="sxs-lookup"><span data-stu-id="ec26c-146">Current value of setting on device</span></span>|

## <a name="relationships"></a><span data-ttu-id="ec26c-147">Relações</span><span class="sxs-lookup"><span data-stu-id="ec26c-147">Relationships</span></span>
<span data-ttu-id="ec26c-148">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ec26c-148">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ec26c-149">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ec26c-149">JSON Representation</span></span>
<span data-ttu-id="ec26c-150">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ec26c-150">Here is a JSON representation of the resource.</span></span>
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



