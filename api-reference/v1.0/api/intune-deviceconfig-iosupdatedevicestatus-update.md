---
title: Atualizar iosUpdateDeviceStatus
description: Atualizar as propriedades de um objeto iosUpdateDeviceStatus.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 0f3b6e10719ac13bb8fb483a837154cd83da553a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27820360"
---
# <a name="update-iosupdatedevicestatus"></a><span data-ttu-id="1821b-103">Atualizar iosUpdateDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="1821b-103">Update iosUpdateDeviceStatus</span></span>

> <span data-ttu-id="1821b-104">**Observação:** o uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="1821b-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1821b-105">Atualizar as propriedades de um objeto [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="1821b-105">Update the properties of a [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="1821b-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="1821b-106">Prerequisites</span></span>
<span data-ttu-id="1821b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1821b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1821b-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1821b-109">Permission type</span></span>|<span data-ttu-id="1821b-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="1821b-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1821b-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1821b-111">Delegated (work or school account)</span></span>|<span data-ttu-id="1821b-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1821b-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="1821b-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1821b-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1821b-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1821b-114">Not supported.</span></span>|
|<span data-ttu-id="1821b-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1821b-115">Application</span></span>|<span data-ttu-id="1821b-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1821b-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1821b-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1821b-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/iosUpdateStatuses/{iosUpdateDeviceStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="1821b-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1821b-118">Request headers</span></span>
|<span data-ttu-id="1821b-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1821b-119">Header</span></span>|<span data-ttu-id="1821b-120">Valor</span><span class="sxs-lookup"><span data-stu-id="1821b-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1821b-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="1821b-121">Authorization</span></span>|<span data-ttu-id="1821b-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1821b-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1821b-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="1821b-123">Accept</span></span>|<span data-ttu-id="1821b-124">application/json</span><span class="sxs-lookup"><span data-stu-id="1821b-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1821b-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1821b-125">Request body</span></span>
<span data-ttu-id="1821b-126">No corpo da solicitação, forneça uma representação JSON do objeto [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="1821b-126">In the request body, supply a JSON representation for the [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) object.</span></span>

<span data-ttu-id="1821b-127">A tabela a seguir mostra as propriedades obrigatórias ao criar [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="1821b-127">The following table shows the properties that are required when you create the [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md).</span></span>

|<span data-ttu-id="1821b-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1821b-128">Property</span></span>|<span data-ttu-id="1821b-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="1821b-129">Type</span></span>|<span data-ttu-id="1821b-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="1821b-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1821b-131">id</span><span class="sxs-lookup"><span data-stu-id="1821b-131">id</span></span>|<span data-ttu-id="1821b-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1821b-132">String</span></span>|<span data-ttu-id="1821b-133">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="1821b-133">Key of the entity.</span></span>|
|<span data-ttu-id="1821b-134">installStatus</span><span class="sxs-lookup"><span data-stu-id="1821b-134">installStatus</span></span>|[<span data-ttu-id="1821b-135">iosUpdatesInstallStatus</span><span class="sxs-lookup"><span data-stu-id="1821b-135">iosUpdatesInstallStatus</span></span>](../resources/intune-deviceconfig-iosupdatesinstallstatus.md)|<span data-ttu-id="1821b-136">O status de instalação do relatório de políticas.</span><span class="sxs-lookup"><span data-stu-id="1821b-136">The installation status of the policy report.</span></span> <span data-ttu-id="1821b-137">Os valores possíveis são: `success`, `available`, `idle`, `unknown`, `downloading`, `downloadFailed`, `downloadRequiresComputer`, `downloadInsufficientSpace`, `downloadInsufficientPower`, `downloadInsufficientNetwork`, `installing`, `installInsufficientSpace`, `installInsufficientPower`, `installPhoneCallInProgress`, `installFailed`, `notSupportedOperation`, `sharedDeviceUserLoggedInError`.</span><span class="sxs-lookup"><span data-stu-id="1821b-137">Possible values are: `success`, `available`, `idle`, `unknown`, `downloading`, `downloadFailed`, `downloadRequiresComputer`, `downloadInsufficientSpace`, `downloadInsufficientPower`, `downloadInsufficientNetwork`, `installing`, `installInsufficientSpace`, `installInsufficientPower`, `installPhoneCallInProgress`, `installFailed`, `notSupportedOperation`, `sharedDeviceUserLoggedInError`.</span></span>|
|<span data-ttu-id="1821b-138">osVersion</span><span class="sxs-lookup"><span data-stu-id="1821b-138">osVersion</span></span>|<span data-ttu-id="1821b-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1821b-139">String</span></span>|<span data-ttu-id="1821b-140">A versão do dispositivo que está sendo relatado.</span><span class="sxs-lookup"><span data-stu-id="1821b-140">The device version that is being reported.</span></span>|
|<span data-ttu-id="1821b-141">deviceId</span><span class="sxs-lookup"><span data-stu-id="1821b-141">deviceId</span></span>|<span data-ttu-id="1821b-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1821b-142">String</span></span>|<span data-ttu-id="1821b-143">A ID do dispositivo que está sendo relatado.</span><span class="sxs-lookup"><span data-stu-id="1821b-143">The device id that is being reported.</span></span>|
|<span data-ttu-id="1821b-144">userId</span><span class="sxs-lookup"><span data-stu-id="1821b-144">userId</span></span>|<span data-ttu-id="1821b-145">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1821b-145">String</span></span>|<span data-ttu-id="1821b-146">A ID do usuário que está sendo relatado.</span><span class="sxs-lookup"><span data-stu-id="1821b-146">The User id that is being reported.</span></span>|
|<span data-ttu-id="1821b-147">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="1821b-147">deviceDisplayName</span></span>|<span data-ttu-id="1821b-148">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1821b-148">String</span></span>|<span data-ttu-id="1821b-149">Nome do dispositivo de DevicePolicyStatus.</span><span class="sxs-lookup"><span data-stu-id="1821b-149">Device name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="1821b-150">userName</span><span class="sxs-lookup"><span data-stu-id="1821b-150">userName</span></span>|<span data-ttu-id="1821b-151">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1821b-151">String</span></span>|<span data-ttu-id="1821b-152">O nome de usuário que está sendo relatado</span><span class="sxs-lookup"><span data-stu-id="1821b-152">The User Name that is being reported</span></span>|
|<span data-ttu-id="1821b-153">deviceModel</span><span class="sxs-lookup"><span data-stu-id="1821b-153">deviceModel</span></span>|<span data-ttu-id="1821b-154">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1821b-154">String</span></span>|<span data-ttu-id="1821b-155">O modelo do dispositivo que está sendo relatado</span><span class="sxs-lookup"><span data-stu-id="1821b-155">The device model that is being reported</span></span>|
|<span data-ttu-id="1821b-156">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="1821b-156">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="1821b-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1821b-157">DateTimeOffset</span></span>|<span data-ttu-id="1821b-158">DateTime em que o período de cortesia de conformidade do dispositivo termina</span><span class="sxs-lookup"><span data-stu-id="1821b-158">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="1821b-159">status</span><span class="sxs-lookup"><span data-stu-id="1821b-159">status</span></span>|[<span data-ttu-id="1821b-160">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="1821b-160">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="1821b-161">Status de conformidade do relatório de políticas.</span><span class="sxs-lookup"><span data-stu-id="1821b-161">Compliance status of the policy report.</span></span> <span data-ttu-id="1821b-162">Os valores possíveis são: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="1821b-162">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="1821b-163">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="1821b-163">lastReportedDateTime</span></span>|<span data-ttu-id="1821b-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1821b-164">DateTimeOffset</span></span>|<span data-ttu-id="1821b-165">Data e hora da última modificação do relatório de políticas.</span><span class="sxs-lookup"><span data-stu-id="1821b-165">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="1821b-166">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="1821b-166">userPrincipalName</span></span>|<span data-ttu-id="1821b-167">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1821b-167">String</span></span>|<span data-ttu-id="1821b-168">UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="1821b-168">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="1821b-169">Resposta</span><span class="sxs-lookup"><span data-stu-id="1821b-169">Response</span></span>
<span data-ttu-id="1821b-170">Se for bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1821b-170">If successful, this method returns a `200 OK` response code and an updated [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1821b-171">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1821b-171">Example</span></span>
### <a name="request"></a><span data-ttu-id="1821b-172">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1821b-172">Request</span></span>
<span data-ttu-id="1821b-173">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1821b-173">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/iosUpdateStatuses/{iosUpdateDeviceStatusId}
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

### <a name="response"></a><span data-ttu-id="1821b-174">Resposta</span><span class="sxs-lookup"><span data-stu-id="1821b-174">Response</span></span>
<span data-ttu-id="1821b-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1821b-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



