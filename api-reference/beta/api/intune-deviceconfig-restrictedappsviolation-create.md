---
title: Criar restrictedAppsViolation
description: Criar um novo objeto restrictedAppsViolation.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 9b3556293fee01cbb89133dcf9e0e79717e4d0f2
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43431822"
---
# <a name="create-restrictedappsviolation"></a><span data-ttu-id="55318-103">Criar restrictedAppsViolation</span><span class="sxs-lookup"><span data-stu-id="55318-103">Create restrictedAppsViolation</span></span>

<span data-ttu-id="55318-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="55318-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="55318-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="55318-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="55318-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="55318-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="55318-107">Criar um novo objeto [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) .</span><span class="sxs-lookup"><span data-stu-id="55318-107">Create a new [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="55318-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="55318-108">Prerequisites</span></span>
<span data-ttu-id="55318-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="55318-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="55318-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="55318-111">Permission type</span></span>|<span data-ttu-id="55318-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="55318-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="55318-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="55318-113">Delegated (work or school account)</span></span>|<span data-ttu-id="55318-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="55318-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="55318-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="55318-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="55318-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="55318-116">Not supported.</span></span>|
|<span data-ttu-id="55318-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="55318-117">Application</span></span>|<span data-ttu-id="55318-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="55318-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="55318-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="55318-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurationRestrictedAppsViolations
```

## <a name="request-headers"></a><span data-ttu-id="55318-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="55318-120">Request headers</span></span>
|<span data-ttu-id="55318-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="55318-121">Header</span></span>|<span data-ttu-id="55318-122">Valor</span><span class="sxs-lookup"><span data-stu-id="55318-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="55318-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="55318-123">Authorization</span></span>|<span data-ttu-id="55318-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="55318-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="55318-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="55318-125">Accept</span></span>|<span data-ttu-id="55318-126">application/json</span><span class="sxs-lookup"><span data-stu-id="55318-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="55318-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="55318-127">Request body</span></span>
<span data-ttu-id="55318-128">No corpo da solicitação, forneça uma representação JSON do objeto restrictedAppsViolation.</span><span class="sxs-lookup"><span data-stu-id="55318-128">In the request body, supply a JSON representation for the restrictedAppsViolation object.</span></span>

<span data-ttu-id="55318-129">A tabela a seguir mostra as propriedades que são necessárias ao criar restrictedAppsViolation.</span><span class="sxs-lookup"><span data-stu-id="55318-129">The following table shows the properties that are required when you create the restrictedAppsViolation.</span></span>

|<span data-ttu-id="55318-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="55318-130">Property</span></span>|<span data-ttu-id="55318-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="55318-131">Type</span></span>|<span data-ttu-id="55318-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="55318-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="55318-133">id</span><span class="sxs-lookup"><span data-stu-id="55318-133">id</span></span>|<span data-ttu-id="55318-134">String</span><span class="sxs-lookup"><span data-stu-id="55318-134">String</span></span>|<span data-ttu-id="55318-135">Identificador exclusivo do objeto.</span><span class="sxs-lookup"><span data-stu-id="55318-135">Unique identifier for the object.</span></span> <span data-ttu-id="55318-136">Composto de AccountId, DeviceID, PolicyId e userId</span><span class="sxs-lookup"><span data-stu-id="55318-136">Composed from accountId, deviceId, policyId and userId</span></span>|
|<span data-ttu-id="55318-137">userId</span><span class="sxs-lookup"><span data-stu-id="55318-137">userId</span></span>|<span data-ttu-id="55318-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="55318-138">String</span></span>|<span data-ttu-id="55318-139">O identificador exclusivo do usuário deve ser GUID</span><span class="sxs-lookup"><span data-stu-id="55318-139">User unique identifier, must be Guid</span></span>|
|<span data-ttu-id="55318-140">userName</span><span class="sxs-lookup"><span data-stu-id="55318-140">userName</span></span>|<span data-ttu-id="55318-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="55318-141">String</span></span>|<span data-ttu-id="55318-142">Nome de usuário</span><span class="sxs-lookup"><span data-stu-id="55318-142">User name</span></span>|
|<span data-ttu-id="55318-143">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="55318-143">managedDeviceId</span></span>|<span data-ttu-id="55318-144">String</span><span class="sxs-lookup"><span data-stu-id="55318-144">String</span></span>|<span data-ttu-id="55318-145">O identificador exclusivo do dispositivo gerenciado deve ser GUID</span><span class="sxs-lookup"><span data-stu-id="55318-145">Managed device unique identifier, must be Guid</span></span>|
|<span data-ttu-id="55318-146">deviceName</span><span class="sxs-lookup"><span data-stu-id="55318-146">deviceName</span></span>|<span data-ttu-id="55318-147">String</span><span class="sxs-lookup"><span data-stu-id="55318-147">String</span></span>|<span data-ttu-id="55318-148">Nome do dispositivo</span><span class="sxs-lookup"><span data-stu-id="55318-148">Device name</span></span>|
|<span data-ttu-id="55318-149">deviceConfigurationId</span><span class="sxs-lookup"><span data-stu-id="55318-149">deviceConfigurationId</span></span>|<span data-ttu-id="55318-150">String</span><span class="sxs-lookup"><span data-stu-id="55318-150">String</span></span>|<span data-ttu-id="55318-151">O identificador exclusivo do perfil de configuração do dispositivo deve ser GUID</span><span class="sxs-lookup"><span data-stu-id="55318-151">Device configuration profile unique identifier, must be Guid</span></span>|
|<span data-ttu-id="55318-152">deviceConfigurationName</span><span class="sxs-lookup"><span data-stu-id="55318-152">deviceConfigurationName</span></span>|<span data-ttu-id="55318-153">String</span><span class="sxs-lookup"><span data-stu-id="55318-153">String</span></span>|<span data-ttu-id="55318-154">Nome do perfil de configuração do dispositivo</span><span class="sxs-lookup"><span data-stu-id="55318-154">Device configuration profile name</span></span>|
|<span data-ttu-id="55318-155">platformType</span><span class="sxs-lookup"><span data-stu-id="55318-155">platformType</span></span>|[<span data-ttu-id="55318-156">policyPlatformType</span><span class="sxs-lookup"><span data-stu-id="55318-156">policyPlatformType</span></span>](../resources/intune-shared-policyplatformtype.md)|<span data-ttu-id="55318-157">Tipo de plataforma.</span><span class="sxs-lookup"><span data-stu-id="55318-157">Platform type.</span></span> <span data-ttu-id="55318-158">Os valores possíveis são: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `windows10XProfile`, `all`.</span><span class="sxs-lookup"><span data-stu-id="55318-158">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `windows10XProfile`, `all`.</span></span>|
|<span data-ttu-id="55318-159">restrictedAppsState</span><span class="sxs-lookup"><span data-stu-id="55318-159">restrictedAppsState</span></span>|[<span data-ttu-id="55318-160">restrictedAppsState</span><span class="sxs-lookup"><span data-stu-id="55318-160">restrictedAppsState</span></span>](../resources/intune-deviceconfig-restrictedappsstate.md)|<span data-ttu-id="55318-161">Estado de aplicativos restritos.</span><span class="sxs-lookup"><span data-stu-id="55318-161">Restricted apps state.</span></span> <span data-ttu-id="55318-162">Os valores possíveis são: `prohibitedApps` e `notApprovedApps`.</span><span class="sxs-lookup"><span data-stu-id="55318-162">Possible values are: `prohibitedApps`, `notApprovedApps`.</span></span>|
|<span data-ttu-id="55318-163">restrictedApps</span><span class="sxs-lookup"><span data-stu-id="55318-163">restrictedApps</span></span>|<span data-ttu-id="55318-164">coleção [managedDeviceReportedApp](../resources/intune-deviceconfig-manageddevicereportedapp.md)</span><span class="sxs-lookup"><span data-stu-id="55318-164">[managedDeviceReportedApp](../resources/intune-deviceconfig-manageddevicereportedapp.md) collection</span></span>|<span data-ttu-id="55318-165">Lista de aplicativos restritos violados</span><span class="sxs-lookup"><span data-stu-id="55318-165">List of violated restricted apps</span></span>|



## <a name="response"></a><span data-ttu-id="55318-166">Resposta</span><span class="sxs-lookup"><span data-stu-id="55318-166">Response</span></span>
<span data-ttu-id="55318-167">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="55318-167">If successful, this method returns a `201 Created` response code and a [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="55318-168">Exemplo</span><span class="sxs-lookup"><span data-stu-id="55318-168">Example</span></span>

### <a name="request"></a><span data-ttu-id="55318-169">Solicitação</span><span class="sxs-lookup"><span data-stu-id="55318-169">Request</span></span>
<span data-ttu-id="55318-170">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="55318-170">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurationRestrictedAppsViolations
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

### <a name="response"></a><span data-ttu-id="55318-171">Resposta</span><span class="sxs-lookup"><span data-stu-id="55318-171">Response</span></span>
<span data-ttu-id="55318-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="55318-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



