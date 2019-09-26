---
title: Atualizar mobileAppInstallStatus
description: Atualiza as propriedades de um objeto mobileAppInstallStatus.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 91203a42503505dc72335e11b47112bb4cc19ba4
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37172545"
---
# <a name="update-mobileappinstallstatus"></a><span data-ttu-id="42c73-103">Atualizar mobileAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="42c73-103">Update mobileAppInstallStatus</span></span>

> <span data-ttu-id="42c73-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="42c73-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="42c73-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="42c73-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="42c73-106">Atualiza as propriedades de um objeto [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) .</span><span class="sxs-lookup"><span data-stu-id="42c73-106">Update the properties of a [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="42c73-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="42c73-107">Prerequisites</span></span>
<span data-ttu-id="42c73-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="42c73-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="42c73-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="42c73-110">Permission type</span></span>|<span data-ttu-id="42c73-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="42c73-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="42c73-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="42c73-112">Delegated (work or school account)</span></span>|<span data-ttu-id="42c73-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="42c73-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="42c73-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="42c73-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="42c73-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="42c73-115">Not supported.</span></span>|
|<span data-ttu-id="42c73-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="42c73-116">Application</span></span>|<span data-ttu-id="42c73-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="42c73-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="42c73-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="42c73-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/deviceStatuses/{mobileAppInstallStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="42c73-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="42c73-119">Request headers</span></span>
|<span data-ttu-id="42c73-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="42c73-120">Header</span></span>|<span data-ttu-id="42c73-121">Valor</span><span class="sxs-lookup"><span data-stu-id="42c73-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="42c73-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="42c73-122">Authorization</span></span>|<span data-ttu-id="42c73-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="42c73-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="42c73-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="42c73-124">Accept</span></span>|<span data-ttu-id="42c73-125">application/json</span><span class="sxs-lookup"><span data-stu-id="42c73-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="42c73-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="42c73-126">Request body</span></span>
<span data-ttu-id="42c73-127">No corpo da solicitação, forneça uma representação JSON do objeto [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) .</span><span class="sxs-lookup"><span data-stu-id="42c73-127">In the request body, supply a JSON representation for the [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) object.</span></span>

<span data-ttu-id="42c73-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md).</span><span class="sxs-lookup"><span data-stu-id="42c73-128">The following table shows the properties that are required when you create the [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md).</span></span>

|<span data-ttu-id="42c73-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="42c73-129">Property</span></span>|<span data-ttu-id="42c73-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="42c73-130">Type</span></span>|<span data-ttu-id="42c73-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="42c73-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="42c73-132">id</span><span class="sxs-lookup"><span data-stu-id="42c73-132">id</span></span>|<span data-ttu-id="42c73-133">String</span><span class="sxs-lookup"><span data-stu-id="42c73-133">String</span></span>|<span data-ttu-id="42c73-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="42c73-134">Key of the entity.</span></span>|
|<span data-ttu-id="42c73-135">deviceName</span><span class="sxs-lookup"><span data-stu-id="42c73-135">deviceName</span></span>|<span data-ttu-id="42c73-136">String</span><span class="sxs-lookup"><span data-stu-id="42c73-136">String</span></span>|<span data-ttu-id="42c73-137">Nome do dispositivo</span><span class="sxs-lookup"><span data-stu-id="42c73-137">Device name</span></span>|
|<span data-ttu-id="42c73-138">deviceId</span><span class="sxs-lookup"><span data-stu-id="42c73-138">deviceId</span></span>|<span data-ttu-id="42c73-139">String</span><span class="sxs-lookup"><span data-stu-id="42c73-139">String</span></span>|<span data-ttu-id="42c73-140">ID do dispositivo</span><span class="sxs-lookup"><span data-stu-id="42c73-140">Device ID</span></span>|
|<span data-ttu-id="42c73-141">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="42c73-141">lastSyncDateTime</span></span>|<span data-ttu-id="42c73-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="42c73-142">DateTimeOffset</span></span>|<span data-ttu-id="42c73-143">Hora da data da última sincronização</span><span class="sxs-lookup"><span data-stu-id="42c73-143">Last sync date time</span></span>|
|<span data-ttu-id="42c73-144">mobileAppInstallStatusValue</span><span class="sxs-lookup"><span data-stu-id="42c73-144">mobileAppInstallStatusValue</span></span>|[<span data-ttu-id="42c73-145">resultantAppState</span><span class="sxs-lookup"><span data-stu-id="42c73-145">resultantAppState</span></span>](../resources/intune-shared-resultantappstate.md)|<span data-ttu-id="42c73-146">O estado de instalação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="42c73-146">The install state of the app.</span></span> <span data-ttu-id="42c73-147">Os valores possíveis são: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span><span class="sxs-lookup"><span data-stu-id="42c73-147">Possible values are: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span></span>|
|<span data-ttu-id="42c73-148">installState</span><span class="sxs-lookup"><span data-stu-id="42c73-148">installState</span></span>|[<span data-ttu-id="42c73-149">resultantAppState</span><span class="sxs-lookup"><span data-stu-id="42c73-149">resultantAppState</span></span>](../resources/intune-shared-resultantappstate.md)|<span data-ttu-id="42c73-150">O estado de instalação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="42c73-150">The install state of the app.</span></span> <span data-ttu-id="42c73-151">Os valores possíveis são: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span><span class="sxs-lookup"><span data-stu-id="42c73-151">Possible values are: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span></span>|
|<span data-ttu-id="42c73-152">installStateDetail</span><span class="sxs-lookup"><span data-stu-id="42c73-152">installStateDetail</span></span>|[<span data-ttu-id="42c73-153">resultantAppStateDetail</span><span class="sxs-lookup"><span data-stu-id="42c73-153">resultantAppStateDetail</span></span>](../resources/intune-apps-resultantappstatedetail.md)|<span data-ttu-id="42c73-154">Os detalhes do estado de instalação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="42c73-154">The install state detail of the app.</span></span> <span data-ttu-id="42c73-155">Os valores possíveis são `noAdditionalDetails`: `dependencyFailedToInstall`, `dependencyWithRequirementsNotMet`, `dependencyPendingReboot`, `dependencyWithAutoInstallDisabled`, `seeInstallErrorCode`, `autoInstallDisabled`, `seeUninstallErrorCode`, `pendingReboot`, `installingDependencies` `powerShellScriptRequirementNotMet` `registryRequirementNotMet`,,, `fileSystemRequirementNotMet`, `platformNotApplicable`, `minimumCpuSpeedNotMet`, `minimumLogicalProcessorCountNotMet`, `minimumPhysicalMemoryNotMet`, `minimumOsVersionNotMet`, `minimumDiskSpaceNotMet` ,,,,,,,, , `processorArchitectureNotApplicable`.</span><span class="sxs-lookup"><span data-stu-id="42c73-155">Possible values are: `noAdditionalDetails`, `dependencyFailedToInstall`, `dependencyWithRequirementsNotMet`, `dependencyPendingReboot`, `dependencyWithAutoInstallDisabled`, `seeInstallErrorCode`, `autoInstallDisabled`, `seeUninstallErrorCode`, `pendingReboot`, `installingDependencies`, `powerShellScriptRequirementNotMet`, `registryRequirementNotMet`, `fileSystemRequirementNotMet`, `platformNotApplicable`, `minimumCpuSpeedNotMet`, `minimumLogicalProcessorCountNotMet`, `minimumPhysicalMemoryNotMet`, `minimumOsVersionNotMet`, `minimumDiskSpaceNotMet`, `processorArchitectureNotApplicable`.</span></span>|
|<span data-ttu-id="42c73-156">errorCode</span><span class="sxs-lookup"><span data-stu-id="42c73-156">errorCode</span></span>|<span data-ttu-id="42c73-157">Int32</span><span class="sxs-lookup"><span data-stu-id="42c73-157">Int32</span></span>|<span data-ttu-id="42c73-158">O código de erro para instalação ou desinstalação de falhas.</span><span class="sxs-lookup"><span data-stu-id="42c73-158">The error code for install or uninstall failures.</span></span>|
|<span data-ttu-id="42c73-159">osVersion</span><span class="sxs-lookup"><span data-stu-id="42c73-159">osVersion</span></span>|<span data-ttu-id="42c73-160">String</span><span class="sxs-lookup"><span data-stu-id="42c73-160">String</span></span>|<span data-ttu-id="42c73-161">Versão do sistema operacional</span><span class="sxs-lookup"><span data-stu-id="42c73-161">OS Version</span></span>|
|<span data-ttu-id="42c73-162">osDescription</span><span class="sxs-lookup"><span data-stu-id="42c73-162">osDescription</span></span>|<span data-ttu-id="42c73-163">String</span><span class="sxs-lookup"><span data-stu-id="42c73-163">String</span></span>|<span data-ttu-id="42c73-164">Descrição do sistema operacional</span><span class="sxs-lookup"><span data-stu-id="42c73-164">OS Description</span></span>|
|<span data-ttu-id="42c73-165">userName</span><span class="sxs-lookup"><span data-stu-id="42c73-165">userName</span></span>|<span data-ttu-id="42c73-166">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="42c73-166">String</span></span>|<span data-ttu-id="42c73-167">Nome de usuário do dispositivo</span><span class="sxs-lookup"><span data-stu-id="42c73-167">Device User Name</span></span>|
|<span data-ttu-id="42c73-168">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="42c73-168">userPrincipalName</span></span>|<span data-ttu-id="42c73-169">String</span><span class="sxs-lookup"><span data-stu-id="42c73-169">String</span></span>|<span data-ttu-id="42c73-170">Nome UPN</span><span class="sxs-lookup"><span data-stu-id="42c73-170">User Principal Name</span></span>|
|<span data-ttu-id="42c73-171">displayVersion</span><span class="sxs-lookup"><span data-stu-id="42c73-171">displayVersion</span></span>|<span data-ttu-id="42c73-172">String</span><span class="sxs-lookup"><span data-stu-id="42c73-172">String</span></span>|<span data-ttu-id="42c73-173">Versão de leitura humana do aplicativo</span><span class="sxs-lookup"><span data-stu-id="42c73-173">Human readable version of the application</span></span>|



## <a name="response"></a><span data-ttu-id="42c73-174">Resposta</span><span class="sxs-lookup"><span data-stu-id="42c73-174">Response</span></span>
<span data-ttu-id="42c73-175">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="42c73-175">If successful, this method returns a `200 OK` response code and an updated [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="42c73-176">Exemplo</span><span class="sxs-lookup"><span data-stu-id="42c73-176">Example</span></span>

### <a name="request"></a><span data-ttu-id="42c73-177">Solicitação</span><span class="sxs-lookup"><span data-stu-id="42c73-177">Request</span></span>
<span data-ttu-id="42c73-178">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="42c73-178">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}
Content-type: application/json
Content-length: 555

{
  "@odata.type": "#microsoft.graph.mobileAppInstallStatus",
  "deviceName": "Device Name value",
  "deviceId": "Device Id value",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "mobileAppInstallStatusValue": "failed",
  "installState": "failed",
  "installStateDetail": "dependencyFailedToInstall",
  "errorCode": 9,
  "osVersion": "Os Version value",
  "osDescription": "Os Description value",
  "userName": "User Name value",
  "userPrincipalName": "User Principal Name value",
  "displayVersion": "Display Version value"
}
```

### <a name="response"></a><span data-ttu-id="42c73-179">Resposta</span><span class="sxs-lookup"><span data-stu-id="42c73-179">Response</span></span>
<span data-ttu-id="42c73-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="42c73-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 604

{
  "@odata.type": "#microsoft.graph.mobileAppInstallStatus",
  "id": "7560ee45-ee45-7560-45ee-607545ee6075",
  "deviceName": "Device Name value",
  "deviceId": "Device Id value",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "mobileAppInstallStatusValue": "failed",
  "installState": "failed",
  "installStateDetail": "dependencyFailedToInstall",
  "errorCode": 9,
  "osVersion": "Os Version value",
  "osDescription": "Os Description value",
  "userName": "User Name value",
  "userPrincipalName": "User Principal Name value",
  "displayVersion": "Display Version value"
}
```




