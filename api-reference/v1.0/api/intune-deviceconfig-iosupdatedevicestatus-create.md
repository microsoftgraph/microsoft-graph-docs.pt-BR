---
title: Criar iosUpdateDeviceStatus
description: Criar um novo objeto iosUpdateDeviceStatus.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e24e1127be43344e9ec66de8acf3fe6b2ebcd55b
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52758320"
---
# <a name="create-iosupdatedevicestatus"></a><span data-ttu-id="f4672-103">Criar iosUpdateDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="f4672-103">Create iosUpdateDeviceStatus</span></span>

<span data-ttu-id="f4672-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f4672-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f4672-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f4672-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f4672-106">Criar um novo objeto [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="f4672-106">Create a new [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f4672-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f4672-107">Prerequisites</span></span>
<span data-ttu-id="f4672-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f4672-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f4672-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f4672-110">Permission type</span></span>|<span data-ttu-id="f4672-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f4672-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f4672-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f4672-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f4672-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f4672-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f4672-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f4672-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f4672-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f4672-115">Not supported.</span></span>|
|<span data-ttu-id="f4672-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f4672-116">Application</span></span>|<span data-ttu-id="f4672-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f4672-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f4672-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f4672-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/iosUpdateStatuses
```

## <a name="request-headers"></a><span data-ttu-id="f4672-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f4672-119">Request headers</span></span>
|<span data-ttu-id="f4672-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f4672-120">Header</span></span>|<span data-ttu-id="f4672-121">Valor</span><span class="sxs-lookup"><span data-stu-id="f4672-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f4672-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="f4672-122">Authorization</span></span>|<span data-ttu-id="f4672-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f4672-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f4672-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f4672-124">Accept</span></span>|<span data-ttu-id="f4672-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f4672-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f4672-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f4672-126">Request body</span></span>
<span data-ttu-id="f4672-127">No corpo da solicitação, forneça uma representação JSON do objeto iosUpdateDeviceStatus.</span><span class="sxs-lookup"><span data-stu-id="f4672-127">In the request body, supply a JSON representation for the iosUpdateDeviceStatus object.</span></span>

<span data-ttu-id="f4672-128">A tabela a seguir mostra as propriedades que são necessárias ao criar iosUpdateDeviceStatus.</span><span class="sxs-lookup"><span data-stu-id="f4672-128">The following table shows the properties that are required when you create the iosUpdateDeviceStatus.</span></span>

|<span data-ttu-id="f4672-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f4672-129">Property</span></span>|<span data-ttu-id="f4672-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="f4672-130">Type</span></span>|<span data-ttu-id="f4672-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="f4672-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f4672-132">id</span><span class="sxs-lookup"><span data-stu-id="f4672-132">id</span></span>|<span data-ttu-id="f4672-133">String</span><span class="sxs-lookup"><span data-stu-id="f4672-133">String</span></span>|<span data-ttu-id="f4672-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="f4672-134">Key of the entity.</span></span>|
|<span data-ttu-id="f4672-135">installStatus</span><span class="sxs-lookup"><span data-stu-id="f4672-135">installStatus</span></span>|[<span data-ttu-id="f4672-136">iosUpdatesInstallStatus</span><span class="sxs-lookup"><span data-stu-id="f4672-136">iosUpdatesInstallStatus</span></span>](../resources/intune-deviceconfig-iosupdatesinstallstatus.md)|<span data-ttu-id="f4672-137">O status de instalação do relatório de políticas.</span><span class="sxs-lookup"><span data-stu-id="f4672-137">The installation status of the policy report.</span></span> <span data-ttu-id="f4672-138">Os valores possíveis são: `success` , , , , , , , , `available` , , , `idle` , , `unknown` , , , `downloading` , , `downloadFailed` `downloadRequiresComputer` , `downloadInsufficientSpace` `downloadInsufficientPower` `downloadInsufficientNetwork` `installing` `installInsufficientSpace` `installInsufficientPower` `installPhoneCallInProgress` `installFailed` `notSupportedOperation` . `sharedDeviceUserLoggedInError` `deviceOsHigherThanDesiredOsVersion`</span><span class="sxs-lookup"><span data-stu-id="f4672-138">Possible values are: `success`, `available`, `idle`, `unknown`, `downloading`, `downloadFailed`, `downloadRequiresComputer`, `downloadInsufficientSpace`, `downloadInsufficientPower`, `downloadInsufficientNetwork`, `installing`, `installInsufficientSpace`, `installInsufficientPower`, `installPhoneCallInProgress`, `installFailed`, `notSupportedOperation`, `sharedDeviceUserLoggedInError`, `deviceOsHigherThanDesiredOsVersion`.</span></span>|
|<span data-ttu-id="f4672-139">osVersion</span><span class="sxs-lookup"><span data-stu-id="f4672-139">osVersion</span></span>|<span data-ttu-id="f4672-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f4672-140">String</span></span>|<span data-ttu-id="f4672-141">A versão do dispositivo que está sendo relatado.</span><span class="sxs-lookup"><span data-stu-id="f4672-141">The device version that is being reported.</span></span>|
|<span data-ttu-id="f4672-142">deviceId</span><span class="sxs-lookup"><span data-stu-id="f4672-142">deviceId</span></span>|<span data-ttu-id="f4672-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f4672-143">String</span></span>|<span data-ttu-id="f4672-144">A ID do dispositivo que está sendo relatado.</span><span class="sxs-lookup"><span data-stu-id="f4672-144">The device id that is being reported.</span></span>|
|<span data-ttu-id="f4672-145">userId</span><span class="sxs-lookup"><span data-stu-id="f4672-145">userId</span></span>|<span data-ttu-id="f4672-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f4672-146">String</span></span>|<span data-ttu-id="f4672-147">A ID do usuário que está sendo relatado.</span><span class="sxs-lookup"><span data-stu-id="f4672-147">The User id that is being reported.</span></span>|
|<span data-ttu-id="f4672-148">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="f4672-148">deviceDisplayName</span></span>|<span data-ttu-id="f4672-149">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f4672-149">String</span></span>|<span data-ttu-id="f4672-150">Nome do dispositivo de DevicePolicyStatus.</span><span class="sxs-lookup"><span data-stu-id="f4672-150">Device name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="f4672-151">userName</span><span class="sxs-lookup"><span data-stu-id="f4672-151">userName</span></span>|<span data-ttu-id="f4672-152">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f4672-152">String</span></span>|<span data-ttu-id="f4672-153">O nome de usuário que está sendo relatado</span><span class="sxs-lookup"><span data-stu-id="f4672-153">The User Name that is being reported</span></span>|
|<span data-ttu-id="f4672-154">deviceModel</span><span class="sxs-lookup"><span data-stu-id="f4672-154">deviceModel</span></span>|<span data-ttu-id="f4672-155">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f4672-155">String</span></span>|<span data-ttu-id="f4672-156">O modelo do dispositivo que está sendo relatado</span><span class="sxs-lookup"><span data-stu-id="f4672-156">The device model that is being reported</span></span>|
|<span data-ttu-id="f4672-157">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="f4672-157">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="f4672-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f4672-158">DateTimeOffset</span></span>|<span data-ttu-id="f4672-159">DateTime em que o período de cortesia de conformidade do dispositivo termina</span><span class="sxs-lookup"><span data-stu-id="f4672-159">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="f4672-160">status</span><span class="sxs-lookup"><span data-stu-id="f4672-160">status</span></span>|[<span data-ttu-id="f4672-161">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="f4672-161">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="f4672-162">Status de conformidade do relatório de políticas.</span><span class="sxs-lookup"><span data-stu-id="f4672-162">Compliance status of the policy report.</span></span> <span data-ttu-id="f4672-163">Os valores possíveis são: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="f4672-163">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="f4672-164">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="f4672-164">lastReportedDateTime</span></span>|<span data-ttu-id="f4672-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f4672-165">DateTimeOffset</span></span>|<span data-ttu-id="f4672-166">Data e hora da última modificação do relatório de políticas.</span><span class="sxs-lookup"><span data-stu-id="f4672-166">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="f4672-167">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="f4672-167">userPrincipalName</span></span>|<span data-ttu-id="f4672-168">String</span><span class="sxs-lookup"><span data-stu-id="f4672-168">String</span></span>|<span data-ttu-id="f4672-169">UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="f4672-169">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="f4672-170">Resposta</span><span class="sxs-lookup"><span data-stu-id="f4672-170">Response</span></span>
<span data-ttu-id="f4672-171">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f4672-171">If successful, this method returns a `201 Created` response code and a [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f4672-172">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f4672-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="f4672-173">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f4672-173">Request</span></span>
<span data-ttu-id="f4672-174">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f4672-174">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f4672-175">Resposta</span><span class="sxs-lookup"><span data-stu-id="f4672-175">Response</span></span>
<span data-ttu-id="f4672-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f4672-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




