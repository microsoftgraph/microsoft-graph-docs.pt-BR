---
title: Atualizar restrictedAppsViolation
description: Atualize as propriedades de um objeto restrictedAppsViolation.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 4b0e600358463916219109b1123413d9f69b2d44
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51132468"
---
# <a name="update-restrictedappsviolation"></a><span data-ttu-id="921a9-103">Atualizar restrictedAppsViolation</span><span class="sxs-lookup"><span data-stu-id="921a9-103">Update restrictedAppsViolation</span></span>

<span data-ttu-id="921a9-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="921a9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="921a9-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="921a9-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="921a9-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="921a9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="921a9-107">Atualize as propriedades de [um objeto restrictedAppsViolation.](../resources/intune-deviceconfig-restrictedappsviolation.md)</span><span class="sxs-lookup"><span data-stu-id="921a9-107">Update the properties of a [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="921a9-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="921a9-108">Prerequisites</span></span>
<span data-ttu-id="921a9-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="921a9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="921a9-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="921a9-111">Permission type</span></span>|<span data-ttu-id="921a9-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="921a9-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="921a9-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="921a9-113">Delegated (work or school account)</span></span>|<span data-ttu-id="921a9-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="921a9-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="921a9-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="921a9-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="921a9-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="921a9-116">Not supported.</span></span>|
|<span data-ttu-id="921a9-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="921a9-117">Application</span></span>|<span data-ttu-id="921a9-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="921a9-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="921a9-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="921a9-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurationRestrictedAppsViolations/{restrictedAppsViolationId}
```

## <a name="request-headers"></a><span data-ttu-id="921a9-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="921a9-120">Request headers</span></span>
|<span data-ttu-id="921a9-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="921a9-121">Header</span></span>|<span data-ttu-id="921a9-122">Valor</span><span class="sxs-lookup"><span data-stu-id="921a9-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="921a9-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="921a9-123">Authorization</span></span>|<span data-ttu-id="921a9-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="921a9-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="921a9-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="921a9-125">Accept</span></span>|<span data-ttu-id="921a9-126">application/json</span><span class="sxs-lookup"><span data-stu-id="921a9-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="921a9-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="921a9-127">Request body</span></span>
<span data-ttu-id="921a9-128">No corpo da solicitação, fornece uma representação JSON para o objeto [restrictedAppsViolation.](../resources/intune-deviceconfig-restrictedappsviolation.md)</span><span class="sxs-lookup"><span data-stu-id="921a9-128">In the request body, supply a JSON representation for the [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) object.</span></span>

<span data-ttu-id="921a9-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [o restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md).</span><span class="sxs-lookup"><span data-stu-id="921a9-129">The following table shows the properties that are required when you create the [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md).</span></span>

|<span data-ttu-id="921a9-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="921a9-130">Property</span></span>|<span data-ttu-id="921a9-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="921a9-131">Type</span></span>|<span data-ttu-id="921a9-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="921a9-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="921a9-133">id</span><span class="sxs-lookup"><span data-stu-id="921a9-133">id</span></span>|<span data-ttu-id="921a9-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="921a9-134">String</span></span>|<span data-ttu-id="921a9-135">Identificador exclusivo do objeto.</span><span class="sxs-lookup"><span data-stu-id="921a9-135">Unique identifier for the object.</span></span> <span data-ttu-id="921a9-136">Composto por accountId, deviceId, policyId e userId</span><span class="sxs-lookup"><span data-stu-id="921a9-136">Composed from accountId, deviceId, policyId and userId</span></span>|
|<span data-ttu-id="921a9-137">userId</span><span class="sxs-lookup"><span data-stu-id="921a9-137">userId</span></span>|<span data-ttu-id="921a9-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="921a9-138">String</span></span>|<span data-ttu-id="921a9-139">Identificador exclusivo do usuário, deve ser Guid</span><span class="sxs-lookup"><span data-stu-id="921a9-139">User unique identifier, must be Guid</span></span>|
|<span data-ttu-id="921a9-140">userName</span><span class="sxs-lookup"><span data-stu-id="921a9-140">userName</span></span>|<span data-ttu-id="921a9-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="921a9-141">String</span></span>|<span data-ttu-id="921a9-142">Nome de usuário</span><span class="sxs-lookup"><span data-stu-id="921a9-142">User name</span></span>|
|<span data-ttu-id="921a9-143">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="921a9-143">managedDeviceId</span></span>|<span data-ttu-id="921a9-144">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="921a9-144">String</span></span>|<span data-ttu-id="921a9-145">Identificador exclusivo do dispositivo gerenciado, deve ser Guid</span><span class="sxs-lookup"><span data-stu-id="921a9-145">Managed device unique identifier, must be Guid</span></span>|
|<span data-ttu-id="921a9-146">deviceName</span><span class="sxs-lookup"><span data-stu-id="921a9-146">deviceName</span></span>|<span data-ttu-id="921a9-147">String</span><span class="sxs-lookup"><span data-stu-id="921a9-147">String</span></span>|<span data-ttu-id="921a9-148">Nome do dispositivo</span><span class="sxs-lookup"><span data-stu-id="921a9-148">Device name</span></span>|
|<span data-ttu-id="921a9-149">deviceConfigurationId</span><span class="sxs-lookup"><span data-stu-id="921a9-149">deviceConfigurationId</span></span>|<span data-ttu-id="921a9-150">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="921a9-150">String</span></span>|<span data-ttu-id="921a9-151">Identificador exclusivo do perfil de configuração do dispositivo, deve ser Guid</span><span class="sxs-lookup"><span data-stu-id="921a9-151">Device configuration profile unique identifier, must be Guid</span></span>|
|<span data-ttu-id="921a9-152">deviceConfigurationName</span><span class="sxs-lookup"><span data-stu-id="921a9-152">deviceConfigurationName</span></span>|<span data-ttu-id="921a9-153">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="921a9-153">String</span></span>|<span data-ttu-id="921a9-154">Nome do perfil de configuração do dispositivo</span><span class="sxs-lookup"><span data-stu-id="921a9-154">Device configuration profile name</span></span>|
|<span data-ttu-id="921a9-155">platformType</span><span class="sxs-lookup"><span data-stu-id="921a9-155">platformType</span></span>|[<span data-ttu-id="921a9-156">policyPlatformType</span><span class="sxs-lookup"><span data-stu-id="921a9-156">policyPlatformType</span></span>](../resources/intune-shared-policyplatformtype.md)|<span data-ttu-id="921a9-157">Tipo de plataforma.</span><span class="sxs-lookup"><span data-stu-id="921a9-157">Platform type.</span></span> <span data-ttu-id="921a9-158">Os valores possíveis são: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `windows10XProfile`, `all`.</span><span class="sxs-lookup"><span data-stu-id="921a9-158">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `windows10XProfile`, `all`.</span></span>|
|<span data-ttu-id="921a9-159">restrictedAppsState</span><span class="sxs-lookup"><span data-stu-id="921a9-159">restrictedAppsState</span></span>|[<span data-ttu-id="921a9-160">restrictedAppsState</span><span class="sxs-lookup"><span data-stu-id="921a9-160">restrictedAppsState</span></span>](../resources/intune-deviceconfig-restrictedappsstate.md)|<span data-ttu-id="921a9-161">Estado de aplicativos restritos.</span><span class="sxs-lookup"><span data-stu-id="921a9-161">Restricted apps state.</span></span> <span data-ttu-id="921a9-162">Os valores possíveis são: `prohibitedApps` e `notApprovedApps`.</span><span class="sxs-lookup"><span data-stu-id="921a9-162">Possible values are: `prohibitedApps`, `notApprovedApps`.</span></span>|
|<span data-ttu-id="921a9-163">restrictedApps</span><span class="sxs-lookup"><span data-stu-id="921a9-163">restrictedApps</span></span>|<span data-ttu-id="921a9-164">[Coleção managedDeviceReportedApp](../resources/intune-deviceconfig-manageddevicereportedapp.md)</span><span class="sxs-lookup"><span data-stu-id="921a9-164">[managedDeviceReportedApp](../resources/intune-deviceconfig-manageddevicereportedapp.md) collection</span></span>|<span data-ttu-id="921a9-165">Lista de aplicativos restritos violados</span><span class="sxs-lookup"><span data-stu-id="921a9-165">List of violated restricted apps</span></span>|



## <a name="response"></a><span data-ttu-id="921a9-166">Resposta</span><span class="sxs-lookup"><span data-stu-id="921a9-166">Response</span></span>
<span data-ttu-id="921a9-167">Se tiver êxito, este método retornará um código de resposta e um `200 OK` objeto [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="921a9-167">If successful, this method returns a `200 OK` response code and an updated [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="921a9-168">Exemplo</span><span class="sxs-lookup"><span data-stu-id="921a9-168">Example</span></span>

### <a name="request"></a><span data-ttu-id="921a9-169">Solicitação</span><span class="sxs-lookup"><span data-stu-id="921a9-169">Request</span></span>
<span data-ttu-id="921a9-170">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="921a9-170">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="921a9-171">Resposta</span><span class="sxs-lookup"><span data-stu-id="921a9-171">Response</span></span>
<span data-ttu-id="921a9-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="921a9-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




