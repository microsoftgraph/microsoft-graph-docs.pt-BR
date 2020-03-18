---
title: Atualizar restrictedAppsViolation
description: Atualiza as propriedades de um objeto restrictedAppsViolation.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 5dd783a68ffe608265d0b65f9404678d244b705d
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42742390"
---
# <a name="update-restrictedappsviolation"></a><span data-ttu-id="17133-103">Atualizar restrictedAppsViolation</span><span class="sxs-lookup"><span data-stu-id="17133-103">Update restrictedAppsViolation</span></span>

> <span data-ttu-id="17133-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="17133-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="17133-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="17133-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="17133-106">Atualiza as propriedades de um objeto [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) .</span><span class="sxs-lookup"><span data-stu-id="17133-106">Update the properties of a [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="17133-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="17133-107">Prerequisites</span></span>
<span data-ttu-id="17133-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="17133-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="17133-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="17133-110">Permission type</span></span>|<span data-ttu-id="17133-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="17133-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="17133-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="17133-112">Delegated (work or school account)</span></span>|<span data-ttu-id="17133-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="17133-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="17133-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="17133-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="17133-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="17133-115">Not supported.</span></span>|
|<span data-ttu-id="17133-116">Application</span><span class="sxs-lookup"><span data-stu-id="17133-116">Application</span></span>|<span data-ttu-id="17133-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="17133-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="17133-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="17133-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurationRestrictedAppsViolations/{restrictedAppsViolationId}
```

## <a name="request-headers"></a><span data-ttu-id="17133-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="17133-119">Request headers</span></span>
|<span data-ttu-id="17133-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="17133-120">Header</span></span>|<span data-ttu-id="17133-121">Valor</span><span class="sxs-lookup"><span data-stu-id="17133-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="17133-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="17133-122">Authorization</span></span>|<span data-ttu-id="17133-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="17133-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="17133-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="17133-124">Accept</span></span>|<span data-ttu-id="17133-125">application/json</span><span class="sxs-lookup"><span data-stu-id="17133-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="17133-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="17133-126">Request body</span></span>
<span data-ttu-id="17133-127">No corpo da solicitação, forneça uma representação JSON do objeto [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) .</span><span class="sxs-lookup"><span data-stu-id="17133-127">In the request body, supply a JSON representation for the [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) object.</span></span>

<span data-ttu-id="17133-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md).</span><span class="sxs-lookup"><span data-stu-id="17133-128">The following table shows the properties that are required when you create the [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md).</span></span>

|<span data-ttu-id="17133-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="17133-129">Property</span></span>|<span data-ttu-id="17133-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="17133-130">Type</span></span>|<span data-ttu-id="17133-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="17133-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="17133-132">id</span><span class="sxs-lookup"><span data-stu-id="17133-132">id</span></span>|<span data-ttu-id="17133-133">String</span><span class="sxs-lookup"><span data-stu-id="17133-133">String</span></span>|<span data-ttu-id="17133-134">Identificador exclusivo do objeto.</span><span class="sxs-lookup"><span data-stu-id="17133-134">Unique identifier for the object.</span></span> <span data-ttu-id="17133-135">Composto de AccountId, DeviceID, PolicyId e userId</span><span class="sxs-lookup"><span data-stu-id="17133-135">Composed from accountId, deviceId, policyId and userId</span></span>|
|<span data-ttu-id="17133-136">userId</span><span class="sxs-lookup"><span data-stu-id="17133-136">userId</span></span>|<span data-ttu-id="17133-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="17133-137">String</span></span>|<span data-ttu-id="17133-138">O identificador exclusivo do usuário deve ser GUID</span><span class="sxs-lookup"><span data-stu-id="17133-138">User unique identifier, must be Guid</span></span>|
|<span data-ttu-id="17133-139">userName</span><span class="sxs-lookup"><span data-stu-id="17133-139">userName</span></span>|<span data-ttu-id="17133-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="17133-140">String</span></span>|<span data-ttu-id="17133-141">Nome de usuário</span><span class="sxs-lookup"><span data-stu-id="17133-141">User name</span></span>|
|<span data-ttu-id="17133-142">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="17133-142">managedDeviceId</span></span>|<span data-ttu-id="17133-143">String</span><span class="sxs-lookup"><span data-stu-id="17133-143">String</span></span>|<span data-ttu-id="17133-144">O identificador exclusivo do dispositivo gerenciado deve ser GUID</span><span class="sxs-lookup"><span data-stu-id="17133-144">Managed device unique identifier, must be Guid</span></span>|
|<span data-ttu-id="17133-145">deviceName</span><span class="sxs-lookup"><span data-stu-id="17133-145">deviceName</span></span>|<span data-ttu-id="17133-146">String</span><span class="sxs-lookup"><span data-stu-id="17133-146">String</span></span>|<span data-ttu-id="17133-147">Nome do dispositivo</span><span class="sxs-lookup"><span data-stu-id="17133-147">Device name</span></span>|
|<span data-ttu-id="17133-148">deviceConfigurationId</span><span class="sxs-lookup"><span data-stu-id="17133-148">deviceConfigurationId</span></span>|<span data-ttu-id="17133-149">String</span><span class="sxs-lookup"><span data-stu-id="17133-149">String</span></span>|<span data-ttu-id="17133-150">O identificador exclusivo do perfil de configuração do dispositivo deve ser GUID</span><span class="sxs-lookup"><span data-stu-id="17133-150">Device configuration profile unique identifier, must be Guid</span></span>|
|<span data-ttu-id="17133-151">deviceConfigurationName</span><span class="sxs-lookup"><span data-stu-id="17133-151">deviceConfigurationName</span></span>|<span data-ttu-id="17133-152">String</span><span class="sxs-lookup"><span data-stu-id="17133-152">String</span></span>|<span data-ttu-id="17133-153">Nome do perfil de configuração do dispositivo</span><span class="sxs-lookup"><span data-stu-id="17133-153">Device configuration profile name</span></span>|
|<span data-ttu-id="17133-154">platformType</span><span class="sxs-lookup"><span data-stu-id="17133-154">platformType</span></span>|[<span data-ttu-id="17133-155">policyPlatformType</span><span class="sxs-lookup"><span data-stu-id="17133-155">policyPlatformType</span></span>](../resources/intune-shared-policyplatformtype.md)|<span data-ttu-id="17133-156">Tipo de plataforma.</span><span class="sxs-lookup"><span data-stu-id="17133-156">Platform type.</span></span> <span data-ttu-id="17133-157">Os valores possíveis são: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.</span><span class="sxs-lookup"><span data-stu-id="17133-157">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.</span></span>|
|<span data-ttu-id="17133-158">restrictedAppsState</span><span class="sxs-lookup"><span data-stu-id="17133-158">restrictedAppsState</span></span>|[<span data-ttu-id="17133-159">restrictedAppsState</span><span class="sxs-lookup"><span data-stu-id="17133-159">restrictedAppsState</span></span>](../resources/intune-deviceconfig-restrictedappsstate.md)|<span data-ttu-id="17133-160">Estado de aplicativos restritos.</span><span class="sxs-lookup"><span data-stu-id="17133-160">Restricted apps state.</span></span> <span data-ttu-id="17133-161">Os valores possíveis são: `prohibitedApps` e `notApprovedApps`.</span><span class="sxs-lookup"><span data-stu-id="17133-161">Possible values are: `prohibitedApps`, `notApprovedApps`.</span></span>|
|<span data-ttu-id="17133-162">restrictedApps</span><span class="sxs-lookup"><span data-stu-id="17133-162">restrictedApps</span></span>|<span data-ttu-id="17133-163">coleção [managedDeviceReportedApp](../resources/intune-deviceconfig-manageddevicereportedapp.md)</span><span class="sxs-lookup"><span data-stu-id="17133-163">[managedDeviceReportedApp](../resources/intune-deviceconfig-manageddevicereportedapp.md) collection</span></span>|<span data-ttu-id="17133-164">Lista de aplicativos restritos violados</span><span class="sxs-lookup"><span data-stu-id="17133-164">List of violated restricted apps</span></span>|



## <a name="response"></a><span data-ttu-id="17133-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="17133-165">Response</span></span>
<span data-ttu-id="17133-166">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="17133-166">If successful, this method returns a `200 OK` response code and an updated [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="17133-167">Exemplo</span><span class="sxs-lookup"><span data-stu-id="17133-167">Example</span></span>

### <a name="request"></a><span data-ttu-id="17133-168">Solicitação</span><span class="sxs-lookup"><span data-stu-id="17133-168">Request</span></span>
<span data-ttu-id="17133-169">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="17133-169">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurationRestrictedAppsViolations/{restrictedAppsViolationId}
Content-type: application/json
Content-length: 564

{
  "@odata.type": "#microsoft.graph.restrictedAppsViolation",
  "userId": "User Id value",
  "userName": "User Name value",
  "managedDeviceId": "Managed Device Id value",
  "deviceName": "Device Name value",
  "deviceConfigurationId": "Device Configuration Id value",
  "deviceConfigurationName": "Device Configuration Name value",
  "platformType": "androidForWork",
  "restrictedAppsState": "notApprovedApps",
  "restrictedApps": [
    {
      "@odata.type": "microsoft.graph.managedDeviceReportedApp",
      "appId": "App Id value"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="17133-170">Resposta</span><span class="sxs-lookup"><span data-stu-id="17133-170">Response</span></span>
<span data-ttu-id="17133-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="17133-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 613

{
  "@odata.type": "#microsoft.graph.restrictedAppsViolation",
  "id": "53f99903-9903-53f9-0399-f9530399f953",
  "userId": "User Id value",
  "userName": "User Name value",
  "managedDeviceId": "Managed Device Id value",
  "deviceName": "Device Name value",
  "deviceConfigurationId": "Device Configuration Id value",
  "deviceConfigurationName": "Device Configuration Name value",
  "platformType": "androidForWork",
  "restrictedAppsState": "notApprovedApps",
  "restrictedApps": [
    {
      "@odata.type": "microsoft.graph.managedDeviceReportedApp",
      "appId": "App Id value"
    }
  ]
}
```




