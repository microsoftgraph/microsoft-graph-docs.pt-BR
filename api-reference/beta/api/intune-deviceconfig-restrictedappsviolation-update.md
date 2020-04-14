---
title: Atualizar restrictedAppsViolation
description: Atualiza as propriedades de um objeto restrictedAppsViolation.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 4055cbfd6a25d718e97c0fc874b7d450b19598a6
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43431664"
---
# <a name="update-restrictedappsviolation"></a><span data-ttu-id="cf559-103">Atualizar restrictedAppsViolation</span><span class="sxs-lookup"><span data-stu-id="cf559-103">Update restrictedAppsViolation</span></span>

<span data-ttu-id="cf559-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cf559-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="cf559-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="cf559-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cf559-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="cf559-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cf559-107">Atualiza as propriedades de um objeto [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) .</span><span class="sxs-lookup"><span data-stu-id="cf559-107">Update the properties of a [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cf559-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="cf559-108">Prerequisites</span></span>
<span data-ttu-id="cf559-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cf559-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cf559-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cf559-111">Permission type</span></span>|<span data-ttu-id="cf559-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="cf559-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cf559-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cf559-113">Delegated (work or school account)</span></span>|<span data-ttu-id="cf559-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cf559-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="cf559-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cf559-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cf559-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cf559-116">Not supported.</span></span>|
|<span data-ttu-id="cf559-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cf559-117">Application</span></span>|<span data-ttu-id="cf559-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cf559-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="cf559-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cf559-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurationRestrictedAppsViolations/{restrictedAppsViolationId}
```

## <a name="request-headers"></a><span data-ttu-id="cf559-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cf559-120">Request headers</span></span>
|<span data-ttu-id="cf559-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="cf559-121">Header</span></span>|<span data-ttu-id="cf559-122">Valor</span><span class="sxs-lookup"><span data-stu-id="cf559-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cf559-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="cf559-123">Authorization</span></span>|<span data-ttu-id="cf559-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cf559-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cf559-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="cf559-125">Accept</span></span>|<span data-ttu-id="cf559-126">application/json</span><span class="sxs-lookup"><span data-stu-id="cf559-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cf559-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cf559-127">Request body</span></span>
<span data-ttu-id="cf559-128">No corpo da solicitação, forneça uma representação JSON do objeto [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) .</span><span class="sxs-lookup"><span data-stu-id="cf559-128">In the request body, supply a JSON representation for the [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) object.</span></span>

<span data-ttu-id="cf559-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md).</span><span class="sxs-lookup"><span data-stu-id="cf559-129">The following table shows the properties that are required when you create the [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md).</span></span>

|<span data-ttu-id="cf559-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cf559-130">Property</span></span>|<span data-ttu-id="cf559-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="cf559-131">Type</span></span>|<span data-ttu-id="cf559-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="cf559-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cf559-133">id</span><span class="sxs-lookup"><span data-stu-id="cf559-133">id</span></span>|<span data-ttu-id="cf559-134">String</span><span class="sxs-lookup"><span data-stu-id="cf559-134">String</span></span>|<span data-ttu-id="cf559-135">Identificador exclusivo do objeto.</span><span class="sxs-lookup"><span data-stu-id="cf559-135">Unique identifier for the object.</span></span> <span data-ttu-id="cf559-136">Composto de AccountId, DeviceID, PolicyId e userId</span><span class="sxs-lookup"><span data-stu-id="cf559-136">Composed from accountId, deviceId, policyId and userId</span></span>|
|<span data-ttu-id="cf559-137">userId</span><span class="sxs-lookup"><span data-stu-id="cf559-137">userId</span></span>|<span data-ttu-id="cf559-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cf559-138">String</span></span>|<span data-ttu-id="cf559-139">O identificador exclusivo do usuário deve ser GUID</span><span class="sxs-lookup"><span data-stu-id="cf559-139">User unique identifier, must be Guid</span></span>|
|<span data-ttu-id="cf559-140">userName</span><span class="sxs-lookup"><span data-stu-id="cf559-140">userName</span></span>|<span data-ttu-id="cf559-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cf559-141">String</span></span>|<span data-ttu-id="cf559-142">Nome de usuário</span><span class="sxs-lookup"><span data-stu-id="cf559-142">User name</span></span>|
|<span data-ttu-id="cf559-143">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="cf559-143">managedDeviceId</span></span>|<span data-ttu-id="cf559-144">String</span><span class="sxs-lookup"><span data-stu-id="cf559-144">String</span></span>|<span data-ttu-id="cf559-145">O identificador exclusivo do dispositivo gerenciado deve ser GUID</span><span class="sxs-lookup"><span data-stu-id="cf559-145">Managed device unique identifier, must be Guid</span></span>|
|<span data-ttu-id="cf559-146">deviceName</span><span class="sxs-lookup"><span data-stu-id="cf559-146">deviceName</span></span>|<span data-ttu-id="cf559-147">String</span><span class="sxs-lookup"><span data-stu-id="cf559-147">String</span></span>|<span data-ttu-id="cf559-148">Nome do dispositivo</span><span class="sxs-lookup"><span data-stu-id="cf559-148">Device name</span></span>|
|<span data-ttu-id="cf559-149">deviceConfigurationId</span><span class="sxs-lookup"><span data-stu-id="cf559-149">deviceConfigurationId</span></span>|<span data-ttu-id="cf559-150">String</span><span class="sxs-lookup"><span data-stu-id="cf559-150">String</span></span>|<span data-ttu-id="cf559-151">O identificador exclusivo do perfil de configuração do dispositivo deve ser GUID</span><span class="sxs-lookup"><span data-stu-id="cf559-151">Device configuration profile unique identifier, must be Guid</span></span>|
|<span data-ttu-id="cf559-152">deviceConfigurationName</span><span class="sxs-lookup"><span data-stu-id="cf559-152">deviceConfigurationName</span></span>|<span data-ttu-id="cf559-153">String</span><span class="sxs-lookup"><span data-stu-id="cf559-153">String</span></span>|<span data-ttu-id="cf559-154">Nome do perfil de configuração do dispositivo</span><span class="sxs-lookup"><span data-stu-id="cf559-154">Device configuration profile name</span></span>|
|<span data-ttu-id="cf559-155">platformType</span><span class="sxs-lookup"><span data-stu-id="cf559-155">platformType</span></span>|[<span data-ttu-id="cf559-156">policyPlatformType</span><span class="sxs-lookup"><span data-stu-id="cf559-156">policyPlatformType</span></span>](../resources/intune-shared-policyplatformtype.md)|<span data-ttu-id="cf559-157">Tipo de plataforma.</span><span class="sxs-lookup"><span data-stu-id="cf559-157">Platform type.</span></span> <span data-ttu-id="cf559-158">Os valores possíveis são: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `windows10XProfile`, `all`.</span><span class="sxs-lookup"><span data-stu-id="cf559-158">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `windows10XProfile`, `all`.</span></span>|
|<span data-ttu-id="cf559-159">restrictedAppsState</span><span class="sxs-lookup"><span data-stu-id="cf559-159">restrictedAppsState</span></span>|[<span data-ttu-id="cf559-160">restrictedAppsState</span><span class="sxs-lookup"><span data-stu-id="cf559-160">restrictedAppsState</span></span>](../resources/intune-deviceconfig-restrictedappsstate.md)|<span data-ttu-id="cf559-161">Estado de aplicativos restritos.</span><span class="sxs-lookup"><span data-stu-id="cf559-161">Restricted apps state.</span></span> <span data-ttu-id="cf559-162">Os valores possíveis são: `prohibitedApps` e `notApprovedApps`.</span><span class="sxs-lookup"><span data-stu-id="cf559-162">Possible values are: `prohibitedApps`, `notApprovedApps`.</span></span>|
|<span data-ttu-id="cf559-163">restrictedApps</span><span class="sxs-lookup"><span data-stu-id="cf559-163">restrictedApps</span></span>|<span data-ttu-id="cf559-164">coleção [managedDeviceReportedApp](../resources/intune-deviceconfig-manageddevicereportedapp.md)</span><span class="sxs-lookup"><span data-stu-id="cf559-164">[managedDeviceReportedApp](../resources/intune-deviceconfig-manageddevicereportedapp.md) collection</span></span>|<span data-ttu-id="cf559-165">Lista de aplicativos restritos violados</span><span class="sxs-lookup"><span data-stu-id="cf559-165">List of violated restricted apps</span></span>|



## <a name="response"></a><span data-ttu-id="cf559-166">Resposta</span><span class="sxs-lookup"><span data-stu-id="cf559-166">Response</span></span>
<span data-ttu-id="cf559-167">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cf559-167">If successful, this method returns a `200 OK` response code and an updated [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cf559-168">Exemplo</span><span class="sxs-lookup"><span data-stu-id="cf559-168">Example</span></span>

### <a name="request"></a><span data-ttu-id="cf559-169">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cf559-169">Request</span></span>
<span data-ttu-id="cf559-170">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="cf559-170">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="cf559-171">Resposta</span><span class="sxs-lookup"><span data-stu-id="cf559-171">Response</span></span>
<span data-ttu-id="cf559-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="cf559-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



