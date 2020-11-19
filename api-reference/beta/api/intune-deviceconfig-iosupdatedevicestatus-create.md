---
title: Criar iosUpdateDeviceStatus
description: Criar um novo objeto iosUpdateDeviceStatus.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 29344bae3a28e23f5ab62e7f6bd3a4d107de228a
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49205676"
---
# <a name="create-iosupdatedevicestatus"></a><span data-ttu-id="039a5-103">Criar iosUpdateDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="039a5-103">Create iosUpdateDeviceStatus</span></span>

<span data-ttu-id="039a5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="039a5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="039a5-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="039a5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="039a5-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="039a5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="039a5-107">Criar um novo objeto [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="039a5-107">Create a new [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="039a5-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="039a5-108">Prerequisites</span></span>
<span data-ttu-id="039a5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="039a5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="039a5-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="039a5-111">Permission type</span></span>|<span data-ttu-id="039a5-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="039a5-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="039a5-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="039a5-113">Delegated (work or school account)</span></span>|<span data-ttu-id="039a5-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="039a5-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="039a5-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="039a5-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="039a5-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="039a5-116">Not supported.</span></span>|
|<span data-ttu-id="039a5-117">Application</span><span class="sxs-lookup"><span data-stu-id="039a5-117">Application</span></span>|<span data-ttu-id="039a5-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="039a5-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="039a5-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="039a5-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/iosUpdateStatuses
```

## <a name="request-headers"></a><span data-ttu-id="039a5-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="039a5-120">Request headers</span></span>
|<span data-ttu-id="039a5-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="039a5-121">Header</span></span>|<span data-ttu-id="039a5-122">Valor</span><span class="sxs-lookup"><span data-stu-id="039a5-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="039a5-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="039a5-123">Authorization</span></span>|<span data-ttu-id="039a5-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="039a5-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="039a5-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="039a5-125">Accept</span></span>|<span data-ttu-id="039a5-126">application/json</span><span class="sxs-lookup"><span data-stu-id="039a5-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="039a5-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="039a5-127">Request body</span></span>
<span data-ttu-id="039a5-128">No corpo da solicitação, forneça uma representação JSON do objeto iosUpdateDeviceStatus.</span><span class="sxs-lookup"><span data-stu-id="039a5-128">In the request body, supply a JSON representation for the iosUpdateDeviceStatus object.</span></span>

<span data-ttu-id="039a5-129">A tabela a seguir mostra as propriedades que são necessárias ao criar iosUpdateDeviceStatus.</span><span class="sxs-lookup"><span data-stu-id="039a5-129">The following table shows the properties that are required when you create the iosUpdateDeviceStatus.</span></span>

|<span data-ttu-id="039a5-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="039a5-130">Property</span></span>|<span data-ttu-id="039a5-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="039a5-131">Type</span></span>|<span data-ttu-id="039a5-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="039a5-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="039a5-133">id</span><span class="sxs-lookup"><span data-stu-id="039a5-133">id</span></span>|<span data-ttu-id="039a5-134">String</span><span class="sxs-lookup"><span data-stu-id="039a5-134">String</span></span>|<span data-ttu-id="039a5-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="039a5-135">Key of the entity.</span></span>|
|<span data-ttu-id="039a5-136">installStatus</span><span class="sxs-lookup"><span data-stu-id="039a5-136">installStatus</span></span>|[<span data-ttu-id="039a5-137">iosUpdatesInstallStatus</span><span class="sxs-lookup"><span data-stu-id="039a5-137">iosUpdatesInstallStatus</span></span>](../resources/intune-deviceconfig-iosupdatesinstallstatus.md)|<span data-ttu-id="039a5-138">O status de instalação do relatório de políticas.</span><span class="sxs-lookup"><span data-stu-id="039a5-138">The installation status of the policy report.</span></span> <span data-ttu-id="039a5-139">Os valores possíveis são:,,,,,,,,,,,,,,,,,,,, `success` `available` `idle` `unknown` `mdmClientCrashed` `timeout` `downloading` `downloadFailed` `downloadRequiresComputer` `downloadInsufficientSpace` `downloadInsufficientPower` `downloadInsufficientNetwork` `installing` , `installInsufficientSpace` , `installInsufficientPower` ,, `installPhoneCallInProgress` `installFailed` , `notSupportedOperation` `sharedDeviceUserLoggedInError` `updateError` `deviceOsHigherThanDesiredOsVersion` `updateScanFailed` ,,,,,.</span><span class="sxs-lookup"><span data-stu-id="039a5-139">Possible values are: `success`, `available`, `idle`, `unknown`, `mdmClientCrashed`, `timeout`, `downloading`, `downloadFailed`, `downloadRequiresComputer`, `downloadInsufficientSpace`, `downloadInsufficientPower`, `downloadInsufficientNetwork`, `installing`, `installInsufficientSpace`, `installInsufficientPower`, `installPhoneCallInProgress`, `installFailed`, `notSupportedOperation`, `sharedDeviceUserLoggedInError`, `updateError`, `deviceOsHigherThanDesiredOsVersion`, `updateScanFailed`.</span></span>|
|<span data-ttu-id="039a5-140">osVersion</span><span class="sxs-lookup"><span data-stu-id="039a5-140">osVersion</span></span>|<span data-ttu-id="039a5-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="039a5-141">String</span></span>|<span data-ttu-id="039a5-142">A versão do dispositivo que está sendo relatado.</span><span class="sxs-lookup"><span data-stu-id="039a5-142">The device version that is being reported.</span></span>|
|<span data-ttu-id="039a5-143">deviceId</span><span class="sxs-lookup"><span data-stu-id="039a5-143">deviceId</span></span>|<span data-ttu-id="039a5-144">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="039a5-144">String</span></span>|<span data-ttu-id="039a5-145">A ID do dispositivo que está sendo relatado.</span><span class="sxs-lookup"><span data-stu-id="039a5-145">The device id that is being reported.</span></span>|
|<span data-ttu-id="039a5-146">userId</span><span class="sxs-lookup"><span data-stu-id="039a5-146">userId</span></span>|<span data-ttu-id="039a5-147">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="039a5-147">String</span></span>|<span data-ttu-id="039a5-148">A ID do usuário que está sendo relatado.</span><span class="sxs-lookup"><span data-stu-id="039a5-148">The User id that is being reported.</span></span>|
|<span data-ttu-id="039a5-149">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="039a5-149">deviceDisplayName</span></span>|<span data-ttu-id="039a5-150">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="039a5-150">String</span></span>|<span data-ttu-id="039a5-151">Nome do dispositivo de DevicePolicyStatus.</span><span class="sxs-lookup"><span data-stu-id="039a5-151">Device name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="039a5-152">userName</span><span class="sxs-lookup"><span data-stu-id="039a5-152">userName</span></span>|<span data-ttu-id="039a5-153">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="039a5-153">String</span></span>|<span data-ttu-id="039a5-154">O nome de usuário que está sendo relatado</span><span class="sxs-lookup"><span data-stu-id="039a5-154">The User Name that is being reported</span></span>|
|<span data-ttu-id="039a5-155">deviceModel</span><span class="sxs-lookup"><span data-stu-id="039a5-155">deviceModel</span></span>|<span data-ttu-id="039a5-156">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="039a5-156">String</span></span>|<span data-ttu-id="039a5-157">O modelo do dispositivo que está sendo relatado</span><span class="sxs-lookup"><span data-stu-id="039a5-157">The device model that is being reported</span></span>|
|<span data-ttu-id="039a5-158">plataforma</span><span class="sxs-lookup"><span data-stu-id="039a5-158">platform</span></span>|<span data-ttu-id="039a5-159">Int32</span><span class="sxs-lookup"><span data-stu-id="039a5-159">Int32</span></span>|<span data-ttu-id="039a5-160">Plataforma do dispositivo que está sendo relatado</span><span class="sxs-lookup"><span data-stu-id="039a5-160">Platform of the device that is being reported</span></span>|
|<span data-ttu-id="039a5-161">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="039a5-161">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="039a5-162">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="039a5-162">DateTimeOffset</span></span>|<span data-ttu-id="039a5-163">DateTime em que o período de cortesia de conformidade do dispositivo termina</span><span class="sxs-lookup"><span data-stu-id="039a5-163">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="039a5-164">status</span><span class="sxs-lookup"><span data-stu-id="039a5-164">status</span></span>|[<span data-ttu-id="039a5-165">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="039a5-165">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="039a5-166">Status de conformidade do relatório de políticas.</span><span class="sxs-lookup"><span data-stu-id="039a5-166">Compliance status of the policy report.</span></span> <span data-ttu-id="039a5-167">Os valores possíveis são: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="039a5-167">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="039a5-168">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="039a5-168">lastReportedDateTime</span></span>|<span data-ttu-id="039a5-169">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="039a5-169">DateTimeOffset</span></span>|<span data-ttu-id="039a5-170">Data e hora da última modificação do relatório de políticas.</span><span class="sxs-lookup"><span data-stu-id="039a5-170">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="039a5-171">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="039a5-171">userPrincipalName</span></span>|<span data-ttu-id="039a5-172">String</span><span class="sxs-lookup"><span data-stu-id="039a5-172">String</span></span>|<span data-ttu-id="039a5-173">UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="039a5-173">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="039a5-174">Resposta</span><span class="sxs-lookup"><span data-stu-id="039a5-174">Response</span></span>
<span data-ttu-id="039a5-175">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="039a5-175">If successful, this method returns a `201 Created` response code and a [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="039a5-176">Exemplo</span><span class="sxs-lookup"><span data-stu-id="039a5-176">Example</span></span>

### <a name="request"></a><span data-ttu-id="039a5-177">Solicitação</span><span class="sxs-lookup"><span data-stu-id="039a5-177">Request</span></span>
<span data-ttu-id="039a5-178">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="039a5-178">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="039a5-179">Resposta</span><span class="sxs-lookup"><span data-stu-id="039a5-179">Response</span></span>
<span data-ttu-id="039a5-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="039a5-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




