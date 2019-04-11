---
title: Criar restrictedAppsViolation
description: Criar um novo objeto restrictedAppsViolation.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b1c207bc34403f831d86d9849faf2287210d7bb5
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31778632"
---
# <a name="create-restrictedappsviolation"></a><span data-ttu-id="6b800-103">Criar restrictedAppsViolation</span><span class="sxs-lookup"><span data-stu-id="6b800-103">Create restrictedAppsViolation</span></span>

> <span data-ttu-id="6b800-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="6b800-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6b800-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6b800-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6b800-106">Criar um novo objeto [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) .</span><span class="sxs-lookup"><span data-stu-id="6b800-106">Create a new [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6b800-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="6b800-107">Prerequisites</span></span>
<span data-ttu-id="6b800-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6b800-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6b800-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6b800-110">Permission type</span></span>|<span data-ttu-id="6b800-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="6b800-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6b800-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6b800-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6b800-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6b800-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6b800-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6b800-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6b800-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6b800-115">Not supported.</span></span>|
|<span data-ttu-id="6b800-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6b800-116">Application</span></span>|<span data-ttu-id="6b800-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6b800-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6b800-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6b800-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurationRestrictedAppsViolations
```

## <a name="request-headers"></a><span data-ttu-id="6b800-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6b800-119">Request headers</span></span>
|<span data-ttu-id="6b800-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6b800-120">Header</span></span>|<span data-ttu-id="6b800-121">Valor</span><span class="sxs-lookup"><span data-stu-id="6b800-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6b800-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="6b800-122">Authorization</span></span>|<span data-ttu-id="6b800-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6b800-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6b800-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="6b800-124">Accept</span></span>|<span data-ttu-id="6b800-125">application/json</span><span class="sxs-lookup"><span data-stu-id="6b800-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6b800-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6b800-126">Request body</span></span>
<span data-ttu-id="6b800-127">No corpo da solicitação, forneça uma representação JSON do objeto restrictedAppsViolation.</span><span class="sxs-lookup"><span data-stu-id="6b800-127">In the request body, supply a JSON representation for the restrictedAppsViolation object.</span></span>

<span data-ttu-id="6b800-128">A tabela a seguir mostra as propriedades que são necessárias ao criar restrictedAppsViolation.</span><span class="sxs-lookup"><span data-stu-id="6b800-128">The following table shows the properties that are required when you create the restrictedAppsViolation.</span></span>

|<span data-ttu-id="6b800-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6b800-129">Property</span></span>|<span data-ttu-id="6b800-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="6b800-130">Type</span></span>|<span data-ttu-id="6b800-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="6b800-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6b800-132">id</span><span class="sxs-lookup"><span data-stu-id="6b800-132">id</span></span>|<span data-ttu-id="6b800-133">String</span><span class="sxs-lookup"><span data-stu-id="6b800-133">String</span></span>|<span data-ttu-id="6b800-134">Identificador exclusivo do objeto.</span><span class="sxs-lookup"><span data-stu-id="6b800-134">Unique identifier for the object.</span></span> <span data-ttu-id="6b800-135">Composto de AccountId, DeviceID, PolicyId e userId</span><span class="sxs-lookup"><span data-stu-id="6b800-135">Composed from accountId, deviceId, policyId and userId</span></span>|
|<span data-ttu-id="6b800-136">userId</span><span class="sxs-lookup"><span data-stu-id="6b800-136">userId</span></span>|<span data-ttu-id="6b800-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6b800-137">String</span></span>|<span data-ttu-id="6b800-138">O identificador exclusivo do usuário deve ser GUID</span><span class="sxs-lookup"><span data-stu-id="6b800-138">User unique identifier, must be Guid</span></span>|
|<span data-ttu-id="6b800-139">userName</span><span class="sxs-lookup"><span data-stu-id="6b800-139">userName</span></span>|<span data-ttu-id="6b800-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6b800-140">String</span></span>|<span data-ttu-id="6b800-141">Nome de usuário</span><span class="sxs-lookup"><span data-stu-id="6b800-141">User name</span></span>|
|<span data-ttu-id="6b800-142">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="6b800-142">managedDeviceId</span></span>|<span data-ttu-id="6b800-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6b800-143">String</span></span>|<span data-ttu-id="6b800-144">O identificador exclusivo do dispositivo gerenciado deve ser GUID</span><span class="sxs-lookup"><span data-stu-id="6b800-144">Managed device unique identifier, must be Guid</span></span>|
|<span data-ttu-id="6b800-145">deviceName</span><span class="sxs-lookup"><span data-stu-id="6b800-145">deviceName</span></span>|<span data-ttu-id="6b800-146">String</span><span class="sxs-lookup"><span data-stu-id="6b800-146">String</span></span>|<span data-ttu-id="6b800-147">Nome do dispositivo</span><span class="sxs-lookup"><span data-stu-id="6b800-147">Device name</span></span>|
|<span data-ttu-id="6b800-148">deviceConfigurationId</span><span class="sxs-lookup"><span data-stu-id="6b800-148">deviceConfigurationId</span></span>|<span data-ttu-id="6b800-149">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6b800-149">String</span></span>|<span data-ttu-id="6b800-150">O identificador exclusivo do perfil de configuração do dispositivo deve ser GUID</span><span class="sxs-lookup"><span data-stu-id="6b800-150">Device configuration profile unique identifier, must be Guid</span></span>|
|<span data-ttu-id="6b800-151">deviceConfigurationName</span><span class="sxs-lookup"><span data-stu-id="6b800-151">deviceConfigurationName</span></span>|<span data-ttu-id="6b800-152">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6b800-152">String</span></span>|<span data-ttu-id="6b800-153">Nome do perfil de configuração do dispositivo</span><span class="sxs-lookup"><span data-stu-id="6b800-153">Device configuration profile name</span></span>|
|<span data-ttu-id="6b800-154">platformType</span><span class="sxs-lookup"><span data-stu-id="6b800-154">platformType</span></span>|[<span data-ttu-id="6b800-155">policyPlatformType</span><span class="sxs-lookup"><span data-stu-id="6b800-155">policyPlatformType</span></span>](../resources/intune-deviceconfig-policyplatformtype.md)|<span data-ttu-id="6b800-156">Tipo de plataforma.</span><span class="sxs-lookup"><span data-stu-id="6b800-156">Platform type.</span></span> <span data-ttu-id="6b800-157">Os valores possíveis são: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.</span><span class="sxs-lookup"><span data-stu-id="6b800-157">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.</span></span>|
|<span data-ttu-id="6b800-158">restrictedAppsState</span><span class="sxs-lookup"><span data-stu-id="6b800-158">restrictedAppsState</span></span>|[<span data-ttu-id="6b800-159">restrictedAppsState</span><span class="sxs-lookup"><span data-stu-id="6b800-159">restrictedAppsState</span></span>](../resources/intune-deviceconfig-restrictedappsstate.md)|<span data-ttu-id="6b800-160">Estado de aplicativos restritos.</span><span class="sxs-lookup"><span data-stu-id="6b800-160">Restricted apps state.</span></span> <span data-ttu-id="6b800-161">Os valores possíveis são: `prohibitedApps` e `notApprovedApps`.</span><span class="sxs-lookup"><span data-stu-id="6b800-161">Possible values are: `prohibitedApps`, `notApprovedApps`.</span></span>|
|<span data-ttu-id="6b800-162">restrictedApps</span><span class="sxs-lookup"><span data-stu-id="6b800-162">restrictedApps</span></span>|<span data-ttu-id="6b800-163">coleção [managedDeviceReportedApp](../resources/intune-deviceconfig-manageddevicereportedapp.md)</span><span class="sxs-lookup"><span data-stu-id="6b800-163">[managedDeviceReportedApp](../resources/intune-deviceconfig-manageddevicereportedapp.md) collection</span></span>|<span data-ttu-id="6b800-164">Lista de aplicativos restritos violados</span><span class="sxs-lookup"><span data-stu-id="6b800-164">List of violated restricted apps</span></span>|



## <a name="response"></a><span data-ttu-id="6b800-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="6b800-165">Response</span></span>
<span data-ttu-id="6b800-166">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6b800-166">If successful, this method returns a `201 Created` response code and a [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6b800-167">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6b800-167">Example</span></span>

### <a name="request"></a><span data-ttu-id="6b800-168">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6b800-168">Request</span></span>
<span data-ttu-id="6b800-169">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6b800-169">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="6b800-170">Resposta</span><span class="sxs-lookup"><span data-stu-id="6b800-170">Response</span></span>
<span data-ttu-id="6b800-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6b800-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





