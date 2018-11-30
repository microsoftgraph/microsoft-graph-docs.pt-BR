---
title: Criar iosUpdateDeviceStatus
description: Criar um novo objeto iosUpdateDeviceStatus.
ms.openlocfilehash: 205bc02b37f3ba846e2fc7df0685d50fbd9e5279
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27038019"
---
# <a name="create-iosupdatedevicestatus"></a><span data-ttu-id="2233c-103">Criar iosUpdateDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="2233c-103">Create iosUpdateDeviceStatus</span></span>

> <span data-ttu-id="2233c-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="2233c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2233c-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="2233c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2233c-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="2233c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2233c-107">Criar um novo objeto [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="2233c-107">Create a new [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="2233c-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="2233c-108">Prerequisites</span></span>
<span data-ttu-id="2233c-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2233c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2233c-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2233c-111">Permission type</span></span>|<span data-ttu-id="2233c-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="2233c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2233c-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2233c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2233c-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2233c-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="2233c-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2233c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2233c-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2233c-116">Not supported.</span></span>|
|<span data-ttu-id="2233c-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2233c-117">Application</span></span>|<span data-ttu-id="2233c-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2233c-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2233c-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2233c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/iosUpdateStatuses
```

## <a name="request-headers"></a><span data-ttu-id="2233c-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2233c-120">Request headers</span></span>
|<span data-ttu-id="2233c-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2233c-121">Header</span></span>|<span data-ttu-id="2233c-122">Valor</span><span class="sxs-lookup"><span data-stu-id="2233c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2233c-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="2233c-123">Authorization</span></span>|<span data-ttu-id="2233c-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2233c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2233c-125">Accept</span><span class="sxs-lookup"><span data-stu-id="2233c-125">Accept</span></span>|<span data-ttu-id="2233c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2233c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2233c-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2233c-127">Request body</span></span>
<span data-ttu-id="2233c-128">No corpo da solicitação, forneça uma representação JSON do objeto iosUpdateDeviceStatus.</span><span class="sxs-lookup"><span data-stu-id="2233c-128">In the request body, supply a JSON representation for the iosUpdateDeviceStatus object.</span></span>

<span data-ttu-id="2233c-129">A tabela a seguir mostra as propriedades que são necessárias ao criar iosUpdateDeviceStatus.</span><span class="sxs-lookup"><span data-stu-id="2233c-129">The following table shows the properties that are required when you create the iosUpdateDeviceStatus.</span></span>

|<span data-ttu-id="2233c-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2233c-130">Property</span></span>|<span data-ttu-id="2233c-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="2233c-131">Type</span></span>|<span data-ttu-id="2233c-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="2233c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2233c-133">id</span><span class="sxs-lookup"><span data-stu-id="2233c-133">id</span></span>|<span data-ttu-id="2233c-134">String</span><span class="sxs-lookup"><span data-stu-id="2233c-134">String</span></span>|<span data-ttu-id="2233c-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="2233c-135">Key of the entity.</span></span>|
|<span data-ttu-id="2233c-136">installStatus</span><span class="sxs-lookup"><span data-stu-id="2233c-136">installStatus</span></span>|[<span data-ttu-id="2233c-137">iosUpdatesInstallStatus</span><span class="sxs-lookup"><span data-stu-id="2233c-137">iosUpdatesInstallStatus</span></span>](../resources/intune-deviceconfig-iosupdatesinstallstatus.md)|<span data-ttu-id="2233c-138">O status de instalação do relatório de políticas.</span><span class="sxs-lookup"><span data-stu-id="2233c-138">The installation status of the policy report.</span></span> <span data-ttu-id="2233c-139">Os valores possíveis são: `success`, `available`, `idle`, `unknown`, `downloading`, `downloadFailed`, `downloadRequiresComputer`, `downloadInsufficientSpace`, `downloadInsufficientPower`, `downloadInsufficientNetwork`, `installing`, `installInsufficientSpace`, `installInsufficientPower`, `installPhoneCallInProgress`, `installFailed`, `notSupportedOperation`, `sharedDeviceUserLoggedInError`.</span><span class="sxs-lookup"><span data-stu-id="2233c-139">Possible values are: `success`, `available`, `idle`, `unknown`, `downloading`, `downloadFailed`, `downloadRequiresComputer`, `downloadInsufficientSpace`, `downloadInsufficientPower`, `downloadInsufficientNetwork`, `installing`, `installInsufficientSpace`, `installInsufficientPower`, `installPhoneCallInProgress`, `installFailed`, `notSupportedOperation`, `sharedDeviceUserLoggedInError`.</span></span>|
|<span data-ttu-id="2233c-140">osVersion</span><span class="sxs-lookup"><span data-stu-id="2233c-140">osVersion</span></span>|<span data-ttu-id="2233c-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2233c-141">String</span></span>|<span data-ttu-id="2233c-142">A versão do dispositivo que está sendo relatado.</span><span class="sxs-lookup"><span data-stu-id="2233c-142">The device version that is being reported.</span></span>|
|<span data-ttu-id="2233c-143">deviceId</span><span class="sxs-lookup"><span data-stu-id="2233c-143">deviceId</span></span>|<span data-ttu-id="2233c-144">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2233c-144">String</span></span>|<span data-ttu-id="2233c-145">A ID do dispositivo que está sendo relatado.</span><span class="sxs-lookup"><span data-stu-id="2233c-145">The device id that is being reported.</span></span>|
|<span data-ttu-id="2233c-146">userId</span><span class="sxs-lookup"><span data-stu-id="2233c-146">userId</span></span>|<span data-ttu-id="2233c-147">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2233c-147">String</span></span>|<span data-ttu-id="2233c-148">A ID do usuário que está sendo relatado.</span><span class="sxs-lookup"><span data-stu-id="2233c-148">The User id that is being reported.</span></span>|
|<span data-ttu-id="2233c-149">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="2233c-149">deviceDisplayName</span></span>|<span data-ttu-id="2233c-150">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2233c-150">String</span></span>|<span data-ttu-id="2233c-151">Nome do dispositivo de DevicePolicyStatus.</span><span class="sxs-lookup"><span data-stu-id="2233c-151">Device name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="2233c-152">userName</span><span class="sxs-lookup"><span data-stu-id="2233c-152">userName</span></span>|<span data-ttu-id="2233c-153">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2233c-153">String</span></span>|<span data-ttu-id="2233c-154">O nome de usuário que está sendo relatado</span><span class="sxs-lookup"><span data-stu-id="2233c-154">The User Name that is being reported</span></span>|
|<span data-ttu-id="2233c-155">deviceModel</span><span class="sxs-lookup"><span data-stu-id="2233c-155">deviceModel</span></span>|<span data-ttu-id="2233c-156">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2233c-156">String</span></span>|<span data-ttu-id="2233c-157">O modelo do dispositivo que está sendo relatado</span><span class="sxs-lookup"><span data-stu-id="2233c-157">The device model that is being reported</span></span>|
|<span data-ttu-id="2233c-158">platform</span><span class="sxs-lookup"><span data-stu-id="2233c-158">platform</span></span>|<span data-ttu-id="2233c-159">Int32</span><span class="sxs-lookup"><span data-stu-id="2233c-159">Int32</span></span>|<span data-ttu-id="2233c-160">Plataforma do dispositivo que está sendo relatado</span><span class="sxs-lookup"><span data-stu-id="2233c-160">Platform of the device that is being reported</span></span>|
|<span data-ttu-id="2233c-161">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="2233c-161">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="2233c-162">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2233c-162">DateTimeOffset</span></span>|<span data-ttu-id="2233c-163">DateTime em que o período de cortesia de conformidade do dispositivo termina</span><span class="sxs-lookup"><span data-stu-id="2233c-163">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="2233c-164">status</span><span class="sxs-lookup"><span data-stu-id="2233c-164">status</span></span>|[<span data-ttu-id="2233c-165">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="2233c-165">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="2233c-166">Status de conformidade do relatório de políticas.</span><span class="sxs-lookup"><span data-stu-id="2233c-166">Compliance status of the policy report.</span></span> <span data-ttu-id="2233c-167">Os valores possíveis são: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="2233c-167">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="2233c-168">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="2233c-168">lastReportedDateTime</span></span>|<span data-ttu-id="2233c-169">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2233c-169">DateTimeOffset</span></span>|<span data-ttu-id="2233c-170">Data e hora da última modificação do relatório de políticas.</span><span class="sxs-lookup"><span data-stu-id="2233c-170">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="2233c-171">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="2233c-171">userPrincipalName</span></span>|<span data-ttu-id="2233c-172">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2233c-172">String</span></span>|<span data-ttu-id="2233c-173">UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="2233c-173">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="2233c-174">Resposta</span><span class="sxs-lookup"><span data-stu-id="2233c-174">Response</span></span>
<span data-ttu-id="2233c-175">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2233c-175">If successful, this method returns a `201 Created` response code and a [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2233c-176">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2233c-176">Example</span></span>
### <a name="request"></a><span data-ttu-id="2233c-177">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2233c-177">Request</span></span>
<span data-ttu-id="2233c-178">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2233c-178">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/iosUpdateStatuses
Content-type: application/json
Content-length: 570

{
  "@odata.type": "#microsoft.graph.iosUpdateDeviceStatus",
  "installStatus": "available",
  "osVersion": "Os Version value",
  "deviceId": "Device Id value",
  "userId": "User Id value",
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

### <a name="response"></a><span data-ttu-id="2233c-179">Resposta</span><span class="sxs-lookup"><span data-stu-id="2233c-179">Response</span></span>
<span data-ttu-id="2233c-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2233c-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 619

{
  "@odata.type": "#microsoft.graph.iosUpdateDeviceStatus",
  "id": "63a79499-9499-63a7-9994-a7639994a763",
  "installStatus": "available",
  "osVersion": "Os Version value",
  "deviceId": "Device Id value",
  "userId": "User Id value",
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





