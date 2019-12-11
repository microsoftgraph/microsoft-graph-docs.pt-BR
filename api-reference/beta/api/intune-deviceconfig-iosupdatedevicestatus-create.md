---
title: Criar iosUpdateDeviceStatus
description: Criar um novo objeto iosUpdateDeviceStatus.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 484b7155feed87a36e717177555c2512acf285ff
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39948645"
---
# <a name="create-iosupdatedevicestatus"></a><span data-ttu-id="fa742-103">Criar iosUpdateDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="fa742-103">Create iosUpdateDeviceStatus</span></span>

> <span data-ttu-id="fa742-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="fa742-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fa742-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="fa742-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fa742-106">Criar um novo objeto [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="fa742-106">Create a new [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fa742-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="fa742-107">Prerequisites</span></span>
<span data-ttu-id="fa742-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fa742-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fa742-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fa742-110">Permission type</span></span>|<span data-ttu-id="fa742-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="fa742-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fa742-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fa742-112">Delegated (work or school account)</span></span>|<span data-ttu-id="fa742-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fa742-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="fa742-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fa742-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fa742-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fa742-115">Not supported.</span></span>|
|<span data-ttu-id="fa742-116">Application</span><span class="sxs-lookup"><span data-stu-id="fa742-116">Application</span></span>|<span data-ttu-id="fa742-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fa742-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="fa742-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fa742-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/iosUpdateStatuses
```

## <a name="request-headers"></a><span data-ttu-id="fa742-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fa742-119">Request headers</span></span>
|<span data-ttu-id="fa742-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="fa742-120">Header</span></span>|<span data-ttu-id="fa742-121">Valor</span><span class="sxs-lookup"><span data-stu-id="fa742-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fa742-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="fa742-122">Authorization</span></span>|<span data-ttu-id="fa742-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fa742-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fa742-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="fa742-124">Accept</span></span>|<span data-ttu-id="fa742-125">application/json</span><span class="sxs-lookup"><span data-stu-id="fa742-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fa742-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fa742-126">Request body</span></span>
<span data-ttu-id="fa742-127">No corpo da solicitação, forneça uma representação JSON do objeto iosUpdateDeviceStatus.</span><span class="sxs-lookup"><span data-stu-id="fa742-127">In the request body, supply a JSON representation for the iosUpdateDeviceStatus object.</span></span>

<span data-ttu-id="fa742-128">A tabela a seguir mostra as propriedades que são necessárias ao criar iosUpdateDeviceStatus.</span><span class="sxs-lookup"><span data-stu-id="fa742-128">The following table shows the properties that are required when you create the iosUpdateDeviceStatus.</span></span>

|<span data-ttu-id="fa742-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fa742-129">Property</span></span>|<span data-ttu-id="fa742-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="fa742-130">Type</span></span>|<span data-ttu-id="fa742-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="fa742-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fa742-132">id</span><span class="sxs-lookup"><span data-stu-id="fa742-132">id</span></span>|<span data-ttu-id="fa742-133">String</span><span class="sxs-lookup"><span data-stu-id="fa742-133">String</span></span>|<span data-ttu-id="fa742-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="fa742-134">Key of the entity.</span></span>|
|<span data-ttu-id="fa742-135">installStatus</span><span class="sxs-lookup"><span data-stu-id="fa742-135">installStatus</span></span>|[<span data-ttu-id="fa742-136">iosUpdatesInstallStatus</span><span class="sxs-lookup"><span data-stu-id="fa742-136">iosUpdatesInstallStatus</span></span>](../resources/intune-deviceconfig-iosupdatesinstallstatus.md)|<span data-ttu-id="fa742-137">O status de instalação do relatório de políticas.</span><span class="sxs-lookup"><span data-stu-id="fa742-137">The installation status of the policy report.</span></span> <span data-ttu-id="fa742-138">Os valores possíveis são `success`: `available`, `idle`, `unknown`, `downloading`, `downloadFailed`, `downloadRequiresComputer`, `downloadInsufficientSpace`, `downloadInsufficientPower`, `downloadInsufficientNetwork`, `installing`, `installInsufficientSpace`, `installInsufficientPower`, `installPhoneCallInProgress`, `installFailed`, `notSupportedOperation`, `sharedDeviceUserLoggedInError`,,,,,,,,,.</span><span class="sxs-lookup"><span data-stu-id="fa742-138">Possible values are: `success`, `available`, `idle`, `unknown`, `downloading`, `downloadFailed`, `downloadRequiresComputer`, `downloadInsufficientSpace`, `downloadInsufficientPower`, `downloadInsufficientNetwork`, `installing`, `installInsufficientSpace`, `installInsufficientPower`, `installPhoneCallInProgress`, `installFailed`, `notSupportedOperation`, `sharedDeviceUserLoggedInError`.</span></span>|
|<span data-ttu-id="fa742-139">osVersion</span><span class="sxs-lookup"><span data-stu-id="fa742-139">osVersion</span></span>|<span data-ttu-id="fa742-140">String</span><span class="sxs-lookup"><span data-stu-id="fa742-140">String</span></span>|<span data-ttu-id="fa742-141">A versão do dispositivo que está sendo relatado.</span><span class="sxs-lookup"><span data-stu-id="fa742-141">The device version that is being reported.</span></span>|
|<span data-ttu-id="fa742-142">deviceId</span><span class="sxs-lookup"><span data-stu-id="fa742-142">deviceId</span></span>|<span data-ttu-id="fa742-143">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="fa742-143">String</span></span>|<span data-ttu-id="fa742-144">A ID do dispositivo que está sendo relatado.</span><span class="sxs-lookup"><span data-stu-id="fa742-144">The device id that is being reported.</span></span>|
|<span data-ttu-id="fa742-145">userId</span><span class="sxs-lookup"><span data-stu-id="fa742-145">userId</span></span>|<span data-ttu-id="fa742-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fa742-146">String</span></span>|<span data-ttu-id="fa742-147">A ID do usuário que está sendo relatado.</span><span class="sxs-lookup"><span data-stu-id="fa742-147">The User id that is being reported.</span></span>|
|<span data-ttu-id="fa742-148">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="fa742-148">deviceDisplayName</span></span>|<span data-ttu-id="fa742-149">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="fa742-149">String</span></span>|<span data-ttu-id="fa742-150">Nome do dispositivo de DevicePolicyStatus.</span><span class="sxs-lookup"><span data-stu-id="fa742-150">Device name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="fa742-151">userName</span><span class="sxs-lookup"><span data-stu-id="fa742-151">userName</span></span>|<span data-ttu-id="fa742-152">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="fa742-152">String</span></span>|<span data-ttu-id="fa742-153">O nome de usuário que está sendo relatado</span><span class="sxs-lookup"><span data-stu-id="fa742-153">The User Name that is being reported</span></span>|
|<span data-ttu-id="fa742-154">deviceModel</span><span class="sxs-lookup"><span data-stu-id="fa742-154">deviceModel</span></span>|<span data-ttu-id="fa742-155">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fa742-155">String</span></span>|<span data-ttu-id="fa742-156">O modelo do dispositivo que está sendo relatado</span><span class="sxs-lookup"><span data-stu-id="fa742-156">The device model that is being reported</span></span>|
|<span data-ttu-id="fa742-157">platform</span><span class="sxs-lookup"><span data-stu-id="fa742-157">platform</span></span>|<span data-ttu-id="fa742-158">Int32</span><span class="sxs-lookup"><span data-stu-id="fa742-158">Int32</span></span>|<span data-ttu-id="fa742-159">Plataforma do dispositivo que está sendo relatado</span><span class="sxs-lookup"><span data-stu-id="fa742-159">Platform of the device that is being reported</span></span>|
|<span data-ttu-id="fa742-160">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="fa742-160">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="fa742-161">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fa742-161">DateTimeOffset</span></span>|<span data-ttu-id="fa742-162">DateTime em que o período de cortesia de conformidade do dispositivo termina</span><span class="sxs-lookup"><span data-stu-id="fa742-162">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="fa742-163">status</span><span class="sxs-lookup"><span data-stu-id="fa742-163">status</span></span>|[<span data-ttu-id="fa742-164">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="fa742-164">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="fa742-165">Status de conformidade do relatório de políticas.</span><span class="sxs-lookup"><span data-stu-id="fa742-165">Compliance status of the policy report.</span></span> <span data-ttu-id="fa742-166">Os valores possíveis são: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="fa742-166">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="fa742-167">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="fa742-167">lastReportedDateTime</span></span>|<span data-ttu-id="fa742-168">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fa742-168">DateTimeOffset</span></span>|<span data-ttu-id="fa742-169">Data e hora da última modificação do relatório de políticas.</span><span class="sxs-lookup"><span data-stu-id="fa742-169">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="fa742-170">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="fa742-170">userPrincipalName</span></span>|<span data-ttu-id="fa742-171">String</span><span class="sxs-lookup"><span data-stu-id="fa742-171">String</span></span>|<span data-ttu-id="fa742-172">UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="fa742-172">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="fa742-173">Resposta</span><span class="sxs-lookup"><span data-stu-id="fa742-173">Response</span></span>
<span data-ttu-id="fa742-174">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fa742-174">If successful, this method returns a `201 Created` response code and a [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fa742-175">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fa742-175">Example</span></span>

### <a name="request"></a><span data-ttu-id="fa742-176">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fa742-176">Request</span></span>
<span data-ttu-id="fa742-177">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fa742-177">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="fa742-178">Resposta</span><span class="sxs-lookup"><span data-stu-id="fa742-178">Response</span></span>
<span data-ttu-id="fa742-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fa742-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





