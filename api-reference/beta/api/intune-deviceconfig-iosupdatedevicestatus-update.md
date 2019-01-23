---
title: Atualizar iosUpdateDeviceStatus
description: Atualizar as propriedades de um objeto iosUpdateDeviceStatus.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: e501171c66b2bfc18f82376d382f026f39291e5a
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29419811"
---
# <a name="update-iosupdatedevicestatus"></a><span data-ttu-id="f9245-103">Atualizar iosUpdateDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="f9245-103">Update iosUpdateDeviceStatus</span></span>

> <span data-ttu-id="f9245-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="f9245-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="f9245-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="f9245-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f9245-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="f9245-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f9245-107">Atualizar as propriedades de um objeto [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="f9245-107">Update the properties of a [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f9245-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f9245-108">Prerequisites</span></span>
<span data-ttu-id="f9245-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="f9245-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="f9245-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f9245-111">Permission type</span></span>|<span data-ttu-id="f9245-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f9245-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f9245-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f9245-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f9245-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f9245-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f9245-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f9245-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f9245-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f9245-116">Not supported.</span></span>|
|<span data-ttu-id="f9245-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f9245-117">Application</span></span>|<span data-ttu-id="f9245-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f9245-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f9245-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f9245-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/iosUpdateStatuses/{iosUpdateDeviceStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="f9245-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f9245-120">Request headers</span></span>
|<span data-ttu-id="f9245-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f9245-121">Header</span></span>|<span data-ttu-id="f9245-122">Valor</span><span class="sxs-lookup"><span data-stu-id="f9245-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f9245-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="f9245-123">Authorization</span></span>|<span data-ttu-id="f9245-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f9245-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f9245-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f9245-125">Accept</span></span>|<span data-ttu-id="f9245-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f9245-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f9245-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f9245-127">Request body</span></span>
<span data-ttu-id="f9245-128">No corpo da solicitação, forneça uma representação JSON do objeto [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="f9245-128">In the request body, supply a JSON representation for the [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) object.</span></span>

<span data-ttu-id="f9245-129">A tabela a seguir mostra as propriedades obrigatórias ao criar [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="f9245-129">The following table shows the properties that are required when you create the [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md).</span></span>

|<span data-ttu-id="f9245-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f9245-130">Property</span></span>|<span data-ttu-id="f9245-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="f9245-131">Type</span></span>|<span data-ttu-id="f9245-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="f9245-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f9245-133">id</span><span class="sxs-lookup"><span data-stu-id="f9245-133">id</span></span>|<span data-ttu-id="f9245-134">String</span><span class="sxs-lookup"><span data-stu-id="f9245-134">String</span></span>|<span data-ttu-id="f9245-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="f9245-135">Key of the entity.</span></span>|
|<span data-ttu-id="f9245-136">installStatus</span><span class="sxs-lookup"><span data-stu-id="f9245-136">installStatus</span></span>|[<span data-ttu-id="f9245-137">iosUpdatesInstallStatus</span><span class="sxs-lookup"><span data-stu-id="f9245-137">iosUpdatesInstallStatus</span></span>](../resources/intune-deviceconfig-iosupdatesinstallstatus.md)|<span data-ttu-id="f9245-138">O status de instalação do relatório de políticas.</span><span class="sxs-lookup"><span data-stu-id="f9245-138">The installation status of the policy report.</span></span> <span data-ttu-id="f9245-139">Os valores possíveis são: `success`, `available`, `idle`, `unknown`, `downloading`, `downloadFailed`, `downloadRequiresComputer`, `downloadInsufficientSpace`, `downloadInsufficientPower`, `downloadInsufficientNetwork`, `installing`, `installInsufficientSpace`, `installInsufficientPower`, `installPhoneCallInProgress`, `installFailed`, `notSupportedOperation`, `sharedDeviceUserLoggedInError`.</span><span class="sxs-lookup"><span data-stu-id="f9245-139">Possible values are: `success`, `available`, `idle`, `unknown`, `downloading`, `downloadFailed`, `downloadRequiresComputer`, `downloadInsufficientSpace`, `downloadInsufficientPower`, `downloadInsufficientNetwork`, `installing`, `installInsufficientSpace`, `installInsufficientPower`, `installPhoneCallInProgress`, `installFailed`, `notSupportedOperation`, `sharedDeviceUserLoggedInError`.</span></span>|
|<span data-ttu-id="f9245-140">osVersion</span><span class="sxs-lookup"><span data-stu-id="f9245-140">osVersion</span></span>|<span data-ttu-id="f9245-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f9245-141">String</span></span>|<span data-ttu-id="f9245-142">A versão do dispositivo que está sendo relatado.</span><span class="sxs-lookup"><span data-stu-id="f9245-142">The device version that is being reported.</span></span>|
|<span data-ttu-id="f9245-143">deviceId</span><span class="sxs-lookup"><span data-stu-id="f9245-143">deviceId</span></span>|<span data-ttu-id="f9245-144">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f9245-144">String</span></span>|<span data-ttu-id="f9245-145">A ID do dispositivo que está sendo relatado.</span><span class="sxs-lookup"><span data-stu-id="f9245-145">The device id that is being reported.</span></span>|
|<span data-ttu-id="f9245-146">userId</span><span class="sxs-lookup"><span data-stu-id="f9245-146">userId</span></span>|<span data-ttu-id="f9245-147">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f9245-147">String</span></span>|<span data-ttu-id="f9245-148">A ID do usuário que está sendo relatado.</span><span class="sxs-lookup"><span data-stu-id="f9245-148">The User id that is being reported.</span></span>|
|<span data-ttu-id="f9245-149">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="f9245-149">deviceDisplayName</span></span>|<span data-ttu-id="f9245-150">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f9245-150">String</span></span>|<span data-ttu-id="f9245-151">Nome do dispositivo de DevicePolicyStatus.</span><span class="sxs-lookup"><span data-stu-id="f9245-151">Device name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="f9245-152">userName</span><span class="sxs-lookup"><span data-stu-id="f9245-152">userName</span></span>|<span data-ttu-id="f9245-153">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f9245-153">String</span></span>|<span data-ttu-id="f9245-154">O nome de usuário que está sendo relatado</span><span class="sxs-lookup"><span data-stu-id="f9245-154">The User Name that is being reported</span></span>|
|<span data-ttu-id="f9245-155">deviceModel</span><span class="sxs-lookup"><span data-stu-id="f9245-155">deviceModel</span></span>|<span data-ttu-id="f9245-156">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f9245-156">String</span></span>|<span data-ttu-id="f9245-157">O modelo do dispositivo que está sendo relatado</span><span class="sxs-lookup"><span data-stu-id="f9245-157">The device model that is being reported</span></span>|
|<span data-ttu-id="f9245-158">platform</span><span class="sxs-lookup"><span data-stu-id="f9245-158">platform</span></span>|<span data-ttu-id="f9245-159">Int32</span><span class="sxs-lookup"><span data-stu-id="f9245-159">Int32</span></span>|<span data-ttu-id="f9245-160">Plataforma do dispositivo que está sendo relatado</span><span class="sxs-lookup"><span data-stu-id="f9245-160">Platform of the device that is being reported</span></span>|
|<span data-ttu-id="f9245-161">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="f9245-161">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="f9245-162">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f9245-162">DateTimeOffset</span></span>|<span data-ttu-id="f9245-163">DateTime em que o período de cortesia de conformidade do dispositivo termina</span><span class="sxs-lookup"><span data-stu-id="f9245-163">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="f9245-164">status</span><span class="sxs-lookup"><span data-stu-id="f9245-164">status</span></span>|[<span data-ttu-id="f9245-165">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="f9245-165">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="f9245-166">Status de conformidade do relatório de políticas.</span><span class="sxs-lookup"><span data-stu-id="f9245-166">Compliance status of the policy report.</span></span> <span data-ttu-id="f9245-167">Os valores possíveis são: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="f9245-167">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="f9245-168">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="f9245-168">lastReportedDateTime</span></span>|<span data-ttu-id="f9245-169">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f9245-169">DateTimeOffset</span></span>|<span data-ttu-id="f9245-170">Data e hora da última modificação do relatório de políticas.</span><span class="sxs-lookup"><span data-stu-id="f9245-170">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="f9245-171">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="f9245-171">userPrincipalName</span></span>|<span data-ttu-id="f9245-172">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f9245-172">String</span></span>|<span data-ttu-id="f9245-173">UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="f9245-173">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="f9245-174">Resposta</span><span class="sxs-lookup"><span data-stu-id="f9245-174">Response</span></span>
<span data-ttu-id="f9245-175">Se for bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f9245-175">If successful, this method returns a `200 OK` response code and an updated [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f9245-176">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f9245-176">Example</span></span>

### <a name="request"></a><span data-ttu-id="f9245-177">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f9245-177">Request</span></span>
<span data-ttu-id="f9245-178">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f9245-178">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f9245-179">Resposta</span><span class="sxs-lookup"><span data-stu-id="f9245-179">Response</span></span>
<span data-ttu-id="f9245-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f9245-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




