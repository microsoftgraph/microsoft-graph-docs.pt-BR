---
title: Atualizar iosUpdateDeviceStatus
description: Atualizar as propriedades de um objeto iosUpdateDeviceStatus.
ms.openlocfilehash: 2b652dd6208dee20f164d57c92a8f0d322a58d8d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27038117"
---
# <a name="update-iosupdatedevicestatus"></a><span data-ttu-id="63289-103">Atualizar iosUpdateDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="63289-103">Update iosUpdateDeviceStatus</span></span>

> <span data-ttu-id="63289-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="63289-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="63289-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="63289-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="63289-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="63289-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="63289-107">Atualizar as propriedades de um objeto [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="63289-107">Update the properties of a [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="63289-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="63289-108">Prerequisites</span></span>
<span data-ttu-id="63289-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="63289-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="63289-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="63289-111">Permission type</span></span>|<span data-ttu-id="63289-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="63289-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="63289-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="63289-113">Delegated (work or school account)</span></span>|<span data-ttu-id="63289-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="63289-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="63289-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="63289-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="63289-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="63289-116">Not supported.</span></span>|
|<span data-ttu-id="63289-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="63289-117">Application</span></span>|<span data-ttu-id="63289-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="63289-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="63289-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="63289-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/iosUpdateStatuses/{iosUpdateDeviceStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="63289-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="63289-120">Request headers</span></span>
|<span data-ttu-id="63289-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="63289-121">Header</span></span>|<span data-ttu-id="63289-122">Valor</span><span class="sxs-lookup"><span data-stu-id="63289-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="63289-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="63289-123">Authorization</span></span>|<span data-ttu-id="63289-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="63289-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="63289-125">Accept</span><span class="sxs-lookup"><span data-stu-id="63289-125">Accept</span></span>|<span data-ttu-id="63289-126">application/json</span><span class="sxs-lookup"><span data-stu-id="63289-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="63289-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="63289-127">Request body</span></span>
<span data-ttu-id="63289-128">No corpo da solicitação, forneça uma representação JSON do objeto [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="63289-128">In the request body, supply a JSON representation for the [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) object.</span></span>

<span data-ttu-id="63289-129">A tabela a seguir mostra as propriedades obrigatórias ao criar [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="63289-129">The following table shows the properties that are required when you create the [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md).</span></span>

|<span data-ttu-id="63289-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="63289-130">Property</span></span>|<span data-ttu-id="63289-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="63289-131">Type</span></span>|<span data-ttu-id="63289-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="63289-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="63289-133">id</span><span class="sxs-lookup"><span data-stu-id="63289-133">id</span></span>|<span data-ttu-id="63289-134">String</span><span class="sxs-lookup"><span data-stu-id="63289-134">String</span></span>|<span data-ttu-id="63289-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="63289-135">Key of the entity.</span></span>|
|<span data-ttu-id="63289-136">installStatus</span><span class="sxs-lookup"><span data-stu-id="63289-136">installStatus</span></span>|[<span data-ttu-id="63289-137">iosUpdatesInstallStatus</span><span class="sxs-lookup"><span data-stu-id="63289-137">iosUpdatesInstallStatus</span></span>](../resources/intune-deviceconfig-iosupdatesinstallstatus.md)|<span data-ttu-id="63289-138">O status de instalação do relatório de políticas.</span><span class="sxs-lookup"><span data-stu-id="63289-138">The installation status of the policy report.</span></span> <span data-ttu-id="63289-139">Os valores possíveis são: `success`, `available`, `idle`, `unknown`, `downloading`, `downloadFailed`, `downloadRequiresComputer`, `downloadInsufficientSpace`, `downloadInsufficientPower`, `downloadInsufficientNetwork`, `installing`, `installInsufficientSpace`, `installInsufficientPower`, `installPhoneCallInProgress`, `installFailed`, `notSupportedOperation`, `sharedDeviceUserLoggedInError`.</span><span class="sxs-lookup"><span data-stu-id="63289-139">Possible values are: `success`, `available`, `idle`, `unknown`, `downloading`, `downloadFailed`, `downloadRequiresComputer`, `downloadInsufficientSpace`, `downloadInsufficientPower`, `downloadInsufficientNetwork`, `installing`, `installInsufficientSpace`, `installInsufficientPower`, `installPhoneCallInProgress`, `installFailed`, `notSupportedOperation`, `sharedDeviceUserLoggedInError`.</span></span>|
|<span data-ttu-id="63289-140">osVersion</span><span class="sxs-lookup"><span data-stu-id="63289-140">osVersion</span></span>|<span data-ttu-id="63289-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="63289-141">String</span></span>|<span data-ttu-id="63289-142">A versão do dispositivo que está sendo relatado.</span><span class="sxs-lookup"><span data-stu-id="63289-142">The device version that is being reported.</span></span>|
|<span data-ttu-id="63289-143">deviceId</span><span class="sxs-lookup"><span data-stu-id="63289-143">deviceId</span></span>|<span data-ttu-id="63289-144">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="63289-144">String</span></span>|<span data-ttu-id="63289-145">A ID do dispositivo que está sendo relatado.</span><span class="sxs-lookup"><span data-stu-id="63289-145">The device id that is being reported.</span></span>|
|<span data-ttu-id="63289-146">userId</span><span class="sxs-lookup"><span data-stu-id="63289-146">userId</span></span>|<span data-ttu-id="63289-147">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="63289-147">String</span></span>|<span data-ttu-id="63289-148">A ID do usuário que está sendo relatado.</span><span class="sxs-lookup"><span data-stu-id="63289-148">The User id that is being reported.</span></span>|
|<span data-ttu-id="63289-149">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="63289-149">deviceDisplayName</span></span>|<span data-ttu-id="63289-150">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="63289-150">String</span></span>|<span data-ttu-id="63289-151">Nome do dispositivo de DevicePolicyStatus.</span><span class="sxs-lookup"><span data-stu-id="63289-151">Device name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="63289-152">userName</span><span class="sxs-lookup"><span data-stu-id="63289-152">userName</span></span>|<span data-ttu-id="63289-153">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="63289-153">String</span></span>|<span data-ttu-id="63289-154">O nome de usuário que está sendo relatado</span><span class="sxs-lookup"><span data-stu-id="63289-154">The User Name that is being reported</span></span>|
|<span data-ttu-id="63289-155">deviceModel</span><span class="sxs-lookup"><span data-stu-id="63289-155">deviceModel</span></span>|<span data-ttu-id="63289-156">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="63289-156">String</span></span>|<span data-ttu-id="63289-157">O modelo do dispositivo que está sendo relatado</span><span class="sxs-lookup"><span data-stu-id="63289-157">The device model that is being reported</span></span>|
|<span data-ttu-id="63289-158">platform</span><span class="sxs-lookup"><span data-stu-id="63289-158">platform</span></span>|<span data-ttu-id="63289-159">Int32</span><span class="sxs-lookup"><span data-stu-id="63289-159">Int32</span></span>|<span data-ttu-id="63289-160">Plataforma do dispositivo que está sendo relatado</span><span class="sxs-lookup"><span data-stu-id="63289-160">Platform of the device that is being reported</span></span>|
|<span data-ttu-id="63289-161">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="63289-161">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="63289-162">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="63289-162">DateTimeOffset</span></span>|<span data-ttu-id="63289-163">DateTime em que o período de cortesia de conformidade do dispositivo termina</span><span class="sxs-lookup"><span data-stu-id="63289-163">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="63289-164">status</span><span class="sxs-lookup"><span data-stu-id="63289-164">status</span></span>|[<span data-ttu-id="63289-165">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="63289-165">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="63289-166">Status de conformidade do relatório de políticas.</span><span class="sxs-lookup"><span data-stu-id="63289-166">Compliance status of the policy report.</span></span> <span data-ttu-id="63289-167">Os valores possíveis são: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="63289-167">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="63289-168">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="63289-168">lastReportedDateTime</span></span>|<span data-ttu-id="63289-169">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="63289-169">DateTimeOffset</span></span>|<span data-ttu-id="63289-170">Data e hora da última modificação do relatório de políticas.</span><span class="sxs-lookup"><span data-stu-id="63289-170">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="63289-171">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="63289-171">userPrincipalName</span></span>|<span data-ttu-id="63289-172">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="63289-172">String</span></span>|<span data-ttu-id="63289-173">UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="63289-173">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="63289-174">Resposta</span><span class="sxs-lookup"><span data-stu-id="63289-174">Response</span></span>
<span data-ttu-id="63289-175">Se for bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="63289-175">If successful, this method returns a `200 OK` response code and an updated [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="63289-176">Exemplo</span><span class="sxs-lookup"><span data-stu-id="63289-176">Example</span></span>
### <a name="request"></a><span data-ttu-id="63289-177">Solicitação</span><span class="sxs-lookup"><span data-stu-id="63289-177">Request</span></span>
<span data-ttu-id="63289-178">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="63289-178">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/iosUpdateStatuses/{iosUpdateDeviceStatusId}
Content-type: application/json
Content-length: 510

{
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

### <a name="response"></a><span data-ttu-id="63289-179">Resposta</span><span class="sxs-lookup"><span data-stu-id="63289-179">Response</span></span>
<span data-ttu-id="63289-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="63289-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





