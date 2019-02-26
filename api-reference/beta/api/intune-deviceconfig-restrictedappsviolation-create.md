---
title: Criar restrictedAppsViolation
description: Criar um novo objeto restrictedAppsViolation.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: fbba9348e8b97125651951bdb4df424dc3b9fe47
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30146400"
---
# <a name="create-restrictedappsviolation"></a><span data-ttu-id="407a1-103">Criar restrictedAppsViolation</span><span class="sxs-lookup"><span data-stu-id="407a1-103">Create restrictedAppsViolation</span></span>

> <span data-ttu-id="407a1-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="407a1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="407a1-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="407a1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="407a1-106">Criar um novo objeto [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) .</span><span class="sxs-lookup"><span data-stu-id="407a1-106">Create a new [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="407a1-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="407a1-107">Prerequisites</span></span>
<span data-ttu-id="407a1-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="407a1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="407a1-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="407a1-110">Permission type</span></span>|<span data-ttu-id="407a1-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="407a1-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="407a1-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="407a1-112">Delegated (work or school account)</span></span>|<span data-ttu-id="407a1-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="407a1-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="407a1-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="407a1-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="407a1-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="407a1-115">Not supported.</span></span>|
|<span data-ttu-id="407a1-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="407a1-116">Application</span></span>|<span data-ttu-id="407a1-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="407a1-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="407a1-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="407a1-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurationRestrictedAppsViolations
```

## <a name="request-headers"></a><span data-ttu-id="407a1-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="407a1-119">Request headers</span></span>
|<span data-ttu-id="407a1-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="407a1-120">Header</span></span>|<span data-ttu-id="407a1-121">Valor</span><span class="sxs-lookup"><span data-stu-id="407a1-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="407a1-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="407a1-122">Authorization</span></span>|<span data-ttu-id="407a1-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="407a1-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="407a1-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="407a1-124">Accept</span></span>|<span data-ttu-id="407a1-125">application/json</span><span class="sxs-lookup"><span data-stu-id="407a1-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="407a1-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="407a1-126">Request body</span></span>
<span data-ttu-id="407a1-127">No corpo da solicitação, forneça uma representação JSON do objeto restrictedAppsViolation.</span><span class="sxs-lookup"><span data-stu-id="407a1-127">In the request body, supply a JSON representation for the restrictedAppsViolation object.</span></span>

<span data-ttu-id="407a1-128">A tabela a seguir mostra as propriedades que são necessárias ao criar restrictedAppsViolation.</span><span class="sxs-lookup"><span data-stu-id="407a1-128">The following table shows the properties that are required when you create the restrictedAppsViolation.</span></span>

|<span data-ttu-id="407a1-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="407a1-129">Property</span></span>|<span data-ttu-id="407a1-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="407a1-130">Type</span></span>|<span data-ttu-id="407a1-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="407a1-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="407a1-132">id</span><span class="sxs-lookup"><span data-stu-id="407a1-132">id</span></span>|<span data-ttu-id="407a1-133">String</span><span class="sxs-lookup"><span data-stu-id="407a1-133">String</span></span>|<span data-ttu-id="407a1-134">Identificador exclusivo do objeto.</span><span class="sxs-lookup"><span data-stu-id="407a1-134">Unique identifier for the object.</span></span> <span data-ttu-id="407a1-135">Composto de AccountId, DeviceID, PolicyId e userId</span><span class="sxs-lookup"><span data-stu-id="407a1-135">Composed from accountId, deviceId, policyId and userId</span></span>|
|<span data-ttu-id="407a1-136">userId</span><span class="sxs-lookup"><span data-stu-id="407a1-136">userId</span></span>|<span data-ttu-id="407a1-137">String</span><span class="sxs-lookup"><span data-stu-id="407a1-137">String</span></span>|<span data-ttu-id="407a1-138">O identificador exclusivo do usuário deve ser GUID</span><span class="sxs-lookup"><span data-stu-id="407a1-138">User unique identifier, must be Guid</span></span>|
|<span data-ttu-id="407a1-139">userName</span><span class="sxs-lookup"><span data-stu-id="407a1-139">userName</span></span>|<span data-ttu-id="407a1-140">String</span><span class="sxs-lookup"><span data-stu-id="407a1-140">String</span></span>|<span data-ttu-id="407a1-141">Nome de usuário</span><span class="sxs-lookup"><span data-stu-id="407a1-141">User name</span></span>|
|<span data-ttu-id="407a1-142">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="407a1-142">managedDeviceId</span></span>|<span data-ttu-id="407a1-143">String</span><span class="sxs-lookup"><span data-stu-id="407a1-143">String</span></span>|<span data-ttu-id="407a1-144">O identificador exclusivo do dispositivo gerenciado deve ser GUID</span><span class="sxs-lookup"><span data-stu-id="407a1-144">Managed device unique identifier, must be Guid</span></span>|
|<span data-ttu-id="407a1-145">deviceName</span><span class="sxs-lookup"><span data-stu-id="407a1-145">deviceName</span></span>|<span data-ttu-id="407a1-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="407a1-146">String</span></span>|<span data-ttu-id="407a1-147">Nome do dispositivo</span><span class="sxs-lookup"><span data-stu-id="407a1-147">Device name</span></span>|
|<span data-ttu-id="407a1-148">deviceConfigurationId</span><span class="sxs-lookup"><span data-stu-id="407a1-148">deviceConfigurationId</span></span>|<span data-ttu-id="407a1-149">String</span><span class="sxs-lookup"><span data-stu-id="407a1-149">String</span></span>|<span data-ttu-id="407a1-150">O identificador exclusivo do perfil de configuração do dispositivo deve ser GUID</span><span class="sxs-lookup"><span data-stu-id="407a1-150">Device configuration profile unique identifier, must be Guid</span></span>|
|<span data-ttu-id="407a1-151">deviceConfigurationName</span><span class="sxs-lookup"><span data-stu-id="407a1-151">deviceConfigurationName</span></span>|<span data-ttu-id="407a1-152">String</span><span class="sxs-lookup"><span data-stu-id="407a1-152">String</span></span>|<span data-ttu-id="407a1-153">Nome do perfil de configuração do dispositivo</span><span class="sxs-lookup"><span data-stu-id="407a1-153">Device configuration profile name</span></span>|
|<span data-ttu-id="407a1-154">platformType</span><span class="sxs-lookup"><span data-stu-id="407a1-154">platformType</span></span>|[<span data-ttu-id="407a1-155">policyPlatformType</span><span class="sxs-lookup"><span data-stu-id="407a1-155">policyPlatformType</span></span>](../resources/intune-deviceconfig-policyplatformtype.md)|<span data-ttu-id="407a1-156">Tipo de plataforma.</span><span class="sxs-lookup"><span data-stu-id="407a1-156">Platform type.</span></span> <span data-ttu-id="407a1-157">Os valores possíveis são: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.</span><span class="sxs-lookup"><span data-stu-id="407a1-157">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.</span></span>|
|<span data-ttu-id="407a1-158">restrictedAppsState</span><span class="sxs-lookup"><span data-stu-id="407a1-158">restrictedAppsState</span></span>|[<span data-ttu-id="407a1-159">restrictedAppsState</span><span class="sxs-lookup"><span data-stu-id="407a1-159">restrictedAppsState</span></span>](../resources/intune-deviceconfig-restrictedappsstate.md)|<span data-ttu-id="407a1-160">Estado de aplicativos restritos.</span><span class="sxs-lookup"><span data-stu-id="407a1-160">Restricted apps state.</span></span> <span data-ttu-id="407a1-161">Os valores possíveis são: `prohibitedApps` e `notApprovedApps`.</span><span class="sxs-lookup"><span data-stu-id="407a1-161">Possible values are: `prohibitedApps`, `notApprovedApps`.</span></span>|
|<span data-ttu-id="407a1-162">restrictedApps</span><span class="sxs-lookup"><span data-stu-id="407a1-162">restrictedApps</span></span>|<span data-ttu-id="407a1-163">coleção [managedDeviceReportedApp](../resources/intune-deviceconfig-manageddevicereportedapp.md)</span><span class="sxs-lookup"><span data-stu-id="407a1-163">[managedDeviceReportedApp](../resources/intune-deviceconfig-manageddevicereportedapp.md) collection</span></span>|<span data-ttu-id="407a1-164">Lista de aplicativos restritos violados</span><span class="sxs-lookup"><span data-stu-id="407a1-164">List of violated restricted apps</span></span>|



## <a name="response"></a><span data-ttu-id="407a1-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="407a1-165">Response</span></span>
<span data-ttu-id="407a1-166">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="407a1-166">If successful, this method returns a `201 Created` response code and a [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="407a1-167">Exemplo</span><span class="sxs-lookup"><span data-stu-id="407a1-167">Example</span></span>

### <a name="request"></a><span data-ttu-id="407a1-168">Solicitação</span><span class="sxs-lookup"><span data-stu-id="407a1-168">Request</span></span>
<span data-ttu-id="407a1-169">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="407a1-169">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="407a1-170">Resposta</span><span class="sxs-lookup"><span data-stu-id="407a1-170">Response</span></span>
<span data-ttu-id="407a1-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="407a1-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




