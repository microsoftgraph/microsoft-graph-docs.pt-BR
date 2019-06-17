---
title: Criar iosUpdateDeviceStatus
description: Criar um novo objeto iosUpdateDeviceStatus.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3bfed8ec9b24353c475b229c4dba92d469691434
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34977174"
---
# <a name="create-iosupdatedevicestatus"></a><span data-ttu-id="67aff-103">Criar iosUpdateDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="67aff-103">Create iosUpdateDeviceStatus</span></span>

> <span data-ttu-id="67aff-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="67aff-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="67aff-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="67aff-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="67aff-106">Criar um novo objeto [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="67aff-106">Create a new [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="67aff-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="67aff-107">Prerequisites</span></span>
<span data-ttu-id="67aff-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="67aff-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="67aff-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="67aff-110">Permission type</span></span>|<span data-ttu-id="67aff-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="67aff-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="67aff-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="67aff-112">Delegated (work or school account)</span></span>|<span data-ttu-id="67aff-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="67aff-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="67aff-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="67aff-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="67aff-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="67aff-115">Not supported.</span></span>|
|<span data-ttu-id="67aff-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="67aff-116">Application</span></span>|<span data-ttu-id="67aff-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="67aff-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="67aff-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="67aff-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/iosUpdateStatuses
```

## <a name="request-headers"></a><span data-ttu-id="67aff-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="67aff-119">Request headers</span></span>
|<span data-ttu-id="67aff-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="67aff-120">Header</span></span>|<span data-ttu-id="67aff-121">Valor</span><span class="sxs-lookup"><span data-stu-id="67aff-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="67aff-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="67aff-122">Authorization</span></span>|<span data-ttu-id="67aff-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="67aff-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="67aff-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="67aff-124">Accept</span></span>|<span data-ttu-id="67aff-125">application/json</span><span class="sxs-lookup"><span data-stu-id="67aff-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="67aff-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="67aff-126">Request body</span></span>
<span data-ttu-id="67aff-127">No corpo da solicitação, forneça uma representação JSON do objeto iosUpdateDeviceStatus.</span><span class="sxs-lookup"><span data-stu-id="67aff-127">In the request body, supply a JSON representation for the iosUpdateDeviceStatus object.</span></span>

<span data-ttu-id="67aff-128">A tabela a seguir mostra as propriedades que são necessárias ao criar iosUpdateDeviceStatus.</span><span class="sxs-lookup"><span data-stu-id="67aff-128">The following table shows the properties that are required when you create the iosUpdateDeviceStatus.</span></span>

|<span data-ttu-id="67aff-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="67aff-129">Property</span></span>|<span data-ttu-id="67aff-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="67aff-130">Type</span></span>|<span data-ttu-id="67aff-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="67aff-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="67aff-132">id</span><span class="sxs-lookup"><span data-stu-id="67aff-132">id</span></span>|<span data-ttu-id="67aff-133">String</span><span class="sxs-lookup"><span data-stu-id="67aff-133">String</span></span>|<span data-ttu-id="67aff-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="67aff-134">Key of the entity.</span></span>|
|<span data-ttu-id="67aff-135">installStatus</span><span class="sxs-lookup"><span data-stu-id="67aff-135">installStatus</span></span>|[<span data-ttu-id="67aff-136">iosUpdatesInstallStatus</span><span class="sxs-lookup"><span data-stu-id="67aff-136">iosUpdatesInstallStatus</span></span>](../resources/intune-deviceconfig-iosupdatesinstallstatus.md)|<span data-ttu-id="67aff-137">O status de instalação do relatório de políticas.</span><span class="sxs-lookup"><span data-stu-id="67aff-137">The installation status of the policy report.</span></span> <span data-ttu-id="67aff-138">Os valores possíveis são `success`: `available`, `idle`, `unknown`, `downloading`, `downloadFailed`, `downloadRequiresComputer`, `downloadInsufficientSpace`, `downloadInsufficientPower`, `downloadInsufficientNetwork`, `installing`, `installInsufficientSpace`, `installInsufficientPower`, `installPhoneCallInProgress`, `installFailed`, `notSupportedOperation`, `sharedDeviceUserLoggedInError`,,,,,,,,,.</span><span class="sxs-lookup"><span data-stu-id="67aff-138">Possible values are: `success`, `available`, `idle`, `unknown`, `downloading`, `downloadFailed`, `downloadRequiresComputer`, `downloadInsufficientSpace`, `downloadInsufficientPower`, `downloadInsufficientNetwork`, `installing`, `installInsufficientSpace`, `installInsufficientPower`, `installPhoneCallInProgress`, `installFailed`, `notSupportedOperation`, `sharedDeviceUserLoggedInError`.</span></span>|
|<span data-ttu-id="67aff-139">osVersion</span><span class="sxs-lookup"><span data-stu-id="67aff-139">osVersion</span></span>|<span data-ttu-id="67aff-140">String</span><span class="sxs-lookup"><span data-stu-id="67aff-140">String</span></span>|<span data-ttu-id="67aff-141">A versão do dispositivo que está sendo relatado.</span><span class="sxs-lookup"><span data-stu-id="67aff-141">The device version that is being reported.</span></span>|
|<span data-ttu-id="67aff-142">deviceId</span><span class="sxs-lookup"><span data-stu-id="67aff-142">deviceId</span></span>|<span data-ttu-id="67aff-143">String</span><span class="sxs-lookup"><span data-stu-id="67aff-143">String</span></span>|<span data-ttu-id="67aff-144">A ID do dispositivo que está sendo relatado.</span><span class="sxs-lookup"><span data-stu-id="67aff-144">The device id that is being reported.</span></span>|
|<span data-ttu-id="67aff-145">userId</span><span class="sxs-lookup"><span data-stu-id="67aff-145">userId</span></span>|<span data-ttu-id="67aff-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="67aff-146">String</span></span>|<span data-ttu-id="67aff-147">A ID do usuário que está sendo relatado.</span><span class="sxs-lookup"><span data-stu-id="67aff-147">The User id that is being reported.</span></span>|
|<span data-ttu-id="67aff-148">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="67aff-148">deviceDisplayName</span></span>|<span data-ttu-id="67aff-149">String</span><span class="sxs-lookup"><span data-stu-id="67aff-149">String</span></span>|<span data-ttu-id="67aff-150">Nome do dispositivo de DevicePolicyStatus.</span><span class="sxs-lookup"><span data-stu-id="67aff-150">Device name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="67aff-151">userName</span><span class="sxs-lookup"><span data-stu-id="67aff-151">userName</span></span>|<span data-ttu-id="67aff-152">String</span><span class="sxs-lookup"><span data-stu-id="67aff-152">String</span></span>|<span data-ttu-id="67aff-153">O nome de usuário que está sendo relatado</span><span class="sxs-lookup"><span data-stu-id="67aff-153">The User Name that is being reported</span></span>|
|<span data-ttu-id="67aff-154">deviceModel</span><span class="sxs-lookup"><span data-stu-id="67aff-154">deviceModel</span></span>|<span data-ttu-id="67aff-155">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="67aff-155">String</span></span>|<span data-ttu-id="67aff-156">O modelo do dispositivo que está sendo relatado</span><span class="sxs-lookup"><span data-stu-id="67aff-156">The device model that is being reported</span></span>|
|<span data-ttu-id="67aff-157">platform</span><span class="sxs-lookup"><span data-stu-id="67aff-157">platform</span></span>|<span data-ttu-id="67aff-158">Int32</span><span class="sxs-lookup"><span data-stu-id="67aff-158">Int32</span></span>|<span data-ttu-id="67aff-159">Plataforma do dispositivo que está sendo relatado</span><span class="sxs-lookup"><span data-stu-id="67aff-159">Platform of the device that is being reported</span></span>|
|<span data-ttu-id="67aff-160">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="67aff-160">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="67aff-161">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="67aff-161">DateTimeOffset</span></span>|<span data-ttu-id="67aff-162">DateTime em que o período de cortesia de conformidade do dispositivo termina</span><span class="sxs-lookup"><span data-stu-id="67aff-162">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="67aff-163">status</span><span class="sxs-lookup"><span data-stu-id="67aff-163">status</span></span>|[<span data-ttu-id="67aff-164">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="67aff-164">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="67aff-165">Status de conformidade do relatório de políticas.</span><span class="sxs-lookup"><span data-stu-id="67aff-165">Compliance status of the policy report.</span></span> <span data-ttu-id="67aff-166">Os valores possíveis são: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="67aff-166">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="67aff-167">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="67aff-167">lastReportedDateTime</span></span>|<span data-ttu-id="67aff-168">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="67aff-168">DateTimeOffset</span></span>|<span data-ttu-id="67aff-169">Data e hora da última modificação do relatório de políticas.</span><span class="sxs-lookup"><span data-stu-id="67aff-169">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="67aff-170">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="67aff-170">userPrincipalName</span></span>|<span data-ttu-id="67aff-171">String</span><span class="sxs-lookup"><span data-stu-id="67aff-171">String</span></span>|<span data-ttu-id="67aff-172">UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="67aff-172">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="67aff-173">Resposta</span><span class="sxs-lookup"><span data-stu-id="67aff-173">Response</span></span>
<span data-ttu-id="67aff-174">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="67aff-174">If successful, this method returns a `201 Created` response code and a [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="67aff-175">Exemplo</span><span class="sxs-lookup"><span data-stu-id="67aff-175">Example</span></span>

### <a name="request"></a><span data-ttu-id="67aff-176">Solicitação</span><span class="sxs-lookup"><span data-stu-id="67aff-176">Request</span></span>
<span data-ttu-id="67aff-177">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="67aff-177">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="67aff-178">Resposta</span><span class="sxs-lookup"><span data-stu-id="67aff-178">Response</span></span>
<span data-ttu-id="67aff-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="67aff-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





