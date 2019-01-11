---
title: tipo de recurso de restrictedAppsViolation
description: Violação de perfil de configuração de aplicativos restritos por dispositivo por usuário
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: aefd9996805f0ee454bebc8871662b0ceac05a9b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27849375"
---
# <a name="restrictedappsviolation-resource-type"></a><span data-ttu-id="42d6a-103">tipo de recurso de restrictedAppsViolation</span><span class="sxs-lookup"><span data-stu-id="42d6a-103">restrictedAppsViolation resource type</span></span>

> <span data-ttu-id="42d6a-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="42d6a-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="42d6a-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="42d6a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="42d6a-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="42d6a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="42d6a-107">Violação de perfil de configuração de aplicativos restritos por dispositivo por usuário</span><span class="sxs-lookup"><span data-stu-id="42d6a-107">Violation of restricted apps configuration profile per device per user</span></span>
## <a name="methods"></a><span data-ttu-id="42d6a-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="42d6a-108">Methods</span></span>
|<span data-ttu-id="42d6a-109">Método</span><span class="sxs-lookup"><span data-stu-id="42d6a-109">Method</span></span>|<span data-ttu-id="42d6a-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="42d6a-110">Return Type</span></span>|<span data-ttu-id="42d6a-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="42d6a-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="42d6a-112">Lista restrictedAppsViolations</span><span class="sxs-lookup"><span data-stu-id="42d6a-112">List restrictedAppsViolations</span></span>](../api/intune-deviceconfig-restrictedappsviolation-list.md)|<span data-ttu-id="42d6a-113">coleção [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md)</span><span class="sxs-lookup"><span data-stu-id="42d6a-113">[restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) collection</span></span>|<span data-ttu-id="42d6a-114">Lista as propriedades e os relacionamentos dos objetos [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) .</span><span class="sxs-lookup"><span data-stu-id="42d6a-114">List properties and relationships of the [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) objects.</span></span>|
|[<span data-ttu-id="42d6a-115">Obter restrictedAppsViolation</span><span class="sxs-lookup"><span data-stu-id="42d6a-115">Get restrictedAppsViolation</span></span>](../api/intune-deviceconfig-restrictedappsviolation-get.md)|[<span data-ttu-id="42d6a-116">restrictedAppsViolation</span><span class="sxs-lookup"><span data-stu-id="42d6a-116">restrictedAppsViolation</span></span>](../resources/intune-deviceconfig-restrictedappsviolation.md)|<span data-ttu-id="42d6a-117">Leia as propriedades e os relacionamentos do objeto [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) .</span><span class="sxs-lookup"><span data-stu-id="42d6a-117">Read properties and relationships of the [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) object.</span></span>|
|[<span data-ttu-id="42d6a-118">Criar restrictedAppsViolation</span><span class="sxs-lookup"><span data-stu-id="42d6a-118">Create restrictedAppsViolation</span></span>](../api/intune-deviceconfig-restrictedappsviolation-create.md)|[<span data-ttu-id="42d6a-119">restrictedAppsViolation</span><span class="sxs-lookup"><span data-stu-id="42d6a-119">restrictedAppsViolation</span></span>](../resources/intune-deviceconfig-restrictedappsviolation.md)|<span data-ttu-id="42d6a-120">Crie um novo objeto de [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) .</span><span class="sxs-lookup"><span data-stu-id="42d6a-120">Create a new [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) object.</span></span>|
|[<span data-ttu-id="42d6a-121">Excluir restrictedAppsViolation</span><span class="sxs-lookup"><span data-stu-id="42d6a-121">Delete restrictedAppsViolation</span></span>](../api/intune-deviceconfig-restrictedappsviolation-delete.md)|<span data-ttu-id="42d6a-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="42d6a-122">None</span></span>|<span data-ttu-id="42d6a-123">Exclui um [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md).</span><span class="sxs-lookup"><span data-stu-id="42d6a-123">Deletes a [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md).</span></span>|
|[<span data-ttu-id="42d6a-124">Atualizar restrictedAppsViolation</span><span class="sxs-lookup"><span data-stu-id="42d6a-124">Update restrictedAppsViolation</span></span>](../api/intune-deviceconfig-restrictedappsviolation-update.md)|[<span data-ttu-id="42d6a-125">restrictedAppsViolation</span><span class="sxs-lookup"><span data-stu-id="42d6a-125">restrictedAppsViolation</span></span>](../resources/intune-deviceconfig-restrictedappsviolation.md)|<span data-ttu-id="42d6a-126">Atualize as propriedades de um objeto [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) .</span><span class="sxs-lookup"><span data-stu-id="42d6a-126">Update the properties of a [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="42d6a-127">Propriedades</span><span class="sxs-lookup"><span data-stu-id="42d6a-127">Properties</span></span>
|<span data-ttu-id="42d6a-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="42d6a-128">Property</span></span>|<span data-ttu-id="42d6a-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="42d6a-129">Type</span></span>|<span data-ttu-id="42d6a-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="42d6a-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="42d6a-131">id</span><span class="sxs-lookup"><span data-stu-id="42d6a-131">id</span></span>|<span data-ttu-id="42d6a-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="42d6a-132">String</span></span>|<span data-ttu-id="42d6a-133">Identificador exclusivo para o objeto.</span><span class="sxs-lookup"><span data-stu-id="42d6a-133">Unique identifier for the object.</span></span> <span data-ttu-id="42d6a-134">Composto de accountId, deviceId, policyId e userId</span><span class="sxs-lookup"><span data-stu-id="42d6a-134">Composed from accountId, deviceId, policyId and userId</span></span>|
|<span data-ttu-id="42d6a-135">userId</span><span class="sxs-lookup"><span data-stu-id="42d6a-135">userId</span></span>|<span data-ttu-id="42d6a-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="42d6a-136">String</span></span>|<span data-ttu-id="42d6a-137">Identificador exclusivo do usuário, deve ser um Guid</span><span class="sxs-lookup"><span data-stu-id="42d6a-137">User unique identifier, must be Guid</span></span>|
|<span data-ttu-id="42d6a-138">userName</span><span class="sxs-lookup"><span data-stu-id="42d6a-138">userName</span></span>|<span data-ttu-id="42d6a-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="42d6a-139">String</span></span>|<span data-ttu-id="42d6a-140">Nome de usuário</span><span class="sxs-lookup"><span data-stu-id="42d6a-140">User name</span></span>|
|<span data-ttu-id="42d6a-141">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="42d6a-141">managedDeviceId</span></span>|<span data-ttu-id="42d6a-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="42d6a-142">String</span></span>|<span data-ttu-id="42d6a-143">Identificador exclusivo do dispositivo gerenciado, deve ser um Guid</span><span class="sxs-lookup"><span data-stu-id="42d6a-143">Managed device unique identifier, must be Guid</span></span>|
|<span data-ttu-id="42d6a-144">deviceName</span><span class="sxs-lookup"><span data-stu-id="42d6a-144">deviceName</span></span>|<span data-ttu-id="42d6a-145">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="42d6a-145">String</span></span>|<span data-ttu-id="42d6a-146">Nome do dispositivo</span><span class="sxs-lookup"><span data-stu-id="42d6a-146">Device name</span></span>|
|<span data-ttu-id="42d6a-147">deviceConfigurationId</span><span class="sxs-lookup"><span data-stu-id="42d6a-147">deviceConfigurationId</span></span>|<span data-ttu-id="42d6a-148">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="42d6a-148">String</span></span>|<span data-ttu-id="42d6a-149">Identificador exclusivo do perfil do configuração de dispositivo, deve ser um Guid</span><span class="sxs-lookup"><span data-stu-id="42d6a-149">Device configuration profile unique identifier, must be Guid</span></span>|
|<span data-ttu-id="42d6a-150">deviceConfigurationName</span><span class="sxs-lookup"><span data-stu-id="42d6a-150">deviceConfigurationName</span></span>|<span data-ttu-id="42d6a-151">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="42d6a-151">String</span></span>|<span data-ttu-id="42d6a-152">Nome do perfil de configuração de dispositivo</span><span class="sxs-lookup"><span data-stu-id="42d6a-152">Device configuration profile name</span></span>|
|<span data-ttu-id="42d6a-153">platformType</span><span class="sxs-lookup"><span data-stu-id="42d6a-153">platformType</span></span>|[<span data-ttu-id="42d6a-154">policyPlatformType</span><span class="sxs-lookup"><span data-stu-id="42d6a-154">policyPlatformType</span></span>](../resources/intune-deviceconfig-policyplatformtype.md)|<span data-ttu-id="42d6a-155">Tipo de plataforma.</span><span class="sxs-lookup"><span data-stu-id="42d6a-155">Platform type.</span></span> <span data-ttu-id="42d6a-156">Os valores possíveis são: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.</span><span class="sxs-lookup"><span data-stu-id="42d6a-156">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.</span></span>|
|<span data-ttu-id="42d6a-157">restrictedAppsState</span><span class="sxs-lookup"><span data-stu-id="42d6a-157">restrictedAppsState</span></span>|[<span data-ttu-id="42d6a-158">restrictedAppsState</span><span class="sxs-lookup"><span data-stu-id="42d6a-158">restrictedAppsState</span></span>](../resources/intune-deviceconfig-restrictedappsstate.md)|<span data-ttu-id="42d6a-159">Estado restrito de aplicativos.</span><span class="sxs-lookup"><span data-stu-id="42d6a-159">Restricted apps state.</span></span> <span data-ttu-id="42d6a-160">Os valores possíveis são: `prohibitedApps` e `notApprovedApps`.</span><span class="sxs-lookup"><span data-stu-id="42d6a-160">Possible values are: `prohibitedApps`, `notApprovedApps`.</span></span>|
|<span data-ttu-id="42d6a-161">restrictedApps</span><span class="sxs-lookup"><span data-stu-id="42d6a-161">restrictedApps</span></span>|<span data-ttu-id="42d6a-162">coleção [managedDeviceReportedApp](../resources/intune-deviceconfig-manageddevicereportedapp.md)</span><span class="sxs-lookup"><span data-stu-id="42d6a-162">[managedDeviceReportedApp](../resources/intune-deviceconfig-manageddevicereportedapp.md) collection</span></span>|<span data-ttu-id="42d6a-163">Lista de aplicativos restritos violadas</span><span class="sxs-lookup"><span data-stu-id="42d6a-163">List of violated restricted apps</span></span>|

## <a name="relationships"></a><span data-ttu-id="42d6a-164">Relações</span><span class="sxs-lookup"><span data-stu-id="42d6a-164">Relationships</span></span>
<span data-ttu-id="42d6a-165">Nenhum</span><span class="sxs-lookup"><span data-stu-id="42d6a-165">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="42d6a-166">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="42d6a-166">JSON Representation</span></span>
<span data-ttu-id="42d6a-167">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="42d6a-167">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.restrictedAppsViolation"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.restrictedAppsViolation",
  "id": "String (identifier)",
  "userId": "String",
  "userName": "String",
  "managedDeviceId": "String",
  "deviceName": "String",
  "deviceConfigurationId": "String",
  "deviceConfigurationName": "String",
  "platformType": "String",
  "restrictedAppsState": "String",
  "restrictedApps": [
    {
      "@odata.type": "microsoft.graph.managedDeviceReportedApp",
      "appId": "String"
    }
  ]
}
```





