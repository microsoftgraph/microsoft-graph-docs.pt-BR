---
title: Atualizar iosUpdateDeviceStatus
description: Atualizar as propriedades de um objeto iosUpdateDeviceStatus.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: ea351a610ce18169af5dfa579de116b9d5564dea
ms.sourcegitcommit: dc3bade0c096d5ce716d4bc07cd9c7cabb52477b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/18/2020
ms.locfileid: "46790697"
---
# <a name="update-iosupdatedevicestatus"></a><span data-ttu-id="dd7dc-103">Atualizar iosUpdateDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="dd7dc-103">Update iosUpdateDeviceStatus</span></span>

<span data-ttu-id="dd7dc-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dd7dc-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="dd7dc-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="dd7dc-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dd7dc-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="dd7dc-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dd7dc-107">Atualizar as propriedades de um objeto [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="dd7dc-107">Update the properties of a [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="dd7dc-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="dd7dc-108">Prerequisites</span></span>
<span data-ttu-id="dd7dc-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dd7dc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dd7dc-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="dd7dc-111">Permission type</span></span>|<span data-ttu-id="dd7dc-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="dd7dc-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dd7dc-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="dd7dc-113">Delegated (work or school account)</span></span>|<span data-ttu-id="dd7dc-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dd7dc-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="dd7dc-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="dd7dc-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dd7dc-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dd7dc-116">Not supported.</span></span>|
|<span data-ttu-id="dd7dc-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="dd7dc-117">Application</span></span>|<span data-ttu-id="dd7dc-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dd7dc-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="dd7dc-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="dd7dc-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/iosUpdateStatuses/{iosUpdateDeviceStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="dd7dc-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="dd7dc-120">Request headers</span></span>
|<span data-ttu-id="dd7dc-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="dd7dc-121">Header</span></span>|<span data-ttu-id="dd7dc-122">Valor</span><span class="sxs-lookup"><span data-stu-id="dd7dc-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dd7dc-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="dd7dc-123">Authorization</span></span>|<span data-ttu-id="dd7dc-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dd7dc-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dd7dc-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="dd7dc-125">Accept</span></span>|<span data-ttu-id="dd7dc-126">application/json</span><span class="sxs-lookup"><span data-stu-id="dd7dc-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dd7dc-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="dd7dc-127">Request body</span></span>
<span data-ttu-id="dd7dc-128">No corpo da solicitação, forneça uma representação JSON do objeto [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="dd7dc-128">In the request body, supply a JSON representation for the [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) object.</span></span>

<span data-ttu-id="dd7dc-129">A tabela a seguir mostra as propriedades obrigatórias ao criar [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="dd7dc-129">The following table shows the properties that are required when you create the [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md).</span></span>

|<span data-ttu-id="dd7dc-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="dd7dc-130">Property</span></span>|<span data-ttu-id="dd7dc-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="dd7dc-131">Type</span></span>|<span data-ttu-id="dd7dc-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="dd7dc-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dd7dc-133">id</span><span class="sxs-lookup"><span data-stu-id="dd7dc-133">id</span></span>|<span data-ttu-id="dd7dc-134">String</span><span class="sxs-lookup"><span data-stu-id="dd7dc-134">String</span></span>|<span data-ttu-id="dd7dc-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="dd7dc-135">Key of the entity.</span></span>|
|<span data-ttu-id="dd7dc-136">installStatus</span><span class="sxs-lookup"><span data-stu-id="dd7dc-136">installStatus</span></span>|[<span data-ttu-id="dd7dc-137">iosUpdatesInstallStatus</span><span class="sxs-lookup"><span data-stu-id="dd7dc-137">iosUpdatesInstallStatus</span></span>](../resources/intune-deviceconfig-iosupdatesinstallstatus.md)|<span data-ttu-id="dd7dc-138">O status de instalação do relatório de políticas.</span><span class="sxs-lookup"><span data-stu-id="dd7dc-138">The installation status of the policy report.</span></span> <span data-ttu-id="dd7dc-139">Os valores possíveis são:,,,,,,,,,,,,,,,,,,,, `success` `available` `idle` `unknown` `mdmClientCrashed` `timeout` `downloading` `downloadFailed` `downloadRequiresComputer` `downloadInsufficientSpace` `downloadInsufficientPower` `downloadInsufficientNetwork` `installing` , `installInsufficientSpace` , `installInsufficientPower` ,, `installPhoneCallInProgress` `installFailed` , `notSupportedOperation` `sharedDeviceUserLoggedInError` `updateError` `deviceOsHigherThanDesiredOsVersion` `updateScanFailed` ,,,,,.</span><span class="sxs-lookup"><span data-stu-id="dd7dc-139">Possible values are: `success`, `available`, `idle`, `unknown`, `mdmClientCrashed`, `timeout`, `downloading`, `downloadFailed`, `downloadRequiresComputer`, `downloadInsufficientSpace`, `downloadInsufficientPower`, `downloadInsufficientNetwork`, `installing`, `installInsufficientSpace`, `installInsufficientPower`, `installPhoneCallInProgress`, `installFailed`, `notSupportedOperation`, `sharedDeviceUserLoggedInError`, `updateError`, `deviceOsHigherThanDesiredOsVersion`, `updateScanFailed`.</span></span>|
|<span data-ttu-id="dd7dc-140">osVersion</span><span class="sxs-lookup"><span data-stu-id="dd7dc-140">osVersion</span></span>|<span data-ttu-id="dd7dc-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="dd7dc-141">String</span></span>|<span data-ttu-id="dd7dc-142">A versão do dispositivo que está sendo relatado.</span><span class="sxs-lookup"><span data-stu-id="dd7dc-142">The device version that is being reported.</span></span>|
|<span data-ttu-id="dd7dc-143">deviceId</span><span class="sxs-lookup"><span data-stu-id="dd7dc-143">deviceId</span></span>|<span data-ttu-id="dd7dc-144">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="dd7dc-144">String</span></span>|<span data-ttu-id="dd7dc-145">A ID do dispositivo que está sendo relatado.</span><span class="sxs-lookup"><span data-stu-id="dd7dc-145">The device id that is being reported.</span></span>|
|<span data-ttu-id="dd7dc-146">userId</span><span class="sxs-lookup"><span data-stu-id="dd7dc-146">userId</span></span>|<span data-ttu-id="dd7dc-147">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="dd7dc-147">String</span></span>|<span data-ttu-id="dd7dc-148">A ID do usuário que está sendo relatado.</span><span class="sxs-lookup"><span data-stu-id="dd7dc-148">The User id that is being reported.</span></span>|
|<span data-ttu-id="dd7dc-149">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="dd7dc-149">deviceDisplayName</span></span>|<span data-ttu-id="dd7dc-150">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="dd7dc-150">String</span></span>|<span data-ttu-id="dd7dc-151">Nome do dispositivo de DevicePolicyStatus.</span><span class="sxs-lookup"><span data-stu-id="dd7dc-151">Device name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="dd7dc-152">userName</span><span class="sxs-lookup"><span data-stu-id="dd7dc-152">userName</span></span>|<span data-ttu-id="dd7dc-153">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="dd7dc-153">String</span></span>|<span data-ttu-id="dd7dc-154">O nome de usuário que está sendo relatado</span><span class="sxs-lookup"><span data-stu-id="dd7dc-154">The User Name that is being reported</span></span>|
|<span data-ttu-id="dd7dc-155">deviceModel</span><span class="sxs-lookup"><span data-stu-id="dd7dc-155">deviceModel</span></span>|<span data-ttu-id="dd7dc-156">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="dd7dc-156">String</span></span>|<span data-ttu-id="dd7dc-157">O modelo do dispositivo que está sendo relatado</span><span class="sxs-lookup"><span data-stu-id="dd7dc-157">The device model that is being reported</span></span>|
|<span data-ttu-id="dd7dc-158">plataforma</span><span class="sxs-lookup"><span data-stu-id="dd7dc-158">platform</span></span>|<span data-ttu-id="dd7dc-159">Int32</span><span class="sxs-lookup"><span data-stu-id="dd7dc-159">Int32</span></span>|<span data-ttu-id="dd7dc-160">Plataforma do dispositivo que está sendo relatado</span><span class="sxs-lookup"><span data-stu-id="dd7dc-160">Platform of the device that is being reported</span></span>|
|<span data-ttu-id="dd7dc-161">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="dd7dc-161">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="dd7dc-162">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dd7dc-162">DateTimeOffset</span></span>|<span data-ttu-id="dd7dc-163">DateTime em que o período de cortesia de conformidade do dispositivo termina</span><span class="sxs-lookup"><span data-stu-id="dd7dc-163">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="dd7dc-164">status</span><span class="sxs-lookup"><span data-stu-id="dd7dc-164">status</span></span>|[<span data-ttu-id="dd7dc-165">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="dd7dc-165">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="dd7dc-166">Status de conformidade do relatório de políticas.</span><span class="sxs-lookup"><span data-stu-id="dd7dc-166">Compliance status of the policy report.</span></span> <span data-ttu-id="dd7dc-167">Os valores possíveis são: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="dd7dc-167">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="dd7dc-168">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="dd7dc-168">lastReportedDateTime</span></span>|<span data-ttu-id="dd7dc-169">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dd7dc-169">DateTimeOffset</span></span>|<span data-ttu-id="dd7dc-170">Data e hora da última modificação do relatório de políticas.</span><span class="sxs-lookup"><span data-stu-id="dd7dc-170">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="dd7dc-171">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="dd7dc-171">userPrincipalName</span></span>|<span data-ttu-id="dd7dc-172">String</span><span class="sxs-lookup"><span data-stu-id="dd7dc-172">String</span></span>|<span data-ttu-id="dd7dc-173">UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="dd7dc-173">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="dd7dc-174">Resposta</span><span class="sxs-lookup"><span data-stu-id="dd7dc-174">Response</span></span>
<span data-ttu-id="dd7dc-175">Se for bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="dd7dc-175">If successful, this method returns a `200 OK` response code and an updated [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dd7dc-176">Exemplo</span><span class="sxs-lookup"><span data-stu-id="dd7dc-176">Example</span></span>

### <a name="request"></a><span data-ttu-id="dd7dc-177">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dd7dc-177">Request</span></span>
<span data-ttu-id="dd7dc-178">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="dd7dc-178">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/iosUpdateStatuses/{iosUpdateDeviceStatusId}
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

### <a name="response"></a><span data-ttu-id="dd7dc-179">Resposta</span><span class="sxs-lookup"><span data-stu-id="dd7dc-179">Response</span></span>
<span data-ttu-id="dd7dc-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="dd7dc-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



