---
title: Atualizar mobileAppInstallStatus
description: Atualiza as propriedades de um objeto mobileAppInstallStatus.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a2cb7b3acedd1e036972380002eaf8795b1a35ba
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32489062"
---
# <a name="update-mobileappinstallstatus"></a><span data-ttu-id="65dc2-103">Atualizar mobileAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="65dc2-103">Update mobileAppInstallStatus</span></span>

> <span data-ttu-id="65dc2-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="65dc2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="65dc2-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="65dc2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="65dc2-106">Atualiza as propriedades de um objeto [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) .</span><span class="sxs-lookup"><span data-stu-id="65dc2-106">Update the properties of a [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="65dc2-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="65dc2-107">Prerequisites</span></span>
<span data-ttu-id="65dc2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="65dc2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="65dc2-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="65dc2-110">Permission type</span></span>|<span data-ttu-id="65dc2-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="65dc2-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="65dc2-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="65dc2-112">Delegated (work or school account)</span></span>|<span data-ttu-id="65dc2-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="65dc2-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="65dc2-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="65dc2-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="65dc2-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="65dc2-115">Not supported.</span></span>|
|<span data-ttu-id="65dc2-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="65dc2-116">Application</span></span>|<span data-ttu-id="65dc2-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="65dc2-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="65dc2-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="65dc2-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/deviceStatuses/{mobileAppInstallStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="65dc2-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="65dc2-119">Request headers</span></span>
|<span data-ttu-id="65dc2-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="65dc2-120">Header</span></span>|<span data-ttu-id="65dc2-121">Valor</span><span class="sxs-lookup"><span data-stu-id="65dc2-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="65dc2-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="65dc2-122">Authorization</span></span>|<span data-ttu-id="65dc2-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="65dc2-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="65dc2-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="65dc2-124">Accept</span></span>|<span data-ttu-id="65dc2-125">application/json</span><span class="sxs-lookup"><span data-stu-id="65dc2-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="65dc2-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="65dc2-126">Request body</span></span>
<span data-ttu-id="65dc2-127">No corpo da solicitação, forneça uma representação JSON do objeto [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) .</span><span class="sxs-lookup"><span data-stu-id="65dc2-127">In the request body, supply a JSON representation for the [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) object.</span></span>

<span data-ttu-id="65dc2-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md).</span><span class="sxs-lookup"><span data-stu-id="65dc2-128">The following table shows the properties that are required when you create the [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md).</span></span>

|<span data-ttu-id="65dc2-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="65dc2-129">Property</span></span>|<span data-ttu-id="65dc2-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="65dc2-130">Type</span></span>|<span data-ttu-id="65dc2-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="65dc2-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="65dc2-132">id</span><span class="sxs-lookup"><span data-stu-id="65dc2-132">id</span></span>|<span data-ttu-id="65dc2-133">String</span><span class="sxs-lookup"><span data-stu-id="65dc2-133">String</span></span>|<span data-ttu-id="65dc2-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="65dc2-134">Key of the entity.</span></span>|
|<span data-ttu-id="65dc2-135">deviceName</span><span class="sxs-lookup"><span data-stu-id="65dc2-135">deviceName</span></span>|<span data-ttu-id="65dc2-136">String</span><span class="sxs-lookup"><span data-stu-id="65dc2-136">String</span></span>|<span data-ttu-id="65dc2-137">Nome do dispositivo</span><span class="sxs-lookup"><span data-stu-id="65dc2-137">Device name</span></span>|
|<span data-ttu-id="65dc2-138">deviceId</span><span class="sxs-lookup"><span data-stu-id="65dc2-138">deviceId</span></span>|<span data-ttu-id="65dc2-139">String</span><span class="sxs-lookup"><span data-stu-id="65dc2-139">String</span></span>|<span data-ttu-id="65dc2-140">ID do dispositivo</span><span class="sxs-lookup"><span data-stu-id="65dc2-140">Device ID</span></span>|
|<span data-ttu-id="65dc2-141">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="65dc2-141">lastSyncDateTime</span></span>|<span data-ttu-id="65dc2-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="65dc2-142">DateTimeOffset</span></span>|<span data-ttu-id="65dc2-143">Hora da data da última sincronização</span><span class="sxs-lookup"><span data-stu-id="65dc2-143">Last sync date time</span></span>|
|<span data-ttu-id="65dc2-144">mobileAppInstallStatusValue</span><span class="sxs-lookup"><span data-stu-id="65dc2-144">mobileAppInstallStatusValue</span></span>|[<span data-ttu-id="65dc2-145">resultantAppState</span><span class="sxs-lookup"><span data-stu-id="65dc2-145">resultantAppState</span></span>](../resources/intune-shared-resultantappstate.md)|<span data-ttu-id="65dc2-146">O estado de instalação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="65dc2-146">The install state of the app.</span></span> <span data-ttu-id="65dc2-147">Os valores possíveis são: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span><span class="sxs-lookup"><span data-stu-id="65dc2-147">Possible values are: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span></span>|
|<span data-ttu-id="65dc2-148">installState</span><span class="sxs-lookup"><span data-stu-id="65dc2-148">installState</span></span>|[<span data-ttu-id="65dc2-149">resultantAppState</span><span class="sxs-lookup"><span data-stu-id="65dc2-149">resultantAppState</span></span>](../resources/intune-shared-resultantappstate.md)|<span data-ttu-id="65dc2-150">O estado de instalação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="65dc2-150">The install state of the app.</span></span> <span data-ttu-id="65dc2-151">Os valores possíveis são: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span><span class="sxs-lookup"><span data-stu-id="65dc2-151">Possible values are: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span></span>|
|<span data-ttu-id="65dc2-152">installStateDetail</span><span class="sxs-lookup"><span data-stu-id="65dc2-152">installStateDetail</span></span>|[<span data-ttu-id="65dc2-153">resultantAppStateDetail</span><span class="sxs-lookup"><span data-stu-id="65dc2-153">resultantAppStateDetail</span></span>](../resources/intune-apps-resultantappstatedetail.md)|<span data-ttu-id="65dc2-154">Os detalhes do estado de instalação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="65dc2-154">The install state detail of the app.</span></span> <span data-ttu-id="65dc2-155">Os valores possíveis são `noAdditionalDetails`: `dependencyFailedToInstall`, `dependencyWithRequirementsNotMet`, `dependencyPendingReboot`, `dependencyWithAutoInstallDisabled`, `seeInstallErrorCode`, `autoInstallDisabled`, `seeUninstallErrorCode`, `pendingReboot`, `installingDependencies` `powerShellScriptRequirementNotMet` `registryRequirementNotMet`,,, `fileSystemRequirementNotMet`, `platformNotApplicable`, `minimumCpuSpeedNotMet`, `minimumLogicalProcessorCountNotMet`, `minimumPhysicalMemoryNotMet`, `minimumOsVersionNotMet`, `minimumDiskSpaceNotMet` ,,,,,,,, , `processorArchitectureNotApplicable`.</span><span class="sxs-lookup"><span data-stu-id="65dc2-155">Possible values are: `noAdditionalDetails`, `dependencyFailedToInstall`, `dependencyWithRequirementsNotMet`, `dependencyPendingReboot`, `dependencyWithAutoInstallDisabled`, `seeInstallErrorCode`, `autoInstallDisabled`, `seeUninstallErrorCode`, `pendingReboot`, `installingDependencies`, `powerShellScriptRequirementNotMet`, `registryRequirementNotMet`, `fileSystemRequirementNotMet`, `platformNotApplicable`, `minimumCpuSpeedNotMet`, `minimumLogicalProcessorCountNotMet`, `minimumPhysicalMemoryNotMet`, `minimumOsVersionNotMet`, `minimumDiskSpaceNotMet`, `processorArchitectureNotApplicable`.</span></span>|
|<span data-ttu-id="65dc2-156">errorCode</span><span class="sxs-lookup"><span data-stu-id="65dc2-156">errorCode</span></span>|<span data-ttu-id="65dc2-157">Int32</span><span class="sxs-lookup"><span data-stu-id="65dc2-157">Int32</span></span>|<span data-ttu-id="65dc2-158">O código de erro para instalação ou desinstalação de falhas.</span><span class="sxs-lookup"><span data-stu-id="65dc2-158">The error code for install or uninstall failures.</span></span>|
|<span data-ttu-id="65dc2-159">osVersion</span><span class="sxs-lookup"><span data-stu-id="65dc2-159">osVersion</span></span>|<span data-ttu-id="65dc2-160">String</span><span class="sxs-lookup"><span data-stu-id="65dc2-160">String</span></span>|<span data-ttu-id="65dc2-161">Versão do sistema operacional</span><span class="sxs-lookup"><span data-stu-id="65dc2-161">OS Version</span></span>|
|<span data-ttu-id="65dc2-162">osDescription</span><span class="sxs-lookup"><span data-stu-id="65dc2-162">osDescription</span></span>|<span data-ttu-id="65dc2-163">String</span><span class="sxs-lookup"><span data-stu-id="65dc2-163">String</span></span>|<span data-ttu-id="65dc2-164">Descrição do sistema operacional</span><span class="sxs-lookup"><span data-stu-id="65dc2-164">OS Description</span></span>|
|<span data-ttu-id="65dc2-165">userName</span><span class="sxs-lookup"><span data-stu-id="65dc2-165">userName</span></span>|<span data-ttu-id="65dc2-166">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="65dc2-166">String</span></span>|<span data-ttu-id="65dc2-167">Nome de usuário do dispositivo</span><span class="sxs-lookup"><span data-stu-id="65dc2-167">Device User Name</span></span>|
|<span data-ttu-id="65dc2-168">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="65dc2-168">userPrincipalName</span></span>|<span data-ttu-id="65dc2-169">String</span><span class="sxs-lookup"><span data-stu-id="65dc2-169">String</span></span>|<span data-ttu-id="65dc2-170">Nome UPN</span><span class="sxs-lookup"><span data-stu-id="65dc2-170">User Principal Name</span></span>|
|<span data-ttu-id="65dc2-171">displayVersion</span><span class="sxs-lookup"><span data-stu-id="65dc2-171">displayVersion</span></span>|<span data-ttu-id="65dc2-172">String</span><span class="sxs-lookup"><span data-stu-id="65dc2-172">String</span></span>|<span data-ttu-id="65dc2-173">Versão de leitura humana do aplicativo</span><span class="sxs-lookup"><span data-stu-id="65dc2-173">Human readable version of the application</span></span>|



## <a name="response"></a><span data-ttu-id="65dc2-174">Resposta</span><span class="sxs-lookup"><span data-stu-id="65dc2-174">Response</span></span>
<span data-ttu-id="65dc2-175">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="65dc2-175">If successful, this method returns a `200 OK` response code and an updated [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="65dc2-176">Exemplo</span><span class="sxs-lookup"><span data-stu-id="65dc2-176">Example</span></span>

### <a name="request"></a><span data-ttu-id="65dc2-177">Solicitação</span><span class="sxs-lookup"><span data-stu-id="65dc2-177">Request</span></span>
<span data-ttu-id="65dc2-178">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="65dc2-178">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="65dc2-179">Resposta</span><span class="sxs-lookup"><span data-stu-id="65dc2-179">Response</span></span>
<span data-ttu-id="65dc2-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="65dc2-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





