---
title: Criar iosUpdateDeviceStatus
description: Criar um novo objeto iosUpdateDeviceStatus.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 6f299c169c14cc48528e08c819e68411913b8db9
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27833919"
---
# <a name="create-iosupdatedevicestatus"></a><span data-ttu-id="4f72f-103">Criar iosUpdateDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="4f72f-103">Create iosUpdateDeviceStatus</span></span>

> <span data-ttu-id="4f72f-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="4f72f-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4f72f-105">Criar um novo objeto [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="4f72f-105">Create a new [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="4f72f-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="4f72f-106">Prerequisites</span></span>
<span data-ttu-id="4f72f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4f72f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4f72f-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4f72f-109">Permission type</span></span>|<span data-ttu-id="4f72f-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="4f72f-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4f72f-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4f72f-111">Delegated (work or school account)</span></span>|<span data-ttu-id="4f72f-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4f72f-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4f72f-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4f72f-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4f72f-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4f72f-114">Not supported.</span></span>|
|<span data-ttu-id="4f72f-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4f72f-115">Application</span></span>|<span data-ttu-id="4f72f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4f72f-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4f72f-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4f72f-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/iosUpdateStatuses
```

## <a name="request-headers"></a><span data-ttu-id="4f72f-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4f72f-118">Request headers</span></span>
|<span data-ttu-id="4f72f-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4f72f-119">Header</span></span>|<span data-ttu-id="4f72f-120">Valor</span><span class="sxs-lookup"><span data-stu-id="4f72f-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4f72f-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="4f72f-121">Authorization</span></span>|<span data-ttu-id="4f72f-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4f72f-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4f72f-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="4f72f-123">Accept</span></span>|<span data-ttu-id="4f72f-124">application/json</span><span class="sxs-lookup"><span data-stu-id="4f72f-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4f72f-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4f72f-125">Request body</span></span>
<span data-ttu-id="4f72f-126">No corpo da solicitação, forneça uma representação JSON do objeto iosUpdateDeviceStatus.</span><span class="sxs-lookup"><span data-stu-id="4f72f-126">In the request body, supply a JSON representation for the iosUpdateDeviceStatus object.</span></span>

<span data-ttu-id="4f72f-127">A tabela a seguir mostra as propriedades que são necessárias ao criar iosUpdateDeviceStatus.</span><span class="sxs-lookup"><span data-stu-id="4f72f-127">The following table shows the properties that are required when you create the iosUpdateDeviceStatus.</span></span>

|<span data-ttu-id="4f72f-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4f72f-128">Property</span></span>|<span data-ttu-id="4f72f-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="4f72f-129">Type</span></span>|<span data-ttu-id="4f72f-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="4f72f-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4f72f-131">id</span><span class="sxs-lookup"><span data-stu-id="4f72f-131">id</span></span>|<span data-ttu-id="4f72f-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4f72f-132">String</span></span>|<span data-ttu-id="4f72f-133">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="4f72f-133">Key of the entity.</span></span>|
|<span data-ttu-id="4f72f-134">installStatus</span><span class="sxs-lookup"><span data-stu-id="4f72f-134">installStatus</span></span>|[<span data-ttu-id="4f72f-135">iosUpdatesInstallStatus</span><span class="sxs-lookup"><span data-stu-id="4f72f-135">iosUpdatesInstallStatus</span></span>](../resources/intune-deviceconfig-iosupdatesinstallstatus.md)|<span data-ttu-id="4f72f-136">O status de instalação do relatório de políticas.</span><span class="sxs-lookup"><span data-stu-id="4f72f-136">The installation status of the policy report.</span></span> <span data-ttu-id="4f72f-137">Os valores possíveis são: `success`, `available`, `idle`, `unknown`, `downloading`, `downloadFailed`, `downloadRequiresComputer`, `downloadInsufficientSpace`, `downloadInsufficientPower`, `downloadInsufficientNetwork`, `installing`, `installInsufficientSpace`, `installInsufficientPower`, `installPhoneCallInProgress`, `installFailed`, `notSupportedOperation`, `sharedDeviceUserLoggedInError`.</span><span class="sxs-lookup"><span data-stu-id="4f72f-137">Possible values are: `success`, `available`, `idle`, `unknown`, `downloading`, `downloadFailed`, `downloadRequiresComputer`, `downloadInsufficientSpace`, `downloadInsufficientPower`, `downloadInsufficientNetwork`, `installing`, `installInsufficientSpace`, `installInsufficientPower`, `installPhoneCallInProgress`, `installFailed`, `notSupportedOperation`, `sharedDeviceUserLoggedInError`.</span></span>|
|<span data-ttu-id="4f72f-138">osVersion</span><span class="sxs-lookup"><span data-stu-id="4f72f-138">osVersion</span></span>|<span data-ttu-id="4f72f-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4f72f-139">String</span></span>|<span data-ttu-id="4f72f-140">A versão do dispositivo que está sendo relatado.</span><span class="sxs-lookup"><span data-stu-id="4f72f-140">The device version that is being reported.</span></span>|
|<span data-ttu-id="4f72f-141">deviceId</span><span class="sxs-lookup"><span data-stu-id="4f72f-141">deviceId</span></span>|<span data-ttu-id="4f72f-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4f72f-142">String</span></span>|<span data-ttu-id="4f72f-143">A ID do dispositivo que está sendo relatado.</span><span class="sxs-lookup"><span data-stu-id="4f72f-143">The device id that is being reported.</span></span>|
|<span data-ttu-id="4f72f-144">userId</span><span class="sxs-lookup"><span data-stu-id="4f72f-144">userId</span></span>|<span data-ttu-id="4f72f-145">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4f72f-145">String</span></span>|<span data-ttu-id="4f72f-146">A ID do usuário que está sendo relatado.</span><span class="sxs-lookup"><span data-stu-id="4f72f-146">The User id that is being reported.</span></span>|
|<span data-ttu-id="4f72f-147">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="4f72f-147">deviceDisplayName</span></span>|<span data-ttu-id="4f72f-148">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4f72f-148">String</span></span>|<span data-ttu-id="4f72f-149">Nome do dispositivo de DevicePolicyStatus.</span><span class="sxs-lookup"><span data-stu-id="4f72f-149">Device name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="4f72f-150">userName</span><span class="sxs-lookup"><span data-stu-id="4f72f-150">userName</span></span>|<span data-ttu-id="4f72f-151">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4f72f-151">String</span></span>|<span data-ttu-id="4f72f-152">O nome de usuário que está sendo relatado</span><span class="sxs-lookup"><span data-stu-id="4f72f-152">The User Name that is being reported</span></span>|
|<span data-ttu-id="4f72f-153">deviceModel</span><span class="sxs-lookup"><span data-stu-id="4f72f-153">deviceModel</span></span>|<span data-ttu-id="4f72f-154">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4f72f-154">String</span></span>|<span data-ttu-id="4f72f-155">O modelo do dispositivo que está sendo relatado</span><span class="sxs-lookup"><span data-stu-id="4f72f-155">The device model that is being reported</span></span>|
|<span data-ttu-id="4f72f-156">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="4f72f-156">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="4f72f-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4f72f-157">DateTimeOffset</span></span>|<span data-ttu-id="4f72f-158">DateTime em que o período de cortesia de conformidade do dispositivo termina</span><span class="sxs-lookup"><span data-stu-id="4f72f-158">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="4f72f-159">status</span><span class="sxs-lookup"><span data-stu-id="4f72f-159">status</span></span>|[<span data-ttu-id="4f72f-160">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="4f72f-160">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="4f72f-161">Status de conformidade do relatório de políticas.</span><span class="sxs-lookup"><span data-stu-id="4f72f-161">Compliance status of the policy report.</span></span> <span data-ttu-id="4f72f-162">Os valores possíveis são: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="4f72f-162">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="4f72f-163">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="4f72f-163">lastReportedDateTime</span></span>|<span data-ttu-id="4f72f-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4f72f-164">DateTimeOffset</span></span>|<span data-ttu-id="4f72f-165">Data e hora da última modificação do relatório de políticas.</span><span class="sxs-lookup"><span data-stu-id="4f72f-165">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="4f72f-166">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="4f72f-166">userPrincipalName</span></span>|<span data-ttu-id="4f72f-167">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4f72f-167">String</span></span>|<span data-ttu-id="4f72f-168">UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="4f72f-168">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="4f72f-169">Resposta</span><span class="sxs-lookup"><span data-stu-id="4f72f-169">Response</span></span>
<span data-ttu-id="4f72f-170">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4f72f-170">If successful, this method returns a `201 Created` response code and a [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4f72f-171">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4f72f-171">Example</span></span>
### <a name="request"></a><span data-ttu-id="4f72f-172">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4f72f-172">Request</span></span>
<span data-ttu-id="4f72f-173">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4f72f-173">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/iosUpdateStatuses
Content-type: application/json
Content-length: 552

{
  "@odata.type": "#microsoft.graph.iosUpdateDeviceStatus",
  "installStatus": "available",
  "osVersion": "Os Version value",
  "deviceId": "Device Id value",
  "userId": "User Id value",
  "deviceDisplayName": "Device Display Name value",
  "userName": "User Name value",
  "deviceModel": "Device Model value",
  "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00",
  "status": "notApplicable",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "userPrincipalName": "User Principal Name value"
}
```

### <a name="response"></a><span data-ttu-id="4f72f-174">Resposta</span><span class="sxs-lookup"><span data-stu-id="4f72f-174">Response</span></span>
<span data-ttu-id="4f72f-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4f72f-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 601

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
  "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00",
  "status": "notApplicable",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "userPrincipalName": "User Principal Name value"
}
```



