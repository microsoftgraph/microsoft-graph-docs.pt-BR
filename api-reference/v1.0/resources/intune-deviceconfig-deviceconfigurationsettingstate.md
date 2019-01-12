---
title: tipo de recurso deviceConfigurationSettingState
description: Estado da definição de configuração de um determinado dispositivo.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 68c57b8842136494bf0604a31f62992f7a1c2501
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27928007"
---
# <a name="deviceconfigurationsettingstate-resource-type"></a><span data-ttu-id="0457c-103">tipo de recurso deviceConfigurationSettingState</span><span class="sxs-lookup"><span data-stu-id="0457c-103">deviceConfigurationSettingState resource type</span></span>

> <span data-ttu-id="0457c-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="0457c-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0457c-105">Estado da definição de configuração de um determinado dispositivo.</span><span class="sxs-lookup"><span data-stu-id="0457c-105">Device Configuration Setting State for a given device.</span></span>
## <a name="properties"></a><span data-ttu-id="0457c-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0457c-106">Properties</span></span>
|<span data-ttu-id="0457c-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0457c-107">Property</span></span>|<span data-ttu-id="0457c-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="0457c-108">Type</span></span>|<span data-ttu-id="0457c-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="0457c-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0457c-110">configuração</span><span class="sxs-lookup"><span data-stu-id="0457c-110">setting</span></span>|<span data-ttu-id="0457c-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0457c-111">String</span></span>|<span data-ttu-id="0457c-112">A configuração que está sendo relatada</span><span class="sxs-lookup"><span data-stu-id="0457c-112">The setting that is being reported</span></span>|
|<span data-ttu-id="0457c-113">settingName</span><span class="sxs-lookup"><span data-stu-id="0457c-113">settingName</span></span>|<span data-ttu-id="0457c-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0457c-114">String</span></span>|<span data-ttu-id="0457c-115">Nome traduzido/amigável para o usuário da configuração que está sendo relatada</span><span class="sxs-lookup"><span data-stu-id="0457c-115">Localized/user friendly setting name that is being reported</span></span>|
|<span data-ttu-id="0457c-116">instanceDisplayName</span><span class="sxs-lookup"><span data-stu-id="0457c-116">instanceDisplayName</span></span>|<span data-ttu-id="0457c-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0457c-117">String</span></span>|<span data-ttu-id="0457c-118">Nome da instância de configuração está sendo relatada.</span><span class="sxs-lookup"><span data-stu-id="0457c-118">Name of setting instance that is being reported.</span></span>|
|<span data-ttu-id="0457c-119">estado</span><span class="sxs-lookup"><span data-stu-id="0457c-119">state</span></span>|[<span data-ttu-id="0457c-120">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="0457c-120">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="0457c-121">O estado de conformidade da configuração.</span><span class="sxs-lookup"><span data-stu-id="0457c-121">The compliance state of the setting.</span></span> <span data-ttu-id="0457c-122">Os valores possíveis são: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="0457c-122">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="0457c-123">errorCode</span><span class="sxs-lookup"><span data-stu-id="0457c-123">errorCode</span></span>|<span data-ttu-id="0457c-124">Int64</span><span class="sxs-lookup"><span data-stu-id="0457c-124">Int64</span></span>|<span data-ttu-id="0457c-125">Código de erro da configuração</span><span class="sxs-lookup"><span data-stu-id="0457c-125">Error code for the setting</span></span>|
|<span data-ttu-id="0457c-126">errorDescription</span><span class="sxs-lookup"><span data-stu-id="0457c-126">errorDescription</span></span>|<span data-ttu-id="0457c-127">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0457c-127">String</span></span>|<span data-ttu-id="0457c-128">Descrição do erro</span><span class="sxs-lookup"><span data-stu-id="0457c-128">Error description</span></span>|
|<span data-ttu-id="0457c-129">userId</span><span class="sxs-lookup"><span data-stu-id="0457c-129">userId</span></span>|<span data-ttu-id="0457c-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0457c-130">String</span></span>|<span data-ttu-id="0457c-131">UserId</span><span class="sxs-lookup"><span data-stu-id="0457c-131">UserId</span></span>|
|<span data-ttu-id="0457c-132">userName</span><span class="sxs-lookup"><span data-stu-id="0457c-132">userName</span></span>|<span data-ttu-id="0457c-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0457c-133">String</span></span>|<span data-ttu-id="0457c-134">UserName</span><span class="sxs-lookup"><span data-stu-id="0457c-134">UserName</span></span>|
|<span data-ttu-id="0457c-135">userEmail</span><span class="sxs-lookup"><span data-stu-id="0457c-135">userEmail</span></span>|<span data-ttu-id="0457c-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0457c-136">String</span></span>|<span data-ttu-id="0457c-137">UserEmail</span><span class="sxs-lookup"><span data-stu-id="0457c-137">UserEmail</span></span>|
|<span data-ttu-id="0457c-138">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="0457c-138">userPrincipalName</span></span>|<span data-ttu-id="0457c-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0457c-139">String</span></span>|<span data-ttu-id="0457c-140">UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="0457c-140">UserPrincipalName.</span></span>|
|<span data-ttu-id="0457c-141">sources</span><span class="sxs-lookup"><span data-stu-id="0457c-141">sources</span></span>|<span data-ttu-id="0457c-142">Coleção [settingSource](../resources/intune-deviceconfig-settingsource.md)</span><span class="sxs-lookup"><span data-stu-id="0457c-142">[settingSource](../resources/intune-deviceconfig-settingsource.md) collection</span></span>|<span data-ttu-id="0457c-143">Políticas colaboradoras</span><span class="sxs-lookup"><span data-stu-id="0457c-143">Contributing policies</span></span>|
|<span data-ttu-id="0457c-144">currentValue</span><span class="sxs-lookup"><span data-stu-id="0457c-144">currentValue</span></span>|<span data-ttu-id="0457c-145">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0457c-145">String</span></span>|<span data-ttu-id="0457c-146">Valor atual da configuração no dispositivo</span><span class="sxs-lookup"><span data-stu-id="0457c-146">Current value of setting on device</span></span>|

## <a name="relationships"></a><span data-ttu-id="0457c-147">Relações</span><span class="sxs-lookup"><span data-stu-id="0457c-147">Relationships</span></span>
<span data-ttu-id="0457c-148">Nenhum</span><span class="sxs-lookup"><span data-stu-id="0457c-148">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="0457c-149">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0457c-149">JSON Representation</span></span>
<span data-ttu-id="0457c-150">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0457c-150">Here is a JSON representation of the resource.</span></span>
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



