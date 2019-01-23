---
title: Atualizar restrictedAppsViolation
description: Atualize as propriedades de um objeto restrictedAppsViolation.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 01509691e65410776ba57269c8a7cb9e804ee661
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29403851"
---
# <a name="update-restrictedappsviolation"></a><span data-ttu-id="5942e-103">Atualizar restrictedAppsViolation</span><span class="sxs-lookup"><span data-stu-id="5942e-103">Update restrictedAppsViolation</span></span>

> <span data-ttu-id="5942e-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="5942e-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="5942e-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="5942e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5942e-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="5942e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5942e-107">Atualize as propriedades de um objeto [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) .</span><span class="sxs-lookup"><span data-stu-id="5942e-107">Update the properties of a [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5942e-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="5942e-108">Prerequisites</span></span>
<span data-ttu-id="5942e-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="5942e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="5942e-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5942e-111">Permission type</span></span>|<span data-ttu-id="5942e-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="5942e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5942e-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5942e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5942e-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5942e-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="5942e-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5942e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5942e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5942e-116">Not supported.</span></span>|
|<span data-ttu-id="5942e-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5942e-117">Application</span></span>|<span data-ttu-id="5942e-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5942e-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5942e-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5942e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurationRestrictedAppsViolations/{restrictedAppsViolationId}
```

## <a name="request-headers"></a><span data-ttu-id="5942e-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5942e-120">Request headers</span></span>
|<span data-ttu-id="5942e-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5942e-121">Header</span></span>|<span data-ttu-id="5942e-122">Valor</span><span class="sxs-lookup"><span data-stu-id="5942e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5942e-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="5942e-123">Authorization</span></span>|<span data-ttu-id="5942e-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5942e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5942e-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="5942e-125">Accept</span></span>|<span data-ttu-id="5942e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5942e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5942e-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5942e-127">Request body</span></span>
<span data-ttu-id="5942e-128">No corpo da solicitação, fornece uma representação JSON para o objeto [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) .</span><span class="sxs-lookup"><span data-stu-id="5942e-128">In the request body, supply a JSON representation for the [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) object.</span></span>

<span data-ttu-id="5942e-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md).</span><span class="sxs-lookup"><span data-stu-id="5942e-129">The following table shows the properties that are required when you create the [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md).</span></span>

|<span data-ttu-id="5942e-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5942e-130">Property</span></span>|<span data-ttu-id="5942e-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="5942e-131">Type</span></span>|<span data-ttu-id="5942e-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="5942e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5942e-133">id</span><span class="sxs-lookup"><span data-stu-id="5942e-133">id</span></span>|<span data-ttu-id="5942e-134">String</span><span class="sxs-lookup"><span data-stu-id="5942e-134">String</span></span>|<span data-ttu-id="5942e-135">Identificador exclusivo para o objeto.</span><span class="sxs-lookup"><span data-stu-id="5942e-135">Unique identifier for the object.</span></span> <span data-ttu-id="5942e-136">Composto de accountId, deviceId, policyId e userId</span><span class="sxs-lookup"><span data-stu-id="5942e-136">Composed from accountId, deviceId, policyId and userId</span></span>|
|<span data-ttu-id="5942e-137">userId</span><span class="sxs-lookup"><span data-stu-id="5942e-137">userId</span></span>|<span data-ttu-id="5942e-138">String</span><span class="sxs-lookup"><span data-stu-id="5942e-138">String</span></span>|<span data-ttu-id="5942e-139">Identificador exclusivo do usuário, deve ser um Guid</span><span class="sxs-lookup"><span data-stu-id="5942e-139">User unique identifier, must be Guid</span></span>|
|<span data-ttu-id="5942e-140">userName</span><span class="sxs-lookup"><span data-stu-id="5942e-140">userName</span></span>|<span data-ttu-id="5942e-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5942e-141">String</span></span>|<span data-ttu-id="5942e-142">Nome de usuário</span><span class="sxs-lookup"><span data-stu-id="5942e-142">User name</span></span>|
|<span data-ttu-id="5942e-143">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="5942e-143">managedDeviceId</span></span>|<span data-ttu-id="5942e-144">String</span><span class="sxs-lookup"><span data-stu-id="5942e-144">String</span></span>|<span data-ttu-id="5942e-145">Identificador exclusivo do dispositivo gerenciado, deve ser um Guid</span><span class="sxs-lookup"><span data-stu-id="5942e-145">Managed device unique identifier, must be Guid</span></span>|
|<span data-ttu-id="5942e-146">deviceName</span><span class="sxs-lookup"><span data-stu-id="5942e-146">deviceName</span></span>|<span data-ttu-id="5942e-147">String</span><span class="sxs-lookup"><span data-stu-id="5942e-147">String</span></span>|<span data-ttu-id="5942e-148">Nome do dispositivo</span><span class="sxs-lookup"><span data-stu-id="5942e-148">Device name</span></span>|
|<span data-ttu-id="5942e-149">deviceConfigurationId</span><span class="sxs-lookup"><span data-stu-id="5942e-149">deviceConfigurationId</span></span>|<span data-ttu-id="5942e-150">String</span><span class="sxs-lookup"><span data-stu-id="5942e-150">String</span></span>|<span data-ttu-id="5942e-151">Identificador exclusivo do perfil do configuração de dispositivo, deve ser um Guid</span><span class="sxs-lookup"><span data-stu-id="5942e-151">Device configuration profile unique identifier, must be Guid</span></span>|
|<span data-ttu-id="5942e-152">deviceConfigurationName</span><span class="sxs-lookup"><span data-stu-id="5942e-152">deviceConfigurationName</span></span>|<span data-ttu-id="5942e-153">String</span><span class="sxs-lookup"><span data-stu-id="5942e-153">String</span></span>|<span data-ttu-id="5942e-154">Nome do perfil de configuração de dispositivo</span><span class="sxs-lookup"><span data-stu-id="5942e-154">Device configuration profile name</span></span>|
|<span data-ttu-id="5942e-155">platformType</span><span class="sxs-lookup"><span data-stu-id="5942e-155">platformType</span></span>|[<span data-ttu-id="5942e-156">policyPlatformType</span><span class="sxs-lookup"><span data-stu-id="5942e-156">policyPlatformType</span></span>](../resources/intune-deviceconfig-policyplatformtype.md)|<span data-ttu-id="5942e-157">Tipo de plataforma.</span><span class="sxs-lookup"><span data-stu-id="5942e-157">Platform type.</span></span> <span data-ttu-id="5942e-158">Os valores possíveis são: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.</span><span class="sxs-lookup"><span data-stu-id="5942e-158">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.</span></span>|
|<span data-ttu-id="5942e-159">restrictedAppsState</span><span class="sxs-lookup"><span data-stu-id="5942e-159">restrictedAppsState</span></span>|[<span data-ttu-id="5942e-160">restrictedAppsState</span><span class="sxs-lookup"><span data-stu-id="5942e-160">restrictedAppsState</span></span>](../resources/intune-deviceconfig-restrictedappsstate.md)|<span data-ttu-id="5942e-161">Estado restrito de aplicativos.</span><span class="sxs-lookup"><span data-stu-id="5942e-161">Restricted apps state.</span></span> <span data-ttu-id="5942e-162">Os valores possíveis são: `prohibitedApps` e `notApprovedApps`.</span><span class="sxs-lookup"><span data-stu-id="5942e-162">Possible values are: `prohibitedApps`, `notApprovedApps`.</span></span>|
|<span data-ttu-id="5942e-163">restrictedApps</span><span class="sxs-lookup"><span data-stu-id="5942e-163">restrictedApps</span></span>|<span data-ttu-id="5942e-164">coleção [managedDeviceReportedApp](../resources/intune-deviceconfig-manageddevicereportedapp.md)</span><span class="sxs-lookup"><span data-stu-id="5942e-164">[managedDeviceReportedApp](../resources/intune-deviceconfig-manageddevicereportedapp.md) collection</span></span>|<span data-ttu-id="5942e-165">Lista de aplicativos restritos violadas</span><span class="sxs-lookup"><span data-stu-id="5942e-165">List of violated restricted apps</span></span>|



## <a name="response"></a><span data-ttu-id="5942e-166">Resposta</span><span class="sxs-lookup"><span data-stu-id="5942e-166">Response</span></span>
<span data-ttu-id="5942e-167">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto atualizado [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5942e-167">If successful, this method returns a `200 OK` response code and an updated [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5942e-168">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5942e-168">Example</span></span>

### <a name="request"></a><span data-ttu-id="5942e-169">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5942e-169">Request</span></span>
<span data-ttu-id="5942e-170">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5942e-170">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="5942e-171">Resposta</span><span class="sxs-lookup"><span data-stu-id="5942e-171">Response</span></span>
<span data-ttu-id="5942e-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5942e-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




