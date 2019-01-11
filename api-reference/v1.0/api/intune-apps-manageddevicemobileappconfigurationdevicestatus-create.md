---
title: Criar managedDeviceMobileAppConfigurationDeviceStatus
description: Crie um novo objeto de managedDeviceMobileAppConfigurationDeviceStatus.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 2871583d7fb68ec0004b2a97390b085416ed4495
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27828865"
---
# <a name="create-manageddevicemobileappconfigurationdevicestatus"></a><span data-ttu-id="edfa8-103">Criar managedDeviceMobileAppConfigurationDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="edfa8-103">Create managedDeviceMobileAppConfigurationDeviceStatus</span></span>

> <span data-ttu-id="edfa8-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="edfa8-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="edfa8-105">Crie um novo objeto de [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) .</span><span class="sxs-lookup"><span data-stu-id="edfa8-105">Create a new [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="edfa8-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="edfa8-106">Prerequisites</span></span>
<span data-ttu-id="edfa8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="edfa8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="edfa8-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="edfa8-109">Permission type</span></span>|<span data-ttu-id="edfa8-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="edfa8-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="edfa8-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="edfa8-111">Delegated (work or school account)</span></span>|<span data-ttu-id="edfa8-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="edfa8-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="edfa8-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="edfa8-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="edfa8-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="edfa8-114">Not supported.</span></span>|
|<span data-ttu-id="edfa8-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="edfa8-115">Application</span></span>|<span data-ttu-id="edfa8-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="edfa8-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="edfa8-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="edfa8-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatuses
```

## <a name="request-headers"></a><span data-ttu-id="edfa8-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="edfa8-118">Request headers</span></span>
|<span data-ttu-id="edfa8-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="edfa8-119">Header</span></span>|<span data-ttu-id="edfa8-120">Valor</span><span class="sxs-lookup"><span data-stu-id="edfa8-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="edfa8-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="edfa8-121">Authorization</span></span>|<span data-ttu-id="edfa8-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="edfa8-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="edfa8-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="edfa8-123">Accept</span></span>|<span data-ttu-id="edfa8-124">application/json</span><span class="sxs-lookup"><span data-stu-id="edfa8-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="edfa8-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="edfa8-125">Request body</span></span>
<span data-ttu-id="edfa8-126">No corpo da solicitação, fornece uma representação JSON para o objeto managedDeviceMobileAppConfigurationDeviceStatus.</span><span class="sxs-lookup"><span data-stu-id="edfa8-126">In the request body, supply a JSON representation for the managedDeviceMobileAppConfigurationDeviceStatus object.</span></span>

<span data-ttu-id="edfa8-127">A tabela a seguir mostra as propriedades que são necessárias quando você cria o managedDeviceMobileAppConfigurationDeviceStatus.</span><span class="sxs-lookup"><span data-stu-id="edfa8-127">The following table shows the properties that are required when you create the managedDeviceMobileAppConfigurationDeviceStatus.</span></span>

|<span data-ttu-id="edfa8-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="edfa8-128">Property</span></span>|<span data-ttu-id="edfa8-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="edfa8-129">Type</span></span>|<span data-ttu-id="edfa8-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="edfa8-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="edfa8-131">id</span><span class="sxs-lookup"><span data-stu-id="edfa8-131">id</span></span>|<span data-ttu-id="edfa8-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="edfa8-132">String</span></span>|<span data-ttu-id="edfa8-133">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="edfa8-133">Key of the entity.</span></span>|
|<span data-ttu-id="edfa8-134">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="edfa8-134">deviceDisplayName</span></span>|<span data-ttu-id="edfa8-135">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="edfa8-135">String</span></span>|<span data-ttu-id="edfa8-136">Nome do dispositivo de DevicePolicyStatus.</span><span class="sxs-lookup"><span data-stu-id="edfa8-136">Device name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="edfa8-137">userName</span><span class="sxs-lookup"><span data-stu-id="edfa8-137">userName</span></span>|<span data-ttu-id="edfa8-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="edfa8-138">String</span></span>|<span data-ttu-id="edfa8-139">O nome de usuário que está sendo relatado</span><span class="sxs-lookup"><span data-stu-id="edfa8-139">The User Name that is being reported</span></span>|
|<span data-ttu-id="edfa8-140">deviceModel</span><span class="sxs-lookup"><span data-stu-id="edfa8-140">deviceModel</span></span>|<span data-ttu-id="edfa8-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="edfa8-141">String</span></span>|<span data-ttu-id="edfa8-142">O modelo do dispositivo que está sendo relatado</span><span class="sxs-lookup"><span data-stu-id="edfa8-142">The device model that is being reported</span></span>|
|<span data-ttu-id="edfa8-143">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="edfa8-143">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="edfa8-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="edfa8-144">DateTimeOffset</span></span>|<span data-ttu-id="edfa8-145">DateTime em que o período de cortesia de conformidade do dispositivo termina</span><span class="sxs-lookup"><span data-stu-id="edfa8-145">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="edfa8-146">status</span><span class="sxs-lookup"><span data-stu-id="edfa8-146">status</span></span>|[<span data-ttu-id="edfa8-147">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="edfa8-147">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="edfa8-148">Status de conformidade do relatório de políticas.</span><span class="sxs-lookup"><span data-stu-id="edfa8-148">Compliance status of the policy report.</span></span> <span data-ttu-id="edfa8-149">Os valores possíveis são: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="edfa8-149">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="edfa8-150">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="edfa8-150">lastReportedDateTime</span></span>|<span data-ttu-id="edfa8-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="edfa8-151">DateTimeOffset</span></span>|<span data-ttu-id="edfa8-152">Data e hora da última modificação do relatório de políticas.</span><span class="sxs-lookup"><span data-stu-id="edfa8-152">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="edfa8-153">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="edfa8-153">userPrincipalName</span></span>|<span data-ttu-id="edfa8-154">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="edfa8-154">String</span></span>|<span data-ttu-id="edfa8-155">UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="edfa8-155">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="edfa8-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="edfa8-156">Response</span></span>
<span data-ttu-id="edfa8-157">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="edfa8-157">If successful, this method returns a `201 Created` response code and a [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="edfa8-158">Exemplo</span><span class="sxs-lookup"><span data-stu-id="edfa8-158">Example</span></span>
### <a name="request"></a><span data-ttu-id="edfa8-159">Solicitação</span><span class="sxs-lookup"><span data-stu-id="edfa8-159">Request</span></span>
<span data-ttu-id="edfa8-160">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="edfa8-160">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatuses
Content-type: application/json
Content-length: 445

{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationDeviceStatus",
  "deviceDisplayName": "Device Display Name value",
  "userName": "User Name value",
  "deviceModel": "Device Model value",
  "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00",
  "status": "notApplicable",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "userPrincipalName": "User Principal Name value"
}
```

### <a name="response"></a><span data-ttu-id="edfa8-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="edfa8-161">Response</span></span>
<span data-ttu-id="edfa8-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="edfa8-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 494

{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationDeviceStatus",
  "id": "477d3651-3651-477d-5136-7d4751367d47",
  "deviceDisplayName": "Device Display Name value",
  "userName": "User Name value",
  "deviceModel": "Device Model value",
  "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00",
  "status": "notApplicable",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "userPrincipalName": "User Principal Name value"
}
```



