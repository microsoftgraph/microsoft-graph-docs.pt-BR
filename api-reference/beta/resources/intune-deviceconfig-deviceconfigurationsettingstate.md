---
title: tipo de recurso deviceConfigurationSettingState
description: Estado da definição de configuração de um determinado dispositivo.
author: tfitzmac
ms.openlocfilehash: 7ca50fe6a6186578739b166b1239a309824d1e51
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27316111"
---
# <a name="deviceconfigurationsettingstate-resource-type"></a><span data-ttu-id="7362e-103">tipo de recurso deviceConfigurationSettingState</span><span class="sxs-lookup"><span data-stu-id="7362e-103">deviceConfigurationSettingState resource type</span></span>

> <span data-ttu-id="7362e-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="7362e-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7362e-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="7362e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7362e-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="7362e-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7362e-107">Estado da definição de configuração de um determinado dispositivo.</span><span class="sxs-lookup"><span data-stu-id="7362e-107">Device Configuration Setting State for a given device.</span></span>
## <a name="properties"></a><span data-ttu-id="7362e-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7362e-108">Properties</span></span>
|<span data-ttu-id="7362e-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7362e-109">Property</span></span>|<span data-ttu-id="7362e-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="7362e-110">Type</span></span>|<span data-ttu-id="7362e-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="7362e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7362e-112">configuração</span><span class="sxs-lookup"><span data-stu-id="7362e-112">setting</span></span>|<span data-ttu-id="7362e-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7362e-113">String</span></span>|<span data-ttu-id="7362e-114">A configuração que está sendo relatada</span><span class="sxs-lookup"><span data-stu-id="7362e-114">The setting that is being reported</span></span>|
|<span data-ttu-id="7362e-115">settingName</span><span class="sxs-lookup"><span data-stu-id="7362e-115">settingName</span></span>|<span data-ttu-id="7362e-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7362e-116">String</span></span>|<span data-ttu-id="7362e-117">Nome traduzido/amigável para o usuário da configuração que está sendo relatada</span><span class="sxs-lookup"><span data-stu-id="7362e-117">Localized/user friendly setting name that is being reported</span></span>|
|<span data-ttu-id="7362e-118">instanceDisplayName</span><span class="sxs-lookup"><span data-stu-id="7362e-118">instanceDisplayName</span></span>|<span data-ttu-id="7362e-119">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7362e-119">String</span></span>|<span data-ttu-id="7362e-120">Nome da instância de configuração está sendo relatada.</span><span class="sxs-lookup"><span data-stu-id="7362e-120">Name of setting instance that is being reported.</span></span>|
|<span data-ttu-id="7362e-121">estado</span><span class="sxs-lookup"><span data-stu-id="7362e-121">state</span></span>|[<span data-ttu-id="7362e-122">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="7362e-122">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="7362e-123">O estado de conformidade da configuração.</span><span class="sxs-lookup"><span data-stu-id="7362e-123">The compliance state of the setting.</span></span> <span data-ttu-id="7362e-124">Os valores possíveis são: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="7362e-124">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="7362e-125">errorCode</span><span class="sxs-lookup"><span data-stu-id="7362e-125">errorCode</span></span>|<span data-ttu-id="7362e-126">Int64</span><span class="sxs-lookup"><span data-stu-id="7362e-126">Int64</span></span>|<span data-ttu-id="7362e-127">Código de erro da configuração</span><span class="sxs-lookup"><span data-stu-id="7362e-127">Error code for the setting</span></span>|
|<span data-ttu-id="7362e-128">errorDescription</span><span class="sxs-lookup"><span data-stu-id="7362e-128">errorDescription</span></span>|<span data-ttu-id="7362e-129">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7362e-129">String</span></span>|<span data-ttu-id="7362e-130">Descrição do erro</span><span class="sxs-lookup"><span data-stu-id="7362e-130">Error description</span></span>|
|<span data-ttu-id="7362e-131">userId</span><span class="sxs-lookup"><span data-stu-id="7362e-131">userId</span></span>|<span data-ttu-id="7362e-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7362e-132">String</span></span>|<span data-ttu-id="7362e-133">UserId</span><span class="sxs-lookup"><span data-stu-id="7362e-133">UserId</span></span>|
|<span data-ttu-id="7362e-134">userName</span><span class="sxs-lookup"><span data-stu-id="7362e-134">userName</span></span>|<span data-ttu-id="7362e-135">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7362e-135">String</span></span>|<span data-ttu-id="7362e-136">UserName</span><span class="sxs-lookup"><span data-stu-id="7362e-136">UserName</span></span>|
|<span data-ttu-id="7362e-137">userEmail</span><span class="sxs-lookup"><span data-stu-id="7362e-137">userEmail</span></span>|<span data-ttu-id="7362e-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7362e-138">String</span></span>|<span data-ttu-id="7362e-139">UserEmail</span><span class="sxs-lookup"><span data-stu-id="7362e-139">UserEmail</span></span>|
|<span data-ttu-id="7362e-140">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="7362e-140">userPrincipalName</span></span>|<span data-ttu-id="7362e-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7362e-141">String</span></span>|<span data-ttu-id="7362e-142">UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="7362e-142">UserPrincipalName.</span></span>|
|<span data-ttu-id="7362e-143">sources</span><span class="sxs-lookup"><span data-stu-id="7362e-143">sources</span></span>|<span data-ttu-id="7362e-144">Coleção [settingSource](../resources/intune-deviceconfig-settingsource.md)</span><span class="sxs-lookup"><span data-stu-id="7362e-144">[settingSource](../resources/intune-deviceconfig-settingsource.md) collection</span></span>|<span data-ttu-id="7362e-145">Políticas colaboradoras</span><span class="sxs-lookup"><span data-stu-id="7362e-145">Contributing policies</span></span>|
|<span data-ttu-id="7362e-146">currentValue</span><span class="sxs-lookup"><span data-stu-id="7362e-146">currentValue</span></span>|<span data-ttu-id="7362e-147">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7362e-147">String</span></span>|<span data-ttu-id="7362e-148">Valor atual da configuração no dispositivo</span><span class="sxs-lookup"><span data-stu-id="7362e-148">Current value of setting on device</span></span>|

## <a name="relationships"></a><span data-ttu-id="7362e-149">Relações</span><span class="sxs-lookup"><span data-stu-id="7362e-149">Relationships</span></span>
<span data-ttu-id="7362e-150">Nenhum</span><span class="sxs-lookup"><span data-stu-id="7362e-150">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="7362e-151">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7362e-151">JSON Representation</span></span>
<span data-ttu-id="7362e-152">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7362e-152">Here is a JSON representation of the resource.</span></span>
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





