---
title: tipo de recurso de restrictedAppsViolation
description: Violação de perfil de configuração de aplicativos restritos por dispositivo por usuário
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: dcbd7def59d17dcd6e906e1e6bef85e3a448b880
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29424977"
---
# <a name="restrictedappsviolation-resource-type"></a><span data-ttu-id="3e187-103">tipo de recurso de restrictedAppsViolation</span><span class="sxs-lookup"><span data-stu-id="3e187-103">restrictedAppsViolation resource type</span></span>

> <span data-ttu-id="3e187-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="3e187-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="3e187-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="3e187-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3e187-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="3e187-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3e187-107">Violação de perfil de configuração de aplicativos restritos por dispositivo por usuário</span><span class="sxs-lookup"><span data-stu-id="3e187-107">Violation of restricted apps configuration profile per device per user</span></span>

## <a name="methods"></a><span data-ttu-id="3e187-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="3e187-108">Methods</span></span>
|<span data-ttu-id="3e187-109">Método</span><span class="sxs-lookup"><span data-stu-id="3e187-109">Method</span></span>|<span data-ttu-id="3e187-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="3e187-110">Return Type</span></span>|<span data-ttu-id="3e187-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="3e187-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="3e187-112">Lista restrictedAppsViolations</span><span class="sxs-lookup"><span data-stu-id="3e187-112">List restrictedAppsViolations</span></span>](../api/intune-deviceconfig-restrictedappsviolation-list.md)|<span data-ttu-id="3e187-113">coleção [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md)</span><span class="sxs-lookup"><span data-stu-id="3e187-113">[restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) collection</span></span>|<span data-ttu-id="3e187-114">Lista as propriedades e os relacionamentos dos objetos [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) .</span><span class="sxs-lookup"><span data-stu-id="3e187-114">List properties and relationships of the [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) objects.</span></span>|
|[<span data-ttu-id="3e187-115">Obter restrictedAppsViolation</span><span class="sxs-lookup"><span data-stu-id="3e187-115">Get restrictedAppsViolation</span></span>](../api/intune-deviceconfig-restrictedappsviolation-get.md)|[<span data-ttu-id="3e187-116">restrictedAppsViolation</span><span class="sxs-lookup"><span data-stu-id="3e187-116">restrictedAppsViolation</span></span>](../resources/intune-deviceconfig-restrictedappsviolation.md)|<span data-ttu-id="3e187-117">Leia as propriedades e os relacionamentos do objeto [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) .</span><span class="sxs-lookup"><span data-stu-id="3e187-117">Read properties and relationships of the [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) object.</span></span>|
|[<span data-ttu-id="3e187-118">Criar restrictedAppsViolation</span><span class="sxs-lookup"><span data-stu-id="3e187-118">Create restrictedAppsViolation</span></span>](../api/intune-deviceconfig-restrictedappsviolation-create.md)|[<span data-ttu-id="3e187-119">restrictedAppsViolation</span><span class="sxs-lookup"><span data-stu-id="3e187-119">restrictedAppsViolation</span></span>](../resources/intune-deviceconfig-restrictedappsviolation.md)|<span data-ttu-id="3e187-120">Crie um novo objeto de [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) .</span><span class="sxs-lookup"><span data-stu-id="3e187-120">Create a new [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) object.</span></span>|
|[<span data-ttu-id="3e187-121">Excluir restrictedAppsViolation</span><span class="sxs-lookup"><span data-stu-id="3e187-121">Delete restrictedAppsViolation</span></span>](../api/intune-deviceconfig-restrictedappsviolation-delete.md)|<span data-ttu-id="3e187-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="3e187-122">None</span></span>|<span data-ttu-id="3e187-123">Exclui um [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md).</span><span class="sxs-lookup"><span data-stu-id="3e187-123">Deletes a [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md).</span></span>|
|[<span data-ttu-id="3e187-124">Atualizar restrictedAppsViolation</span><span class="sxs-lookup"><span data-stu-id="3e187-124">Update restrictedAppsViolation</span></span>](../api/intune-deviceconfig-restrictedappsviolation-update.md)|[<span data-ttu-id="3e187-125">restrictedAppsViolation</span><span class="sxs-lookup"><span data-stu-id="3e187-125">restrictedAppsViolation</span></span>](../resources/intune-deviceconfig-restrictedappsviolation.md)|<span data-ttu-id="3e187-126">Atualize as propriedades de um objeto [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) .</span><span class="sxs-lookup"><span data-stu-id="3e187-126">Update the properties of a [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="3e187-127">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3e187-127">Properties</span></span>
|<span data-ttu-id="3e187-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3e187-128">Property</span></span>|<span data-ttu-id="3e187-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="3e187-129">Type</span></span>|<span data-ttu-id="3e187-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="3e187-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3e187-131">id</span><span class="sxs-lookup"><span data-stu-id="3e187-131">id</span></span>|<span data-ttu-id="3e187-132">String</span><span class="sxs-lookup"><span data-stu-id="3e187-132">String</span></span>|<span data-ttu-id="3e187-133">Identificador exclusivo para o objeto.</span><span class="sxs-lookup"><span data-stu-id="3e187-133">Unique identifier for the object.</span></span> <span data-ttu-id="3e187-134">Composto de accountId, deviceId, policyId e userId</span><span class="sxs-lookup"><span data-stu-id="3e187-134">Composed from accountId, deviceId, policyId and userId</span></span>|
|<span data-ttu-id="3e187-135">userId</span><span class="sxs-lookup"><span data-stu-id="3e187-135">userId</span></span>|<span data-ttu-id="3e187-136">String</span><span class="sxs-lookup"><span data-stu-id="3e187-136">String</span></span>|<span data-ttu-id="3e187-137">Identificador exclusivo do usuário, deve ser um Guid</span><span class="sxs-lookup"><span data-stu-id="3e187-137">User unique identifier, must be Guid</span></span>|
|<span data-ttu-id="3e187-138">userName</span><span class="sxs-lookup"><span data-stu-id="3e187-138">userName</span></span>|<span data-ttu-id="3e187-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3e187-139">String</span></span>|<span data-ttu-id="3e187-140">Nome de usuário</span><span class="sxs-lookup"><span data-stu-id="3e187-140">User name</span></span>|
|<span data-ttu-id="3e187-141">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="3e187-141">managedDeviceId</span></span>|<span data-ttu-id="3e187-142">String</span><span class="sxs-lookup"><span data-stu-id="3e187-142">String</span></span>|<span data-ttu-id="3e187-143">Identificador exclusivo do dispositivo gerenciado, deve ser um Guid</span><span class="sxs-lookup"><span data-stu-id="3e187-143">Managed device unique identifier, must be Guid</span></span>|
|<span data-ttu-id="3e187-144">deviceName</span><span class="sxs-lookup"><span data-stu-id="3e187-144">deviceName</span></span>|<span data-ttu-id="3e187-145">String</span><span class="sxs-lookup"><span data-stu-id="3e187-145">String</span></span>|<span data-ttu-id="3e187-146">Nome do dispositivo</span><span class="sxs-lookup"><span data-stu-id="3e187-146">Device name</span></span>|
|<span data-ttu-id="3e187-147">deviceConfigurationId</span><span class="sxs-lookup"><span data-stu-id="3e187-147">deviceConfigurationId</span></span>|<span data-ttu-id="3e187-148">String</span><span class="sxs-lookup"><span data-stu-id="3e187-148">String</span></span>|<span data-ttu-id="3e187-149">Identificador exclusivo do perfil do configuração de dispositivo, deve ser um Guid</span><span class="sxs-lookup"><span data-stu-id="3e187-149">Device configuration profile unique identifier, must be Guid</span></span>|
|<span data-ttu-id="3e187-150">deviceConfigurationName</span><span class="sxs-lookup"><span data-stu-id="3e187-150">deviceConfigurationName</span></span>|<span data-ttu-id="3e187-151">String</span><span class="sxs-lookup"><span data-stu-id="3e187-151">String</span></span>|<span data-ttu-id="3e187-152">Nome do perfil de configuração de dispositivo</span><span class="sxs-lookup"><span data-stu-id="3e187-152">Device configuration profile name</span></span>|
|<span data-ttu-id="3e187-153">platformType</span><span class="sxs-lookup"><span data-stu-id="3e187-153">platformType</span></span>|[<span data-ttu-id="3e187-154">policyPlatformType</span><span class="sxs-lookup"><span data-stu-id="3e187-154">policyPlatformType</span></span>](../resources/intune-deviceconfig-policyplatformtype.md)|<span data-ttu-id="3e187-155">Tipo de plataforma.</span><span class="sxs-lookup"><span data-stu-id="3e187-155">Platform type.</span></span> <span data-ttu-id="3e187-156">Os valores possíveis são: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.</span><span class="sxs-lookup"><span data-stu-id="3e187-156">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.</span></span>|
|<span data-ttu-id="3e187-157">restrictedAppsState</span><span class="sxs-lookup"><span data-stu-id="3e187-157">restrictedAppsState</span></span>|[<span data-ttu-id="3e187-158">restrictedAppsState</span><span class="sxs-lookup"><span data-stu-id="3e187-158">restrictedAppsState</span></span>](../resources/intune-deviceconfig-restrictedappsstate.md)|<span data-ttu-id="3e187-159">Estado restrito de aplicativos.</span><span class="sxs-lookup"><span data-stu-id="3e187-159">Restricted apps state.</span></span> <span data-ttu-id="3e187-160">Os valores possíveis são: `prohibitedApps` e `notApprovedApps`.</span><span class="sxs-lookup"><span data-stu-id="3e187-160">Possible values are: `prohibitedApps`, `notApprovedApps`.</span></span>|
|<span data-ttu-id="3e187-161">restrictedApps</span><span class="sxs-lookup"><span data-stu-id="3e187-161">restrictedApps</span></span>|<span data-ttu-id="3e187-162">coleção [managedDeviceReportedApp](../resources/intune-deviceconfig-manageddevicereportedapp.md)</span><span class="sxs-lookup"><span data-stu-id="3e187-162">[managedDeviceReportedApp](../resources/intune-deviceconfig-manageddevicereportedapp.md) collection</span></span>|<span data-ttu-id="3e187-163">Lista de aplicativos restritos violadas</span><span class="sxs-lookup"><span data-stu-id="3e187-163">List of violated restricted apps</span></span>|

## <a name="relationships"></a><span data-ttu-id="3e187-164">Relações</span><span class="sxs-lookup"><span data-stu-id="3e187-164">Relationships</span></span>
<span data-ttu-id="3e187-165">Nenhum</span><span class="sxs-lookup"><span data-stu-id="3e187-165">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3e187-166">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3e187-166">JSON Representation</span></span>
<span data-ttu-id="3e187-167">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3e187-167">Here is a JSON representation of the resource.</span></span>
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




