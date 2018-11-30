---
title: Criar deviceConfigurationDeviceStatus
description: Criar um novo objeto deviceConfigurationDeviceStatus.
ms.openlocfilehash: b79a58ef701d22b35b1c2c19a0c166db02cada11
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27003817"
---
# <a name="create-deviceconfigurationdevicestatus"></a><span data-ttu-id="8aa49-103">Criar deviceConfigurationDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="8aa49-103">Create deviceConfigurationDeviceStatus</span></span>

> <span data-ttu-id="8aa49-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="8aa49-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8aa49-105">Criar um novo objeto [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="8aa49-105">Create a new [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8aa49-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="8aa49-106">Prerequisites</span></span>
<span data-ttu-id="8aa49-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8aa49-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8aa49-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8aa49-109">Permission type</span></span>|<span data-ttu-id="8aa49-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="8aa49-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8aa49-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8aa49-111">Delegated (work or school account)</span></span>|<span data-ttu-id="8aa49-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8aa49-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8aa49-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8aa49-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8aa49-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8aa49-114">Not supported.</span></span>|
|<span data-ttu-id="8aa49-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8aa49-115">Application</span></span>|<span data-ttu-id="8aa49-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8aa49-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8aa49-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8aa49-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceStatuses
```

## <a name="request-headers"></a><span data-ttu-id="8aa49-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8aa49-118">Request headers</span></span>
|<span data-ttu-id="8aa49-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8aa49-119">Header</span></span>|<span data-ttu-id="8aa49-120">Valor</span><span class="sxs-lookup"><span data-stu-id="8aa49-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8aa49-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="8aa49-121">Authorization</span></span>|<span data-ttu-id="8aa49-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8aa49-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8aa49-123">Accept</span><span class="sxs-lookup"><span data-stu-id="8aa49-123">Accept</span></span>|<span data-ttu-id="8aa49-124">application/json</span><span class="sxs-lookup"><span data-stu-id="8aa49-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8aa49-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8aa49-125">Request body</span></span>
<span data-ttu-id="8aa49-126">No corpo da solicitação, forneça uma representação JSON do objeto deviceConfigurationDeviceStatus.</span><span class="sxs-lookup"><span data-stu-id="8aa49-126">In the request body, supply a JSON representation for the deviceConfigurationDeviceStatus object.</span></span>

<span data-ttu-id="8aa49-127">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceConfigurationDeviceStatus.</span><span class="sxs-lookup"><span data-stu-id="8aa49-127">The following table shows the properties that are required when you create the deviceConfigurationDeviceStatus.</span></span>

|<span data-ttu-id="8aa49-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8aa49-128">Property</span></span>|<span data-ttu-id="8aa49-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="8aa49-129">Type</span></span>|<span data-ttu-id="8aa49-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="8aa49-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8aa49-131">id</span><span class="sxs-lookup"><span data-stu-id="8aa49-131">id</span></span>|<span data-ttu-id="8aa49-132">String</span><span class="sxs-lookup"><span data-stu-id="8aa49-132">String</span></span>|<span data-ttu-id="8aa49-133">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="8aa49-133">Key of the entity.</span></span>|
|<span data-ttu-id="8aa49-134">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="8aa49-134">deviceDisplayName</span></span>|<span data-ttu-id="8aa49-135">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8aa49-135">String</span></span>|<span data-ttu-id="8aa49-136">Nome do dispositivo de DevicePolicyStatus.</span><span class="sxs-lookup"><span data-stu-id="8aa49-136">Device name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="8aa49-137">userName</span><span class="sxs-lookup"><span data-stu-id="8aa49-137">userName</span></span>|<span data-ttu-id="8aa49-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8aa49-138">String</span></span>|<span data-ttu-id="8aa49-139">O nome de usuário que está sendo relatado</span><span class="sxs-lookup"><span data-stu-id="8aa49-139">The User Name that is being reported</span></span>|
|<span data-ttu-id="8aa49-140">deviceModel</span><span class="sxs-lookup"><span data-stu-id="8aa49-140">deviceModel</span></span>|<span data-ttu-id="8aa49-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8aa49-141">String</span></span>|<span data-ttu-id="8aa49-142">O modelo do dispositivo que está sendo relatado</span><span class="sxs-lookup"><span data-stu-id="8aa49-142">The device model that is being reported</span></span>|
|<span data-ttu-id="8aa49-143">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="8aa49-143">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="8aa49-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8aa49-144">DateTimeOffset</span></span>|<span data-ttu-id="8aa49-145">DateTime em que o período de cortesia de conformidade do dispositivo termina</span><span class="sxs-lookup"><span data-stu-id="8aa49-145">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="8aa49-146">status</span><span class="sxs-lookup"><span data-stu-id="8aa49-146">status</span></span>|[<span data-ttu-id="8aa49-147">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="8aa49-147">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="8aa49-148">Status de conformidade do relatório de políticas.</span><span class="sxs-lookup"><span data-stu-id="8aa49-148">Compliance status of the policy report.</span></span> <span data-ttu-id="8aa49-149">Os valores possíveis são: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="8aa49-149">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="8aa49-150">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="8aa49-150">lastReportedDateTime</span></span>|<span data-ttu-id="8aa49-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8aa49-151">DateTimeOffset</span></span>|<span data-ttu-id="8aa49-152">Data e hora da última modificação do relatório de políticas.</span><span class="sxs-lookup"><span data-stu-id="8aa49-152">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="8aa49-153">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="8aa49-153">userPrincipalName</span></span>|<span data-ttu-id="8aa49-154">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8aa49-154">String</span></span>|<span data-ttu-id="8aa49-155">UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="8aa49-155">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="8aa49-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="8aa49-156">Response</span></span>
<span data-ttu-id="8aa49-157">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8aa49-157">If successful, this method returns a `201 Created` response code and a [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8aa49-158">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8aa49-158">Example</span></span>
### <a name="request"></a><span data-ttu-id="8aa49-159">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8aa49-159">Request</span></span>
<span data-ttu-id="8aa49-160">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8aa49-160">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceStatuses
Content-type: application/json
Content-length: 429

{
  "@odata.type": "#microsoft.graph.deviceConfigurationDeviceStatus",
  "deviceDisplayName": "Device Display Name value",
  "userName": "User Name value",
  "deviceModel": "Device Model value",
  "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00",
  "status": "notApplicable",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "userPrincipalName": "User Principal Name value"
}
```

### <a name="response"></a><span data-ttu-id="8aa49-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="8aa49-161">Response</span></span>
<span data-ttu-id="8aa49-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8aa49-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 478

{
  "@odata.type": "#microsoft.graph.deviceConfigurationDeviceStatus",
  "id": "674e98e5-98e5-674e-e598-4e67e5984e67",
  "deviceDisplayName": "Device Display Name value",
  "userName": "User Name value",
  "deviceModel": "Device Model value",
  "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00",
  "status": "notApplicable",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "userPrincipalName": "User Principal Name value"
}
```



