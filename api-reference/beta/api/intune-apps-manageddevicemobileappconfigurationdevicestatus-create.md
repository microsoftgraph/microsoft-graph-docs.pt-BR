---
title: Criar managedDeviceMobileAppConfigurationDeviceStatus
description: Crie um novo objeto de managedDeviceMobileAppConfigurationDeviceStatus.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: ba758e1e7beb9d665c63da575a5011c41a0b95f1
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27887882"
---
# <a name="create-manageddevicemobileappconfigurationdevicestatus"></a><span data-ttu-id="4a96d-103">Criar managedDeviceMobileAppConfigurationDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="4a96d-103">Create managedDeviceMobileAppConfigurationDeviceStatus</span></span>

> <span data-ttu-id="4a96d-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="4a96d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4a96d-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="4a96d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4a96d-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="4a96d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4a96d-107">Crie um novo objeto de [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) .</span><span class="sxs-lookup"><span data-stu-id="4a96d-107">Create a new [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="4a96d-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="4a96d-108">Prerequisites</span></span>
<span data-ttu-id="4a96d-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4a96d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4a96d-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4a96d-111">Permission type</span></span>|<span data-ttu-id="4a96d-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="4a96d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4a96d-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4a96d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4a96d-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4a96d-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="4a96d-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4a96d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4a96d-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4a96d-116">Not supported.</span></span>|
|<span data-ttu-id="4a96d-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4a96d-117">Application</span></span>|<span data-ttu-id="4a96d-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4a96d-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4a96d-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4a96d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatuses
POST /deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/deviceStatuses
```

## <a name="request-headers"></a><span data-ttu-id="4a96d-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4a96d-120">Request headers</span></span>
|<span data-ttu-id="4a96d-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4a96d-121">Header</span></span>|<span data-ttu-id="4a96d-122">Valor</span><span class="sxs-lookup"><span data-stu-id="4a96d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4a96d-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="4a96d-123">Authorization</span></span>|<span data-ttu-id="4a96d-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4a96d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4a96d-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="4a96d-125">Accept</span></span>|<span data-ttu-id="4a96d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4a96d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4a96d-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4a96d-127">Request body</span></span>
<span data-ttu-id="4a96d-128">No corpo da solicitação, fornece uma representação JSON para o objeto managedDeviceMobileAppConfigurationDeviceStatus.</span><span class="sxs-lookup"><span data-stu-id="4a96d-128">In the request body, supply a JSON representation for the managedDeviceMobileAppConfigurationDeviceStatus object.</span></span>

<span data-ttu-id="4a96d-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o managedDeviceMobileAppConfigurationDeviceStatus.</span><span class="sxs-lookup"><span data-stu-id="4a96d-129">The following table shows the properties that are required when you create the managedDeviceMobileAppConfigurationDeviceStatus.</span></span>

|<span data-ttu-id="4a96d-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4a96d-130">Property</span></span>|<span data-ttu-id="4a96d-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="4a96d-131">Type</span></span>|<span data-ttu-id="4a96d-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="4a96d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4a96d-133">id</span><span class="sxs-lookup"><span data-stu-id="4a96d-133">id</span></span>|<span data-ttu-id="4a96d-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4a96d-134">String</span></span>|<span data-ttu-id="4a96d-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="4a96d-135">Key of the entity.</span></span>|
|<span data-ttu-id="4a96d-136">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="4a96d-136">deviceDisplayName</span></span>|<span data-ttu-id="4a96d-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4a96d-137">String</span></span>|<span data-ttu-id="4a96d-138">Nome do dispositivo de DevicePolicyStatus.</span><span class="sxs-lookup"><span data-stu-id="4a96d-138">Device name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="4a96d-139">userName</span><span class="sxs-lookup"><span data-stu-id="4a96d-139">userName</span></span>|<span data-ttu-id="4a96d-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4a96d-140">String</span></span>|<span data-ttu-id="4a96d-141">O nome de usuário que está sendo relatado</span><span class="sxs-lookup"><span data-stu-id="4a96d-141">The User Name that is being reported</span></span>|
|<span data-ttu-id="4a96d-142">deviceModel</span><span class="sxs-lookup"><span data-stu-id="4a96d-142">deviceModel</span></span>|<span data-ttu-id="4a96d-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4a96d-143">String</span></span>|<span data-ttu-id="4a96d-144">O modelo do dispositivo que está sendo relatado</span><span class="sxs-lookup"><span data-stu-id="4a96d-144">The device model that is being reported</span></span>|
|<span data-ttu-id="4a96d-145">platform</span><span class="sxs-lookup"><span data-stu-id="4a96d-145">platform</span></span>|<span data-ttu-id="4a96d-146">Int32</span><span class="sxs-lookup"><span data-stu-id="4a96d-146">Int32</span></span>|<span data-ttu-id="4a96d-147">Plataforma do dispositivo que está sendo relatado</span><span class="sxs-lookup"><span data-stu-id="4a96d-147">Platform of the device that is being reported</span></span>|
|<span data-ttu-id="4a96d-148">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="4a96d-148">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="4a96d-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4a96d-149">DateTimeOffset</span></span>|<span data-ttu-id="4a96d-150">DateTime em que o período de cortesia de conformidade do dispositivo termina</span><span class="sxs-lookup"><span data-stu-id="4a96d-150">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="4a96d-151">status</span><span class="sxs-lookup"><span data-stu-id="4a96d-151">status</span></span>|[<span data-ttu-id="4a96d-152">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="4a96d-152">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="4a96d-153">Status de conformidade do relatório de políticas.</span><span class="sxs-lookup"><span data-stu-id="4a96d-153">Compliance status of the policy report.</span></span> <span data-ttu-id="4a96d-154">Os valores possíveis são: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="4a96d-154">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="4a96d-155">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="4a96d-155">lastReportedDateTime</span></span>|<span data-ttu-id="4a96d-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4a96d-156">DateTimeOffset</span></span>|<span data-ttu-id="4a96d-157">Data e hora da última modificação do relatório de políticas.</span><span class="sxs-lookup"><span data-stu-id="4a96d-157">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="4a96d-158">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="4a96d-158">userPrincipalName</span></span>|<span data-ttu-id="4a96d-159">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4a96d-159">String</span></span>|<span data-ttu-id="4a96d-160">UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="4a96d-160">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="4a96d-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="4a96d-161">Response</span></span>
<span data-ttu-id="4a96d-162">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4a96d-162">If successful, this method returns a `201 Created` response code and a [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4a96d-163">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4a96d-163">Example</span></span>
### <a name="request"></a><span data-ttu-id="4a96d-164">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4a96d-164">Request</span></span>
<span data-ttu-id="4a96d-165">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4a96d-165">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatuses
Content-type: application/json
Content-length: 463

{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationDeviceStatus",
  "deviceDisplayName": "Device Display Name value",
  "userName": "User Name value",
  "deviceModel": "Device Model value",
  "platform": 8,
  "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00",
  "status": "notApplicable",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "userPrincipalName": "User Principal Name value"
}
```

### <a name="response"></a><span data-ttu-id="4a96d-166">Resposta</span><span class="sxs-lookup"><span data-stu-id="4a96d-166">Response</span></span>
<span data-ttu-id="4a96d-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4a96d-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 512

{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationDeviceStatus",
  "id": "477d3651-3651-477d-5136-7d4751367d47",
  "deviceDisplayName": "Device Display Name value",
  "userName": "User Name value",
  "deviceModel": "Device Model value",
  "platform": 8,
  "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00",
  "status": "notApplicable",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "userPrincipalName": "User Principal Name value"
}
```





