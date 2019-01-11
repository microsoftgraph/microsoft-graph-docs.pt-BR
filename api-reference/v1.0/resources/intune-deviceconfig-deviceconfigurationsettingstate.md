---
title: tipo de recurso deviceConfigurationSettingState
description: Estado da definição de configuração de um determinado dispositivo.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: beed55d68c3ef7005a307d75fc1ee58ea78ed8d6
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27845840"
---
# <a name="deviceconfigurationsettingstate-resource-type"></a><span data-ttu-id="7a434-103">tipo de recurso deviceConfigurationSettingState</span><span class="sxs-lookup"><span data-stu-id="7a434-103">deviceConfigurationSettingState resource type</span></span>

> <span data-ttu-id="7a434-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="7a434-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7a434-105">Estado da definição de configuração de um determinado dispositivo.</span><span class="sxs-lookup"><span data-stu-id="7a434-105">Device Configuration Setting State for a given device.</span></span>
## <a name="properties"></a><span data-ttu-id="7a434-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7a434-106">Properties</span></span>
|<span data-ttu-id="7a434-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7a434-107">Property</span></span>|<span data-ttu-id="7a434-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="7a434-108">Type</span></span>|<span data-ttu-id="7a434-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="7a434-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7a434-110">configuração</span><span class="sxs-lookup"><span data-stu-id="7a434-110">setting</span></span>|<span data-ttu-id="7a434-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7a434-111">String</span></span>|<span data-ttu-id="7a434-112">A configuração que está sendo relatada</span><span class="sxs-lookup"><span data-stu-id="7a434-112">The setting that is being reported</span></span>|
|<span data-ttu-id="7a434-113">settingName</span><span class="sxs-lookup"><span data-stu-id="7a434-113">settingName</span></span>|<span data-ttu-id="7a434-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7a434-114">String</span></span>|<span data-ttu-id="7a434-115">Nome traduzido/amigável para o usuário da configuração que está sendo relatada</span><span class="sxs-lookup"><span data-stu-id="7a434-115">Localized/user friendly setting name that is being reported</span></span>|
|<span data-ttu-id="7a434-116">instanceDisplayName</span><span class="sxs-lookup"><span data-stu-id="7a434-116">instanceDisplayName</span></span>|<span data-ttu-id="7a434-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7a434-117">String</span></span>|<span data-ttu-id="7a434-118">Nome da instância de configuração está sendo relatada.</span><span class="sxs-lookup"><span data-stu-id="7a434-118">Name of setting instance that is being reported.</span></span>|
|<span data-ttu-id="7a434-119">estado</span><span class="sxs-lookup"><span data-stu-id="7a434-119">state</span></span>|[<span data-ttu-id="7a434-120">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="7a434-120">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="7a434-121">O estado de conformidade da configuração.</span><span class="sxs-lookup"><span data-stu-id="7a434-121">The compliance state of the setting.</span></span> <span data-ttu-id="7a434-122">Os valores possíveis são: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="7a434-122">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="7a434-123">errorCode</span><span class="sxs-lookup"><span data-stu-id="7a434-123">errorCode</span></span>|<span data-ttu-id="7a434-124">Int64</span><span class="sxs-lookup"><span data-stu-id="7a434-124">Int64</span></span>|<span data-ttu-id="7a434-125">Código de erro da configuração</span><span class="sxs-lookup"><span data-stu-id="7a434-125">Error code for the setting</span></span>|
|<span data-ttu-id="7a434-126">errorDescription</span><span class="sxs-lookup"><span data-stu-id="7a434-126">errorDescription</span></span>|<span data-ttu-id="7a434-127">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7a434-127">String</span></span>|<span data-ttu-id="7a434-128">Descrição do erro</span><span class="sxs-lookup"><span data-stu-id="7a434-128">Error description</span></span>|
|<span data-ttu-id="7a434-129">userId</span><span class="sxs-lookup"><span data-stu-id="7a434-129">userId</span></span>|<span data-ttu-id="7a434-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7a434-130">String</span></span>|<span data-ttu-id="7a434-131">UserId</span><span class="sxs-lookup"><span data-stu-id="7a434-131">UserId</span></span>|
|<span data-ttu-id="7a434-132">userName</span><span class="sxs-lookup"><span data-stu-id="7a434-132">userName</span></span>|<span data-ttu-id="7a434-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7a434-133">String</span></span>|<span data-ttu-id="7a434-134">UserName</span><span class="sxs-lookup"><span data-stu-id="7a434-134">UserName</span></span>|
|<span data-ttu-id="7a434-135">userEmail</span><span class="sxs-lookup"><span data-stu-id="7a434-135">userEmail</span></span>|<span data-ttu-id="7a434-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7a434-136">String</span></span>|<span data-ttu-id="7a434-137">UserEmail</span><span class="sxs-lookup"><span data-stu-id="7a434-137">UserEmail</span></span>|
|<span data-ttu-id="7a434-138">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="7a434-138">userPrincipalName</span></span>|<span data-ttu-id="7a434-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7a434-139">String</span></span>|<span data-ttu-id="7a434-140">UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="7a434-140">UserPrincipalName.</span></span>|
|<span data-ttu-id="7a434-141">sources</span><span class="sxs-lookup"><span data-stu-id="7a434-141">sources</span></span>|<span data-ttu-id="7a434-142">Coleção [settingSource](../resources/intune-deviceconfig-settingsource.md)</span><span class="sxs-lookup"><span data-stu-id="7a434-142">[settingSource](../resources/intune-deviceconfig-settingsource.md) collection</span></span>|<span data-ttu-id="7a434-143">Políticas colaboradoras</span><span class="sxs-lookup"><span data-stu-id="7a434-143">Contributing policies</span></span>|
|<span data-ttu-id="7a434-144">currentValue</span><span class="sxs-lookup"><span data-stu-id="7a434-144">currentValue</span></span>|<span data-ttu-id="7a434-145">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7a434-145">String</span></span>|<span data-ttu-id="7a434-146">Valor atual da configuração no dispositivo</span><span class="sxs-lookup"><span data-stu-id="7a434-146">Current value of setting on device</span></span>|

## <a name="relationships"></a><span data-ttu-id="7a434-147">Relações</span><span class="sxs-lookup"><span data-stu-id="7a434-147">Relationships</span></span>
<span data-ttu-id="7a434-148">Nenhum</span><span class="sxs-lookup"><span data-stu-id="7a434-148">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="7a434-149">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7a434-149">JSON Representation</span></span>
<span data-ttu-id="7a434-150">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7a434-150">Here is a JSON representation of the resource.</span></span>
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



