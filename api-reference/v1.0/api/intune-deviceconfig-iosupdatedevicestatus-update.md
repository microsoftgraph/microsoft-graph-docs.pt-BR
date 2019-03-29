---
title: Atualizar iosUpdateDeviceStatus
description: Atualizar as propriedades de um objeto iosUpdateDeviceStatus.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ede7348a948d78c2ec9f3219fa1ff072d17915f3
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/29/2019
ms.locfileid: "30957917"
---
# <a name="update-iosupdatedevicestatus"></a><span data-ttu-id="bb70d-103">Atualizar iosUpdateDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="bb70d-103">Update iosUpdateDeviceStatus</span></span>

> <span data-ttu-id="bb70d-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="bb70d-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bb70d-105">Atualizar as propriedades de um objeto [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="bb70d-105">Update the properties of a [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bb70d-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="bb70d-106">Prerequisites</span></span>
<span data-ttu-id="bb70d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bb70d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bb70d-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bb70d-109">Permission type</span></span>|<span data-ttu-id="bb70d-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="bb70d-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bb70d-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bb70d-111">Delegated (work or school account)</span></span>|<span data-ttu-id="bb70d-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bb70d-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="bb70d-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bb70d-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bb70d-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bb70d-114">Not supported.</span></span>|
|<span data-ttu-id="bb70d-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bb70d-115">Application</span></span>|<span data-ttu-id="bb70d-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bb70d-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bb70d-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bb70d-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/iosUpdateStatuses/{iosUpdateDeviceStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="bb70d-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bb70d-118">Request headers</span></span>
|<span data-ttu-id="bb70d-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="bb70d-119">Header</span></span>|<span data-ttu-id="bb70d-120">Valor</span><span class="sxs-lookup"><span data-stu-id="bb70d-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bb70d-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="bb70d-121">Authorization</span></span>|<span data-ttu-id="bb70d-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bb70d-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bb70d-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="bb70d-123">Accept</span></span>|<span data-ttu-id="bb70d-124">application/json</span><span class="sxs-lookup"><span data-stu-id="bb70d-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bb70d-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bb70d-125">Request body</span></span>
<span data-ttu-id="bb70d-126">No corpo da solicitação, forneça uma representação JSON do objeto [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="bb70d-126">In the request body, supply a JSON representation for the [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) object.</span></span>

<span data-ttu-id="bb70d-127">A tabela a seguir mostra as propriedades obrigatórias ao criar [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="bb70d-127">The following table shows the properties that are required when you create the [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md).</span></span>

|<span data-ttu-id="bb70d-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bb70d-128">Property</span></span>|<span data-ttu-id="bb70d-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="bb70d-129">Type</span></span>|<span data-ttu-id="bb70d-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="bb70d-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bb70d-131">id</span><span class="sxs-lookup"><span data-stu-id="bb70d-131">id</span></span>|<span data-ttu-id="bb70d-132">String</span><span class="sxs-lookup"><span data-stu-id="bb70d-132">String</span></span>|<span data-ttu-id="bb70d-133">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="bb70d-133">Key of the entity.</span></span>|
|<span data-ttu-id="bb70d-134">installStatus</span><span class="sxs-lookup"><span data-stu-id="bb70d-134">installStatus</span></span>|[<span data-ttu-id="bb70d-135">iosUpdatesInstallStatus</span><span class="sxs-lookup"><span data-stu-id="bb70d-135">iosUpdatesInstallStatus</span></span>](../resources/intune-deviceconfig-iosupdatesinstallstatus.md)|<span data-ttu-id="bb70d-136">O status de instalação do relatório de políticas.</span><span class="sxs-lookup"><span data-stu-id="bb70d-136">The installation status of the policy report.</span></span> <span data-ttu-id="bb70d-137">Os valores possíveis são `success`: `available`, `idle`, `unknown`, `downloading`, `downloadFailed`, `downloadRequiresComputer`, `downloadInsufficientSpace`, `downloadInsufficientPower`, `downloadInsufficientNetwork`, `installing`, `installInsufficientSpace`, `installInsufficientPower`, `installPhoneCallInProgress`, `installFailed`, `notSupportedOperation`, `sharedDeviceUserLoggedInError`,,,,,,,,,.</span><span class="sxs-lookup"><span data-stu-id="bb70d-137">Possible values are: `success`, `available`, `idle`, `unknown`, `downloading`, `downloadFailed`, `downloadRequiresComputer`, `downloadInsufficientSpace`, `downloadInsufficientPower`, `downloadInsufficientNetwork`, `installing`, `installInsufficientSpace`, `installInsufficientPower`, `installPhoneCallInProgress`, `installFailed`, `notSupportedOperation`, `sharedDeviceUserLoggedInError`.</span></span>|
|<span data-ttu-id="bb70d-138">osVersion</span><span class="sxs-lookup"><span data-stu-id="bb70d-138">osVersion</span></span>|<span data-ttu-id="bb70d-139">String</span><span class="sxs-lookup"><span data-stu-id="bb70d-139">String</span></span>|<span data-ttu-id="bb70d-140">A versão do dispositivo que está sendo relatado.</span><span class="sxs-lookup"><span data-stu-id="bb70d-140">The device version that is being reported.</span></span>|
|<span data-ttu-id="bb70d-141">deviceId</span><span class="sxs-lookup"><span data-stu-id="bb70d-141">deviceId</span></span>|<span data-ttu-id="bb70d-142">String</span><span class="sxs-lookup"><span data-stu-id="bb70d-142">String</span></span>|<span data-ttu-id="bb70d-143">A ID do dispositivo que está sendo relatado.</span><span class="sxs-lookup"><span data-stu-id="bb70d-143">The device id that is being reported.</span></span>|
|<span data-ttu-id="bb70d-144">userId</span><span class="sxs-lookup"><span data-stu-id="bb70d-144">userId</span></span>|<span data-ttu-id="bb70d-145">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bb70d-145">String</span></span>|<span data-ttu-id="bb70d-146">A ID do usuário que está sendo relatado.</span><span class="sxs-lookup"><span data-stu-id="bb70d-146">The User id that is being reported.</span></span>|
|<span data-ttu-id="bb70d-147">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="bb70d-147">deviceDisplayName</span></span>|<span data-ttu-id="bb70d-148">String</span><span class="sxs-lookup"><span data-stu-id="bb70d-148">String</span></span>|<span data-ttu-id="bb70d-149">Nome do dispositivo de DevicePolicyStatus.</span><span class="sxs-lookup"><span data-stu-id="bb70d-149">Device name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="bb70d-150">userName</span><span class="sxs-lookup"><span data-stu-id="bb70d-150">userName</span></span>|<span data-ttu-id="bb70d-151">String</span><span class="sxs-lookup"><span data-stu-id="bb70d-151">String</span></span>|<span data-ttu-id="bb70d-152">O nome de usuário que está sendo relatado</span><span class="sxs-lookup"><span data-stu-id="bb70d-152">The User Name that is being reported</span></span>|
|<span data-ttu-id="bb70d-153">deviceModel</span><span class="sxs-lookup"><span data-stu-id="bb70d-153">deviceModel</span></span>|<span data-ttu-id="bb70d-154">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bb70d-154">String</span></span>|<span data-ttu-id="bb70d-155">O modelo do dispositivo que está sendo relatado</span><span class="sxs-lookup"><span data-stu-id="bb70d-155">The device model that is being reported</span></span>|
|<span data-ttu-id="bb70d-156">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="bb70d-156">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="bb70d-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bb70d-157">DateTimeOffset</span></span>|<span data-ttu-id="bb70d-158">DateTime em que o período de cortesia de conformidade do dispositivo termina</span><span class="sxs-lookup"><span data-stu-id="bb70d-158">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="bb70d-159">status</span><span class="sxs-lookup"><span data-stu-id="bb70d-159">status</span></span>|[<span data-ttu-id="bb70d-160">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="bb70d-160">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="bb70d-161">Status de conformidade do relatório de políticas.</span><span class="sxs-lookup"><span data-stu-id="bb70d-161">Compliance status of the policy report.</span></span> <span data-ttu-id="bb70d-162">Os valores possíveis são: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="bb70d-162">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="bb70d-163">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="bb70d-163">lastReportedDateTime</span></span>|<span data-ttu-id="bb70d-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bb70d-164">DateTimeOffset</span></span>|<span data-ttu-id="bb70d-165">Data e hora da última modificação do relatório de políticas.</span><span class="sxs-lookup"><span data-stu-id="bb70d-165">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="bb70d-166">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="bb70d-166">userPrincipalName</span></span>|<span data-ttu-id="bb70d-167">String</span><span class="sxs-lookup"><span data-stu-id="bb70d-167">String</span></span>|<span data-ttu-id="bb70d-168">UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="bb70d-168">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="bb70d-169">Resposta</span><span class="sxs-lookup"><span data-stu-id="bb70d-169">Response</span></span>
<span data-ttu-id="bb70d-170">Se for bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bb70d-170">If successful, this method returns a `200 OK` response code and an updated [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bb70d-171">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bb70d-171">Example</span></span>

### <a name="request"></a><span data-ttu-id="bb70d-172">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bb70d-172">Request</span></span>
<span data-ttu-id="bb70d-173">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="bb70d-173">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="bb70d-174">Resposta</span><span class="sxs-lookup"><span data-stu-id="bb70d-174">Response</span></span>
<span data-ttu-id="bb70d-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="bb70d-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



