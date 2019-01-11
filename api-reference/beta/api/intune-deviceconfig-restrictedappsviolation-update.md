---
title: Atualizar restrictedAppsViolation
description: Atualize as propriedades de um objeto restrictedAppsViolation.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 139a87dafc438e9710ff9494f8477658c61cca0d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27891571"
---
# <a name="update-restrictedappsviolation"></a><span data-ttu-id="c540b-103">Atualizar restrictedAppsViolation</span><span class="sxs-lookup"><span data-stu-id="c540b-103">Update restrictedAppsViolation</span></span>

> <span data-ttu-id="c540b-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="c540b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c540b-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="c540b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c540b-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="c540b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c540b-107">Atualize as propriedades de um objeto [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) .</span><span class="sxs-lookup"><span data-stu-id="c540b-107">Update the properties of a [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c540b-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c540b-108">Prerequisites</span></span>
<span data-ttu-id="c540b-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c540b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c540b-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c540b-111">Permission type</span></span>|<span data-ttu-id="c540b-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="c540b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c540b-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c540b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c540b-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c540b-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c540b-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c540b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c540b-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c540b-116">Not supported.</span></span>|
|<span data-ttu-id="c540b-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c540b-117">Application</span></span>|<span data-ttu-id="c540b-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c540b-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c540b-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c540b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurationRestrictedAppsViolations/{restrictedAppsViolationId}
```

## <a name="request-headers"></a><span data-ttu-id="c540b-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c540b-120">Request headers</span></span>
|<span data-ttu-id="c540b-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c540b-121">Header</span></span>|<span data-ttu-id="c540b-122">Valor</span><span class="sxs-lookup"><span data-stu-id="c540b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c540b-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="c540b-123">Authorization</span></span>|<span data-ttu-id="c540b-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c540b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c540b-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="c540b-125">Accept</span></span>|<span data-ttu-id="c540b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c540b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c540b-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c540b-127">Request body</span></span>
<span data-ttu-id="c540b-128">No corpo da solicitação, fornece uma representação JSON para o objeto [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) .</span><span class="sxs-lookup"><span data-stu-id="c540b-128">In the request body, supply a JSON representation for the [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) object.</span></span>

<span data-ttu-id="c540b-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md).</span><span class="sxs-lookup"><span data-stu-id="c540b-129">The following table shows the properties that are required when you create the [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md).</span></span>

|<span data-ttu-id="c540b-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c540b-130">Property</span></span>|<span data-ttu-id="c540b-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="c540b-131">Type</span></span>|<span data-ttu-id="c540b-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="c540b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c540b-133">id</span><span class="sxs-lookup"><span data-stu-id="c540b-133">id</span></span>|<span data-ttu-id="c540b-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c540b-134">String</span></span>|<span data-ttu-id="c540b-135">Identificador exclusivo para o objeto.</span><span class="sxs-lookup"><span data-stu-id="c540b-135">Unique identifier for the object.</span></span> <span data-ttu-id="c540b-136">Composto de accountId, deviceId, policyId e userId</span><span class="sxs-lookup"><span data-stu-id="c540b-136">Composed from accountId, deviceId, policyId and userId</span></span>|
|<span data-ttu-id="c540b-137">userId</span><span class="sxs-lookup"><span data-stu-id="c540b-137">userId</span></span>|<span data-ttu-id="c540b-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c540b-138">String</span></span>|<span data-ttu-id="c540b-139">Identificador exclusivo do usuário, deve ser um Guid</span><span class="sxs-lookup"><span data-stu-id="c540b-139">User unique identifier, must be Guid</span></span>|
|<span data-ttu-id="c540b-140">userName</span><span class="sxs-lookup"><span data-stu-id="c540b-140">userName</span></span>|<span data-ttu-id="c540b-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c540b-141">String</span></span>|<span data-ttu-id="c540b-142">Nome de usuário</span><span class="sxs-lookup"><span data-stu-id="c540b-142">User name</span></span>|
|<span data-ttu-id="c540b-143">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="c540b-143">managedDeviceId</span></span>|<span data-ttu-id="c540b-144">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c540b-144">String</span></span>|<span data-ttu-id="c540b-145">Identificador exclusivo do dispositivo gerenciado, deve ser um Guid</span><span class="sxs-lookup"><span data-stu-id="c540b-145">Managed device unique identifier, must be Guid</span></span>|
|<span data-ttu-id="c540b-146">deviceName</span><span class="sxs-lookup"><span data-stu-id="c540b-146">deviceName</span></span>|<span data-ttu-id="c540b-147">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c540b-147">String</span></span>|<span data-ttu-id="c540b-148">Nome do dispositivo</span><span class="sxs-lookup"><span data-stu-id="c540b-148">Device name</span></span>|
|<span data-ttu-id="c540b-149">deviceConfigurationId</span><span class="sxs-lookup"><span data-stu-id="c540b-149">deviceConfigurationId</span></span>|<span data-ttu-id="c540b-150">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c540b-150">String</span></span>|<span data-ttu-id="c540b-151">Identificador exclusivo do perfil do configuração de dispositivo, deve ser um Guid</span><span class="sxs-lookup"><span data-stu-id="c540b-151">Device configuration profile unique identifier, must be Guid</span></span>|
|<span data-ttu-id="c540b-152">deviceConfigurationName</span><span class="sxs-lookup"><span data-stu-id="c540b-152">deviceConfigurationName</span></span>|<span data-ttu-id="c540b-153">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c540b-153">String</span></span>|<span data-ttu-id="c540b-154">Nome do perfil de configuração de dispositivo</span><span class="sxs-lookup"><span data-stu-id="c540b-154">Device configuration profile name</span></span>|
|<span data-ttu-id="c540b-155">platformType</span><span class="sxs-lookup"><span data-stu-id="c540b-155">platformType</span></span>|[<span data-ttu-id="c540b-156">policyPlatformType</span><span class="sxs-lookup"><span data-stu-id="c540b-156">policyPlatformType</span></span>](../resources/intune-deviceconfig-policyplatformtype.md)|<span data-ttu-id="c540b-157">Tipo de plataforma.</span><span class="sxs-lookup"><span data-stu-id="c540b-157">Platform type.</span></span> <span data-ttu-id="c540b-158">Os valores possíveis são: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.</span><span class="sxs-lookup"><span data-stu-id="c540b-158">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.</span></span>|
|<span data-ttu-id="c540b-159">restrictedAppsState</span><span class="sxs-lookup"><span data-stu-id="c540b-159">restrictedAppsState</span></span>|[<span data-ttu-id="c540b-160">restrictedAppsState</span><span class="sxs-lookup"><span data-stu-id="c540b-160">restrictedAppsState</span></span>](../resources/intune-deviceconfig-restrictedappsstate.md)|<span data-ttu-id="c540b-161">Estado restrito de aplicativos.</span><span class="sxs-lookup"><span data-stu-id="c540b-161">Restricted apps state.</span></span> <span data-ttu-id="c540b-162">Os valores possíveis são: `prohibitedApps` e `notApprovedApps`.</span><span class="sxs-lookup"><span data-stu-id="c540b-162">Possible values are: `prohibitedApps`, `notApprovedApps`.</span></span>|
|<span data-ttu-id="c540b-163">restrictedApps</span><span class="sxs-lookup"><span data-stu-id="c540b-163">restrictedApps</span></span>|<span data-ttu-id="c540b-164">coleção [managedDeviceReportedApp](../resources/intune-deviceconfig-manageddevicereportedapp.md)</span><span class="sxs-lookup"><span data-stu-id="c540b-164">[managedDeviceReportedApp](../resources/intune-deviceconfig-manageddevicereportedapp.md) collection</span></span>|<span data-ttu-id="c540b-165">Lista de aplicativos restritos violadas</span><span class="sxs-lookup"><span data-stu-id="c540b-165">List of violated restricted apps</span></span>|



## <a name="response"></a><span data-ttu-id="c540b-166">Resposta</span><span class="sxs-lookup"><span data-stu-id="c540b-166">Response</span></span>
<span data-ttu-id="c540b-167">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto atualizado [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c540b-167">If successful, this method returns a `200 OK` response code and an updated [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c540b-168">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c540b-168">Example</span></span>
### <a name="request"></a><span data-ttu-id="c540b-169">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c540b-169">Request</span></span>
<span data-ttu-id="c540b-170">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c540b-170">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurationRestrictedAppsViolations/{restrictedAppsViolationId}
Content-type: application/json
Content-length: 502

{
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

### <a name="response"></a><span data-ttu-id="c540b-171">Resposta</span><span class="sxs-lookup"><span data-stu-id="c540b-171">Response</span></span>
<span data-ttu-id="c540b-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c540b-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





