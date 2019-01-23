---
title: Atualizar mobileAppInstallStatus
description: Atualize as propriedades de um objeto mobileAppInstallStatus.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: e28404181248cef1deae4bec2752de51f553373b
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29394541"
---
# <a name="update-mobileappinstallstatus"></a><span data-ttu-id="62a5a-103">Atualizar mobileAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="62a5a-103">Update mobileAppInstallStatus</span></span>

> <span data-ttu-id="62a5a-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="62a5a-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="62a5a-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="62a5a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="62a5a-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="62a5a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="62a5a-107">Atualize as propriedades de um objeto [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) .</span><span class="sxs-lookup"><span data-stu-id="62a5a-107">Update the properties of a [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="62a5a-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="62a5a-108">Prerequisites</span></span>
<span data-ttu-id="62a5a-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="62a5a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="62a5a-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="62a5a-111">Permission type</span></span>|<span data-ttu-id="62a5a-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="62a5a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="62a5a-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="62a5a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="62a5a-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="62a5a-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="62a5a-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="62a5a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="62a5a-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="62a5a-116">Not supported.</span></span>|
|<span data-ttu-id="62a5a-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="62a5a-117">Application</span></span>|<span data-ttu-id="62a5a-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="62a5a-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="62a5a-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="62a5a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/deviceStatuses/{mobileAppInstallStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="62a5a-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="62a5a-120">Request headers</span></span>
|<span data-ttu-id="62a5a-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="62a5a-121">Header</span></span>|<span data-ttu-id="62a5a-122">Valor</span><span class="sxs-lookup"><span data-stu-id="62a5a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="62a5a-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="62a5a-123">Authorization</span></span>|<span data-ttu-id="62a5a-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="62a5a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="62a5a-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="62a5a-125">Accept</span></span>|<span data-ttu-id="62a5a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="62a5a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="62a5a-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="62a5a-127">Request body</span></span>
<span data-ttu-id="62a5a-128">No corpo da solicitação, fornece uma representação JSON para o objeto [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) .</span><span class="sxs-lookup"><span data-stu-id="62a5a-128">In the request body, supply a JSON representation for the [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) object.</span></span>

<span data-ttu-id="62a5a-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md).</span><span class="sxs-lookup"><span data-stu-id="62a5a-129">The following table shows the properties that are required when you create the [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md).</span></span>

|<span data-ttu-id="62a5a-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="62a5a-130">Property</span></span>|<span data-ttu-id="62a5a-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="62a5a-131">Type</span></span>|<span data-ttu-id="62a5a-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="62a5a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="62a5a-133">id</span><span class="sxs-lookup"><span data-stu-id="62a5a-133">id</span></span>|<span data-ttu-id="62a5a-134">String</span><span class="sxs-lookup"><span data-stu-id="62a5a-134">String</span></span>|<span data-ttu-id="62a5a-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="62a5a-135">Key of the entity.</span></span>|
|<span data-ttu-id="62a5a-136">deviceName</span><span class="sxs-lookup"><span data-stu-id="62a5a-136">deviceName</span></span>|<span data-ttu-id="62a5a-137">String</span><span class="sxs-lookup"><span data-stu-id="62a5a-137">String</span></span>|<span data-ttu-id="62a5a-138">Nome do dispositivo</span><span class="sxs-lookup"><span data-stu-id="62a5a-138">Device name</span></span>|
|<span data-ttu-id="62a5a-139">deviceId</span><span class="sxs-lookup"><span data-stu-id="62a5a-139">deviceId</span></span>|<span data-ttu-id="62a5a-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="62a5a-140">String</span></span>|<span data-ttu-id="62a5a-141">ID do dispositivo</span><span class="sxs-lookup"><span data-stu-id="62a5a-141">Device ID</span></span>|
|<span data-ttu-id="62a5a-142">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="62a5a-142">lastSyncDateTime</span></span>|<span data-ttu-id="62a5a-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="62a5a-143">DateTimeOffset</span></span>|<span data-ttu-id="62a5a-144">Última sincronização data hora</span><span class="sxs-lookup"><span data-stu-id="62a5a-144">Last sync date time</span></span>|
|<span data-ttu-id="62a5a-145">mobileAppInstallStatusValue</span><span class="sxs-lookup"><span data-stu-id="62a5a-145">mobileAppInstallStatusValue</span></span>|[<span data-ttu-id="62a5a-146">resultantAppState</span><span class="sxs-lookup"><span data-stu-id="62a5a-146">resultantAppState</span></span>](../resources/intune-shared-resultantappstate.md)|<span data-ttu-id="62a5a-147">O estado de instalação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="62a5a-147">The install state of the app.</span></span> <span data-ttu-id="62a5a-148">Os valores possíveis são: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span><span class="sxs-lookup"><span data-stu-id="62a5a-148">Possible values are: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span></span>|
|<span data-ttu-id="62a5a-149">installState</span><span class="sxs-lookup"><span data-stu-id="62a5a-149">installState</span></span>|[<span data-ttu-id="62a5a-150">resultantAppState</span><span class="sxs-lookup"><span data-stu-id="62a5a-150">resultantAppState</span></span>](../resources/intune-shared-resultantappstate.md)|<span data-ttu-id="62a5a-151">O estado de instalação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="62a5a-151">The install state of the app.</span></span> <span data-ttu-id="62a5a-152">Os valores possíveis são: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span><span class="sxs-lookup"><span data-stu-id="62a5a-152">Possible values are: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span></span>|
|<span data-ttu-id="62a5a-153">installStateDetail</span><span class="sxs-lookup"><span data-stu-id="62a5a-153">installStateDetail</span></span>|[<span data-ttu-id="62a5a-154">resultantAppStateDetail</span><span class="sxs-lookup"><span data-stu-id="62a5a-154">resultantAppStateDetail</span></span>](../resources/intune-apps-resultantappstatedetail.md)|<span data-ttu-id="62a5a-155">Os detalhes de estado de instalação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="62a5a-155">The install state detail of the app.</span></span> <span data-ttu-id="62a5a-156">Os valores possíveis são: `noAdditionalDetails`, `seeInstallErrorCode`, `seeUninstallErrorCode`, `pendingReboot`, `platformNotApplicable`, `minimumCpuSpeedNotMet`, `minimumLogicalProcessorCountNotMet`, `minimumPhysicalMemoryNotMet`, `minimumOsVersionNotMet`, `minimumDiskSpaceNotMet`, `processorArchitectureNotApplicable`.</span><span class="sxs-lookup"><span data-stu-id="62a5a-156">Possible values are: `noAdditionalDetails`, `seeInstallErrorCode`, `seeUninstallErrorCode`, `pendingReboot`, `platformNotApplicable`, `minimumCpuSpeedNotMet`, `minimumLogicalProcessorCountNotMet`, `minimumPhysicalMemoryNotMet`, `minimumOsVersionNotMet`, `minimumDiskSpaceNotMet`, `processorArchitectureNotApplicable`.</span></span>|
|<span data-ttu-id="62a5a-157">errorCode</span><span class="sxs-lookup"><span data-stu-id="62a5a-157">errorCode</span></span>|<span data-ttu-id="62a5a-158">Int32</span><span class="sxs-lookup"><span data-stu-id="62a5a-158">Int32</span></span>|<span data-ttu-id="62a5a-159">O erro de código para instalar ou desinstalar falhas.</span><span class="sxs-lookup"><span data-stu-id="62a5a-159">The error code for install or uninstall failures.</span></span>|
|<span data-ttu-id="62a5a-160">osVersion</span><span class="sxs-lookup"><span data-stu-id="62a5a-160">osVersion</span></span>|<span data-ttu-id="62a5a-161">String</span><span class="sxs-lookup"><span data-stu-id="62a5a-161">String</span></span>|<span data-ttu-id="62a5a-162">Versão do sistema operacional</span><span class="sxs-lookup"><span data-stu-id="62a5a-162">OS Version</span></span>|
|<span data-ttu-id="62a5a-163">osDescription</span><span class="sxs-lookup"><span data-stu-id="62a5a-163">osDescription</span></span>|<span data-ttu-id="62a5a-164">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="62a5a-164">String</span></span>|<span data-ttu-id="62a5a-165">Descrição do sistema operacional</span><span class="sxs-lookup"><span data-stu-id="62a5a-165">OS Description</span></span>|
|<span data-ttu-id="62a5a-166">userName</span><span class="sxs-lookup"><span data-stu-id="62a5a-166">userName</span></span>|<span data-ttu-id="62a5a-167">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="62a5a-167">String</span></span>|<span data-ttu-id="62a5a-168">Nome de usuário do dispositivo</span><span class="sxs-lookup"><span data-stu-id="62a5a-168">Device User Name</span></span>|
|<span data-ttu-id="62a5a-169">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="62a5a-169">userPrincipalName</span></span>|<span data-ttu-id="62a5a-170">String</span><span class="sxs-lookup"><span data-stu-id="62a5a-170">String</span></span>|<span data-ttu-id="62a5a-171">Nome UPN</span><span class="sxs-lookup"><span data-stu-id="62a5a-171">User Principal Name</span></span>|
|<span data-ttu-id="62a5a-172">displayVersion</span><span class="sxs-lookup"><span data-stu-id="62a5a-172">displayVersion</span></span>|<span data-ttu-id="62a5a-173">String</span><span class="sxs-lookup"><span data-stu-id="62a5a-173">String</span></span>|<span data-ttu-id="62a5a-174">Versão legível humana do aplicativo</span><span class="sxs-lookup"><span data-stu-id="62a5a-174">Human readable version of the application</span></span>|



## <a name="response"></a><span data-ttu-id="62a5a-175">Resposta</span><span class="sxs-lookup"><span data-stu-id="62a5a-175">Response</span></span>
<span data-ttu-id="62a5a-176">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto atualizado [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="62a5a-176">If successful, this method returns a `200 OK` response code and an updated [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="62a5a-177">Exemplo</span><span class="sxs-lookup"><span data-stu-id="62a5a-177">Example</span></span>

### <a name="request"></a><span data-ttu-id="62a5a-178">Solicitação</span><span class="sxs-lookup"><span data-stu-id="62a5a-178">Request</span></span>
<span data-ttu-id="62a5a-179">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="62a5a-179">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}
Content-type: application/json
Content-length: 549

{
  "@odata.type": "#microsoft.graph.mobileAppInstallStatus",
  "deviceName": "Device Name value",
  "deviceId": "Device Id value",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "mobileAppInstallStatusValue": "failed",
  "installState": "failed",
  "installStateDetail": "seeInstallErrorCode",
  "errorCode": 9,
  "osVersion": "Os Version value",
  "osDescription": "Os Description value",
  "userName": "User Name value",
  "userPrincipalName": "User Principal Name value",
  "displayVersion": "Display Version value"
}
```

### <a name="response"></a><span data-ttu-id="62a5a-180">Resposta</span><span class="sxs-lookup"><span data-stu-id="62a5a-180">Response</span></span>
<span data-ttu-id="62a5a-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="62a5a-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 598

{
  "@odata.type": "#microsoft.graph.mobileAppInstallStatus",
  "id": "7560ee45-ee45-7560-45ee-607545ee6075",
  "deviceName": "Device Name value",
  "deviceId": "Device Id value",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "mobileAppInstallStatusValue": "failed",
  "installState": "failed",
  "installStateDetail": "seeInstallErrorCode",
  "errorCode": 9,
  "osVersion": "Os Version value",
  "osDescription": "Os Description value",
  "userName": "User Name value",
  "userPrincipalName": "User Principal Name value",
  "displayVersion": "Display Version value"
}
```




