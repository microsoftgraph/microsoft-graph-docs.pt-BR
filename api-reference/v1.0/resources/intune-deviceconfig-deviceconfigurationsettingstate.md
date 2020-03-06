---
title: tipo de recurso deviceConfigurationSettingState
description: Estado da definição de configuração de um determinado dispositivo.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: aafa0147bac2acfcaa1f77291be1451c907b2f72
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42530765"
---
# <a name="deviceconfigurationsettingstate-resource-type"></a><span data-ttu-id="0c324-103">tipo de recurso deviceConfigurationSettingState</span><span class="sxs-lookup"><span data-stu-id="0c324-103">deviceConfigurationSettingState resource type</span></span>

<span data-ttu-id="0c324-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0c324-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0c324-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0c324-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0c324-106">Estado da definição de configuração de um determinado dispositivo.</span><span class="sxs-lookup"><span data-stu-id="0c324-106">Device Configuration Setting State for a given device.</span></span>

## <a name="properties"></a><span data-ttu-id="0c324-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0c324-107">Properties</span></span>
|<span data-ttu-id="0c324-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0c324-108">Property</span></span>|<span data-ttu-id="0c324-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="0c324-109">Type</span></span>|<span data-ttu-id="0c324-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="0c324-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0c324-111">configuração</span><span class="sxs-lookup"><span data-stu-id="0c324-111">setting</span></span>|<span data-ttu-id="0c324-112">String</span><span class="sxs-lookup"><span data-stu-id="0c324-112">String</span></span>|<span data-ttu-id="0c324-113">A configuração que é relatada</span><span class="sxs-lookup"><span data-stu-id="0c324-113">The setting that is being reported</span></span>|
|<span data-ttu-id="0c324-114">settingName</span><span class="sxs-lookup"><span data-stu-id="0c324-114">settingName</span></span>|<span data-ttu-id="0c324-115">String</span><span class="sxs-lookup"><span data-stu-id="0c324-115">String</span></span>|<span data-ttu-id="0c324-116">Nome de configuração localizada/de usuário que é relatada</span><span class="sxs-lookup"><span data-stu-id="0c324-116">Localized/user friendly setting name that is being reported</span></span>|
|<span data-ttu-id="0c324-117">instanceDisplayName</span><span class="sxs-lookup"><span data-stu-id="0c324-117">instanceDisplayName</span></span>|<span data-ttu-id="0c324-118">String</span><span class="sxs-lookup"><span data-stu-id="0c324-118">String</span></span>|<span data-ttu-id="0c324-119">Nome da instância de configuração que é relatada.</span><span class="sxs-lookup"><span data-stu-id="0c324-119">Name of setting instance that is being reported.</span></span>|
|<span data-ttu-id="0c324-120">state</span><span class="sxs-lookup"><span data-stu-id="0c324-120">state</span></span>|[<span data-ttu-id="0c324-121">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="0c324-121">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="0c324-122">O estado de conformidade da configuração.</span><span class="sxs-lookup"><span data-stu-id="0c324-122">The compliance state of the setting.</span></span> <span data-ttu-id="0c324-123">Os valores possíveis são: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="0c324-123">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="0c324-124">errorCode</span><span class="sxs-lookup"><span data-stu-id="0c324-124">errorCode</span></span>|<span data-ttu-id="0c324-125">Int64</span><span class="sxs-lookup"><span data-stu-id="0c324-125">Int64</span></span>|<span data-ttu-id="0c324-126">Código de erro da configuração</span><span class="sxs-lookup"><span data-stu-id="0c324-126">Error code for the setting</span></span>|
|<span data-ttu-id="0c324-127">errorDescription</span><span class="sxs-lookup"><span data-stu-id="0c324-127">errorDescription</span></span>|<span data-ttu-id="0c324-128">String</span><span class="sxs-lookup"><span data-stu-id="0c324-128">String</span></span>|<span data-ttu-id="0c324-129">Descrição de erro</span><span class="sxs-lookup"><span data-stu-id="0c324-129">Error description</span></span>|
|<span data-ttu-id="0c324-130">userId</span><span class="sxs-lookup"><span data-stu-id="0c324-130">userId</span></span>|<span data-ttu-id="0c324-131">String</span><span class="sxs-lookup"><span data-stu-id="0c324-131">String</span></span>|<span data-ttu-id="0c324-132">UserId</span><span class="sxs-lookup"><span data-stu-id="0c324-132">UserId</span></span>|
|<span data-ttu-id="0c324-133">userName</span><span class="sxs-lookup"><span data-stu-id="0c324-133">userName</span></span>|<span data-ttu-id="0c324-134">String</span><span class="sxs-lookup"><span data-stu-id="0c324-134">String</span></span>|<span data-ttu-id="0c324-135">UserName</span><span class="sxs-lookup"><span data-stu-id="0c324-135">UserName</span></span>|
|<span data-ttu-id="0c324-136">userEmail</span><span class="sxs-lookup"><span data-stu-id="0c324-136">userEmail</span></span>|<span data-ttu-id="0c324-137">String</span><span class="sxs-lookup"><span data-stu-id="0c324-137">String</span></span>|<span data-ttu-id="0c324-138">UserEmail</span><span class="sxs-lookup"><span data-stu-id="0c324-138">UserEmail</span></span>|
|<span data-ttu-id="0c324-139">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="0c324-139">userPrincipalName</span></span>|<span data-ttu-id="0c324-140">String</span><span class="sxs-lookup"><span data-stu-id="0c324-140">String</span></span>|<span data-ttu-id="0c324-141">UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="0c324-141">UserPrincipalName.</span></span>|
|<span data-ttu-id="0c324-142">fontes</span><span class="sxs-lookup"><span data-stu-id="0c324-142">sources</span></span>|<span data-ttu-id="0c324-143">Conjunto [settingSource](../resources/intune-deviceconfig-settingsource.md)</span><span class="sxs-lookup"><span data-stu-id="0c324-143">[settingSource](../resources/intune-deviceconfig-settingsource.md) collection</span></span>|<span data-ttu-id="0c324-144">Políticas de colaboração</span><span class="sxs-lookup"><span data-stu-id="0c324-144">Contributing policies</span></span>|
|<span data-ttu-id="0c324-145">currentValue</span><span class="sxs-lookup"><span data-stu-id="0c324-145">currentValue</span></span>|<span data-ttu-id="0c324-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0c324-146">String</span></span>|<span data-ttu-id="0c324-147">Valor atual da configuração em um dispositivo</span><span class="sxs-lookup"><span data-stu-id="0c324-147">Current value of setting on device</span></span>|

## <a name="relationships"></a><span data-ttu-id="0c324-148">Relações</span><span class="sxs-lookup"><span data-stu-id="0c324-148">Relationships</span></span>
<span data-ttu-id="0c324-149">Nenhum</span><span class="sxs-lookup"><span data-stu-id="0c324-149">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0c324-150">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0c324-150">JSON Representation</span></span>
<span data-ttu-id="0c324-151">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0c324-151">Here is a JSON representation of the resource.</span></span>
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




