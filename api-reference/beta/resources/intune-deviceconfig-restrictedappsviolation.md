---
title: tipo de recurso de restrictedAppsViolation
description: Violação de perfil de configuração de aplicativos restritos por dispositivo por usuário
author: tfitzmac
ms.openlocfilehash: cb614bc56f27281198fcecb73bae2b7beddfa266
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27304932"
---
# <a name="restrictedappsviolation-resource-type"></a><span data-ttu-id="f881c-103">tipo de recurso de restrictedAppsViolation</span><span class="sxs-lookup"><span data-stu-id="f881c-103">restrictedAppsViolation resource type</span></span>

> <span data-ttu-id="f881c-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="f881c-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f881c-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="f881c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f881c-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="f881c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f881c-107">Violação de perfil de configuração de aplicativos restritos por dispositivo por usuário</span><span class="sxs-lookup"><span data-stu-id="f881c-107">Violation of restricted apps configuration profile per device per user</span></span>
## <a name="methods"></a><span data-ttu-id="f881c-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="f881c-108">Methods</span></span>
|<span data-ttu-id="f881c-109">Método</span><span class="sxs-lookup"><span data-stu-id="f881c-109">Method</span></span>|<span data-ttu-id="f881c-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="f881c-110">Return Type</span></span>|<span data-ttu-id="f881c-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="f881c-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="f881c-112">Lista restrictedAppsViolations</span><span class="sxs-lookup"><span data-stu-id="f881c-112">List restrictedAppsViolations</span></span>](../api/intune-deviceconfig-restrictedappsviolation-list.md)|<span data-ttu-id="f881c-113">coleção [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md)</span><span class="sxs-lookup"><span data-stu-id="f881c-113">[restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) collection</span></span>|<span data-ttu-id="f881c-114">Lista as propriedades e os relacionamentos dos objetos [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) .</span><span class="sxs-lookup"><span data-stu-id="f881c-114">List properties and relationships of the [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) objects.</span></span>|
|[<span data-ttu-id="f881c-115">Obter restrictedAppsViolation</span><span class="sxs-lookup"><span data-stu-id="f881c-115">Get restrictedAppsViolation</span></span>](../api/intune-deviceconfig-restrictedappsviolation-get.md)|[<span data-ttu-id="f881c-116">restrictedAppsViolation</span><span class="sxs-lookup"><span data-stu-id="f881c-116">restrictedAppsViolation</span></span>](../resources/intune-deviceconfig-restrictedappsviolation.md)|<span data-ttu-id="f881c-117">Leia as propriedades e os relacionamentos do objeto [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) .</span><span class="sxs-lookup"><span data-stu-id="f881c-117">Read properties and relationships of the [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) object.</span></span>|
|[<span data-ttu-id="f881c-118">Criar restrictedAppsViolation</span><span class="sxs-lookup"><span data-stu-id="f881c-118">Create restrictedAppsViolation</span></span>](../api/intune-deviceconfig-restrictedappsviolation-create.md)|[<span data-ttu-id="f881c-119">restrictedAppsViolation</span><span class="sxs-lookup"><span data-stu-id="f881c-119">restrictedAppsViolation</span></span>](../resources/intune-deviceconfig-restrictedappsviolation.md)|<span data-ttu-id="f881c-120">Crie um novo objeto de [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) .</span><span class="sxs-lookup"><span data-stu-id="f881c-120">Create a new [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) object.</span></span>|
|[<span data-ttu-id="f881c-121">Excluir restrictedAppsViolation</span><span class="sxs-lookup"><span data-stu-id="f881c-121">Delete restrictedAppsViolation</span></span>](../api/intune-deviceconfig-restrictedappsviolation-delete.md)|<span data-ttu-id="f881c-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f881c-122">None</span></span>|<span data-ttu-id="f881c-123">Exclui um [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md).</span><span class="sxs-lookup"><span data-stu-id="f881c-123">Deletes a [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md).</span></span>|
|[<span data-ttu-id="f881c-124">Atualizar restrictedAppsViolation</span><span class="sxs-lookup"><span data-stu-id="f881c-124">Update restrictedAppsViolation</span></span>](../api/intune-deviceconfig-restrictedappsviolation-update.md)|[<span data-ttu-id="f881c-125">restrictedAppsViolation</span><span class="sxs-lookup"><span data-stu-id="f881c-125">restrictedAppsViolation</span></span>](../resources/intune-deviceconfig-restrictedappsviolation.md)|<span data-ttu-id="f881c-126">Atualize as propriedades de um objeto [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) .</span><span class="sxs-lookup"><span data-stu-id="f881c-126">Update the properties of a [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="f881c-127">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f881c-127">Properties</span></span>
|<span data-ttu-id="f881c-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f881c-128">Property</span></span>|<span data-ttu-id="f881c-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="f881c-129">Type</span></span>|<span data-ttu-id="f881c-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="f881c-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f881c-131">id</span><span class="sxs-lookup"><span data-stu-id="f881c-131">id</span></span>|<span data-ttu-id="f881c-132">String</span><span class="sxs-lookup"><span data-stu-id="f881c-132">String</span></span>|<span data-ttu-id="f881c-133">Identificador exclusivo para o objeto.</span><span class="sxs-lookup"><span data-stu-id="f881c-133">Unique identifier for the object.</span></span> <span data-ttu-id="f881c-134">Composto de accountId, deviceId, policyId e userId</span><span class="sxs-lookup"><span data-stu-id="f881c-134">Composed from accountId, deviceId, policyId and userId</span></span>|
|<span data-ttu-id="f881c-135">userId</span><span class="sxs-lookup"><span data-stu-id="f881c-135">userId</span></span>|<span data-ttu-id="f881c-136">String</span><span class="sxs-lookup"><span data-stu-id="f881c-136">String</span></span>|<span data-ttu-id="f881c-137">Identificador exclusivo do usuário, deve ser um Guid</span><span class="sxs-lookup"><span data-stu-id="f881c-137">User unique identifier, must be Guid</span></span>|
|<span data-ttu-id="f881c-138">userName</span><span class="sxs-lookup"><span data-stu-id="f881c-138">userName</span></span>|<span data-ttu-id="f881c-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f881c-139">String</span></span>|<span data-ttu-id="f881c-140">Nome de usuário</span><span class="sxs-lookup"><span data-stu-id="f881c-140">User name</span></span>|
|<span data-ttu-id="f881c-141">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="f881c-141">managedDeviceId</span></span>|<span data-ttu-id="f881c-142">String</span><span class="sxs-lookup"><span data-stu-id="f881c-142">String</span></span>|<span data-ttu-id="f881c-143">Identificador exclusivo do dispositivo gerenciado, deve ser um Guid</span><span class="sxs-lookup"><span data-stu-id="f881c-143">Managed device unique identifier, must be Guid</span></span>|
|<span data-ttu-id="f881c-144">deviceName</span><span class="sxs-lookup"><span data-stu-id="f881c-144">deviceName</span></span>|<span data-ttu-id="f881c-145">String</span><span class="sxs-lookup"><span data-stu-id="f881c-145">String</span></span>|<span data-ttu-id="f881c-146">Nome do dispositivo</span><span class="sxs-lookup"><span data-stu-id="f881c-146">Device name</span></span>|
|<span data-ttu-id="f881c-147">deviceConfigurationId</span><span class="sxs-lookup"><span data-stu-id="f881c-147">deviceConfigurationId</span></span>|<span data-ttu-id="f881c-148">String</span><span class="sxs-lookup"><span data-stu-id="f881c-148">String</span></span>|<span data-ttu-id="f881c-149">Identificador exclusivo do perfil do configuração de dispositivo, deve ser um Guid</span><span class="sxs-lookup"><span data-stu-id="f881c-149">Device configuration profile unique identifier, must be Guid</span></span>|
|<span data-ttu-id="f881c-150">deviceConfigurationName</span><span class="sxs-lookup"><span data-stu-id="f881c-150">deviceConfigurationName</span></span>|<span data-ttu-id="f881c-151">String</span><span class="sxs-lookup"><span data-stu-id="f881c-151">String</span></span>|<span data-ttu-id="f881c-152">Nome do perfil de configuração de dispositivo</span><span class="sxs-lookup"><span data-stu-id="f881c-152">Device configuration profile name</span></span>|
|<span data-ttu-id="f881c-153">platformType</span><span class="sxs-lookup"><span data-stu-id="f881c-153">platformType</span></span>|[<span data-ttu-id="f881c-154">policyPlatformType</span><span class="sxs-lookup"><span data-stu-id="f881c-154">policyPlatformType</span></span>](../resources/intune-deviceconfig-policyplatformtype.md)|<span data-ttu-id="f881c-155">Tipo de plataforma.</span><span class="sxs-lookup"><span data-stu-id="f881c-155">Platform type.</span></span> <span data-ttu-id="f881c-156">Os valores possíveis são: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.</span><span class="sxs-lookup"><span data-stu-id="f881c-156">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.</span></span>|
|<span data-ttu-id="f881c-157">restrictedAppsState</span><span class="sxs-lookup"><span data-stu-id="f881c-157">restrictedAppsState</span></span>|[<span data-ttu-id="f881c-158">restrictedAppsState</span><span class="sxs-lookup"><span data-stu-id="f881c-158">restrictedAppsState</span></span>](../resources/intune-deviceconfig-restrictedappsstate.md)|<span data-ttu-id="f881c-159">Estado restrito de aplicativos.</span><span class="sxs-lookup"><span data-stu-id="f881c-159">Restricted apps state.</span></span> <span data-ttu-id="f881c-160">Os valores possíveis são: `prohibitedApps` e `notApprovedApps`.</span><span class="sxs-lookup"><span data-stu-id="f881c-160">Possible values are: `prohibitedApps`, `notApprovedApps`.</span></span>|
|<span data-ttu-id="f881c-161">restrictedApps</span><span class="sxs-lookup"><span data-stu-id="f881c-161">restrictedApps</span></span>|<span data-ttu-id="f881c-162">coleção [managedDeviceReportedApp](../resources/intune-deviceconfig-manageddevicereportedapp.md)</span><span class="sxs-lookup"><span data-stu-id="f881c-162">[managedDeviceReportedApp](../resources/intune-deviceconfig-manageddevicereportedapp.md) collection</span></span>|<span data-ttu-id="f881c-163">Lista de aplicativos restritos violadas</span><span class="sxs-lookup"><span data-stu-id="f881c-163">List of violated restricted apps</span></span>|

## <a name="relationships"></a><span data-ttu-id="f881c-164">Relações</span><span class="sxs-lookup"><span data-stu-id="f881c-164">Relationships</span></span>
<span data-ttu-id="f881c-165">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f881c-165">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="f881c-166">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f881c-166">JSON Representation</span></span>
<span data-ttu-id="f881c-167">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f881c-167">Here is a JSON representation of the resource.</span></span>
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





