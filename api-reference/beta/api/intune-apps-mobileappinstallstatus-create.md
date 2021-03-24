---
title: Criar mobileAppInstallStatus
description: Crie um novo objeto mobileAppInstallStatus.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: c0c6f07e12240325b1f01dddf857268399026cb1
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51143168"
---
# <a name="create-mobileappinstallstatus"></a><span data-ttu-id="e0626-103">Criar mobileAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="e0626-103">Create mobileAppInstallStatus</span></span>

<span data-ttu-id="e0626-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e0626-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e0626-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e0626-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e0626-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e0626-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e0626-107">Crie um novo [objeto mobileAppInstallStatus.](../resources/intune-apps-mobileappinstallstatus.md)</span><span class="sxs-lookup"><span data-stu-id="e0626-107">Create a new [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e0626-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e0626-108">Prerequisites</span></span>
<span data-ttu-id="e0626-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e0626-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e0626-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e0626-111">Permission type</span></span>|<span data-ttu-id="e0626-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e0626-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e0626-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e0626-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e0626-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e0626-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="e0626-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e0626-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e0626-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e0626-116">Not supported.</span></span>|
|<span data-ttu-id="e0626-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e0626-117">Application</span></span>|<span data-ttu-id="e0626-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e0626-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e0626-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e0626-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses
POST /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/deviceStatuses
```

## <a name="request-headers"></a><span data-ttu-id="e0626-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e0626-120">Request headers</span></span>
|<span data-ttu-id="e0626-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e0626-121">Header</span></span>|<span data-ttu-id="e0626-122">Valor</span><span class="sxs-lookup"><span data-stu-id="e0626-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e0626-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="e0626-123">Authorization</span></span>|<span data-ttu-id="e0626-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e0626-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e0626-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e0626-125">Accept</span></span>|<span data-ttu-id="e0626-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e0626-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e0626-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e0626-127">Request body</span></span>
<span data-ttu-id="e0626-128">No corpo da solicitação, fornece uma representação JSON para o objeto mobileAppInstallStatus.</span><span class="sxs-lookup"><span data-stu-id="e0626-128">In the request body, supply a JSON representation for the mobileAppInstallStatus object.</span></span>

<span data-ttu-id="e0626-129">A tabela a seguir mostra as propriedades necessárias ao criar o mobileAppInstallStatus.</span><span class="sxs-lookup"><span data-stu-id="e0626-129">The following table shows the properties that are required when you create the mobileAppInstallStatus.</span></span>

|<span data-ttu-id="e0626-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e0626-130">Property</span></span>|<span data-ttu-id="e0626-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="e0626-131">Type</span></span>|<span data-ttu-id="e0626-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="e0626-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e0626-133">id</span><span class="sxs-lookup"><span data-stu-id="e0626-133">id</span></span>|<span data-ttu-id="e0626-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e0626-134">String</span></span>|<span data-ttu-id="e0626-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="e0626-135">Key of the entity.</span></span>|
|<span data-ttu-id="e0626-136">deviceName</span><span class="sxs-lookup"><span data-stu-id="e0626-136">deviceName</span></span>|<span data-ttu-id="e0626-137">String</span><span class="sxs-lookup"><span data-stu-id="e0626-137">String</span></span>|<span data-ttu-id="e0626-138">Nome do dispositivo</span><span class="sxs-lookup"><span data-stu-id="e0626-138">Device name</span></span>|
|<span data-ttu-id="e0626-139">deviceId</span><span class="sxs-lookup"><span data-stu-id="e0626-139">deviceId</span></span>|<span data-ttu-id="e0626-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e0626-140">String</span></span>|<span data-ttu-id="e0626-141">ID do dispositivo</span><span class="sxs-lookup"><span data-stu-id="e0626-141">Device ID</span></span>|
|<span data-ttu-id="e0626-142">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="e0626-142">lastSyncDateTime</span></span>|<span data-ttu-id="e0626-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e0626-143">DateTimeOffset</span></span>|<span data-ttu-id="e0626-144">Hora da última sincronização</span><span class="sxs-lookup"><span data-stu-id="e0626-144">Last sync date time</span></span>|
|<span data-ttu-id="e0626-145">mobileAppInstallStatusValue</span><span class="sxs-lookup"><span data-stu-id="e0626-145">mobileAppInstallStatusValue</span></span>|[<span data-ttu-id="e0626-146">resultantAppState</span><span class="sxs-lookup"><span data-stu-id="e0626-146">resultantAppState</span></span>](../resources/intune-shared-resultantappstate.md)|<span data-ttu-id="e0626-147">O estado de instalação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e0626-147">The install state of the app.</span></span> <span data-ttu-id="e0626-148">Os valores possíveis são: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span><span class="sxs-lookup"><span data-stu-id="e0626-148">Possible values are: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span></span>|
|<span data-ttu-id="e0626-149">installState</span><span class="sxs-lookup"><span data-stu-id="e0626-149">installState</span></span>|[<span data-ttu-id="e0626-150">resultantAppState</span><span class="sxs-lookup"><span data-stu-id="e0626-150">resultantAppState</span></span>](../resources/intune-shared-resultantappstate.md)|<span data-ttu-id="e0626-151">O estado de instalação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e0626-151">The install state of the app.</span></span> <span data-ttu-id="e0626-152">Os valores possíveis são: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span><span class="sxs-lookup"><span data-stu-id="e0626-152">Possible values are: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span></span>|
|<span data-ttu-id="e0626-153">installStateDetail</span><span class="sxs-lookup"><span data-stu-id="e0626-153">installStateDetail</span></span>|[<span data-ttu-id="e0626-154">resultantAppStateDetail</span><span class="sxs-lookup"><span data-stu-id="e0626-154">resultantAppStateDetail</span></span>](../resources/intune-apps-resultantappstatedetail.md)|<span data-ttu-id="e0626-155">O detalhe de estado de instalação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e0626-155">The install state detail of the app.</span></span> <span data-ttu-id="e0626-156">Os valores possíveis são: `noAdditionalDetails` , , , , , , , `dependencyFailedToInstall` `dependencyWithRequirementsNotMet` `dependencyPendingReboot` `dependencyWithAutoInstallDisabled` `iosAppStoreUpdateFailedToInstall` `vppAppHasUpdateAvailable` `userRejectedUpdate` `seeInstallErrorCode` `autoInstallDisabled` `managedAppNoLongerPresent` `userRejectedInstall` `userIsNotLoggedIntoAppStore` `seeUninstallErrorCode` , `pendingReboot` `installingDependencies` `contentDownloaded` `powerShellScriptRequirementNotMet` `registryRequirementNotMet` `fileSystemRequirementNotMet` `platformNotApplicable` `minimumCpuSpeedNotMet` `minimumLogicalProcessorCountNotMet` `minimumPhysicalMemoryNotMet` `minimumOsVersionNotMet` `minimumDiskSpaceNotMet` `processorArchitectureNotApplicable`</span><span class="sxs-lookup"><span data-stu-id="e0626-156">Possible values are: `noAdditionalDetails`, `dependencyFailedToInstall`, `dependencyWithRequirementsNotMet`, `dependencyPendingReboot`, `dependencyWithAutoInstallDisabled`, `iosAppStoreUpdateFailedToInstall`, `vppAppHasUpdateAvailable`, `userRejectedUpdate`, `seeInstallErrorCode`, `autoInstallDisabled`, `managedAppNoLongerPresent`, `userRejectedInstall`, `userIsNotLoggedIntoAppStore`, `seeUninstallErrorCode`, `pendingReboot`, `installingDependencies`, `contentDownloaded`, `powerShellScriptRequirementNotMet`, `registryRequirementNotMet`, `fileSystemRequirementNotMet`, `platformNotApplicable`, `minimumCpuSpeedNotMet`, `minimumLogicalProcessorCountNotMet`, `minimumPhysicalMemoryNotMet`, `minimumOsVersionNotMet`, `minimumDiskSpaceNotMet`, `processorArchitectureNotApplicable`.</span></span>|
|<span data-ttu-id="e0626-157">errorCode</span><span class="sxs-lookup"><span data-stu-id="e0626-157">errorCode</span></span>|<span data-ttu-id="e0626-158">Int32</span><span class="sxs-lookup"><span data-stu-id="e0626-158">Int32</span></span>|<span data-ttu-id="e0626-159">O código de erro para instalar ou desinstalar falhas.</span><span class="sxs-lookup"><span data-stu-id="e0626-159">The error code for install or uninstall failures.</span></span>|
|<span data-ttu-id="e0626-160">osVersion</span><span class="sxs-lookup"><span data-stu-id="e0626-160">osVersion</span></span>|<span data-ttu-id="e0626-161">String</span><span class="sxs-lookup"><span data-stu-id="e0626-161">String</span></span>|<span data-ttu-id="e0626-162">Versão do sistema operacional</span><span class="sxs-lookup"><span data-stu-id="e0626-162">OS Version</span></span>|
|<span data-ttu-id="e0626-163">osDescription</span><span class="sxs-lookup"><span data-stu-id="e0626-163">osDescription</span></span>|<span data-ttu-id="e0626-164">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e0626-164">String</span></span>|<span data-ttu-id="e0626-165">Descrição do sistema operacional</span><span class="sxs-lookup"><span data-stu-id="e0626-165">OS Description</span></span>|
|<span data-ttu-id="e0626-166">userName</span><span class="sxs-lookup"><span data-stu-id="e0626-166">userName</span></span>|<span data-ttu-id="e0626-167">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e0626-167">String</span></span>|<span data-ttu-id="e0626-168">Nome de usuário do dispositivo</span><span class="sxs-lookup"><span data-stu-id="e0626-168">Device User Name</span></span>|
|<span data-ttu-id="e0626-169">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="e0626-169">userPrincipalName</span></span>|<span data-ttu-id="e0626-170">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e0626-170">String</span></span>|<span data-ttu-id="e0626-171">Nome UPN</span><span class="sxs-lookup"><span data-stu-id="e0626-171">User Principal Name</span></span>|
|<span data-ttu-id="e0626-172">displayVersion</span><span class="sxs-lookup"><span data-stu-id="e0626-172">displayVersion</span></span>|<span data-ttu-id="e0626-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e0626-173">String</span></span>|<span data-ttu-id="e0626-174">Versão acessível humana do aplicativo</span><span class="sxs-lookup"><span data-stu-id="e0626-174">Human readable version of the application</span></span>|



## <a name="response"></a><span data-ttu-id="e0626-175">Resposta</span><span class="sxs-lookup"><span data-stu-id="e0626-175">Response</span></span>
<span data-ttu-id="e0626-176">Se tiver êxito, este método retornará um código `201 Created` de resposta e um objeto [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e0626-176">If successful, this method returns a `201 Created` response code and a [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e0626-177">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e0626-177">Example</span></span>

### <a name="request"></a><span data-ttu-id="e0626-178">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e0626-178">Request</span></span>
<span data-ttu-id="e0626-179">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e0626-179">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses
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

### <a name="response"></a><span data-ttu-id="e0626-180">Resposta</span><span class="sxs-lookup"><span data-stu-id="e0626-180">Response</span></span>
<span data-ttu-id="e0626-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e0626-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




