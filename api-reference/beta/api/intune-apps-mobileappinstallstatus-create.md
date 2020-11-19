---
title: Criar mobileAppInstallStatus
description: Criar um novo objeto mobileAppInstallStatus.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 1040c85a1c764139a399d47ebc9905e58e6ff0d3
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49248403"
---
# <a name="create-mobileappinstallstatus"></a><span data-ttu-id="ced99-103">Criar mobileAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="ced99-103">Create mobileAppInstallStatus</span></span>

<span data-ttu-id="ced99-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ced99-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ced99-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ced99-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ced99-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ced99-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ced99-107">Criar um novo objeto [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) .</span><span class="sxs-lookup"><span data-stu-id="ced99-107">Create a new [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ced99-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ced99-108">Prerequisites</span></span>
<span data-ttu-id="ced99-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ced99-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ced99-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ced99-111">Permission type</span></span>|<span data-ttu-id="ced99-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ced99-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ced99-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ced99-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ced99-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ced99-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="ced99-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ced99-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ced99-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ced99-116">Not supported.</span></span>|
|<span data-ttu-id="ced99-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ced99-117">Application</span></span>|<span data-ttu-id="ced99-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ced99-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ced99-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ced99-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses
POST /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/deviceStatuses
```

## <a name="request-headers"></a><span data-ttu-id="ced99-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ced99-120">Request headers</span></span>
|<span data-ttu-id="ced99-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ced99-121">Header</span></span>|<span data-ttu-id="ced99-122">Valor</span><span class="sxs-lookup"><span data-stu-id="ced99-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ced99-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="ced99-123">Authorization</span></span>|<span data-ttu-id="ced99-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ced99-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ced99-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ced99-125">Accept</span></span>|<span data-ttu-id="ced99-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ced99-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ced99-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ced99-127">Request body</span></span>
<span data-ttu-id="ced99-128">No corpo da solicitação, forneça uma representação JSON do objeto mobileAppInstallStatus.</span><span class="sxs-lookup"><span data-stu-id="ced99-128">In the request body, supply a JSON representation for the mobileAppInstallStatus object.</span></span>

<span data-ttu-id="ced99-129">A tabela a seguir mostra as propriedades que são necessárias ao criar mobileAppInstallStatus.</span><span class="sxs-lookup"><span data-stu-id="ced99-129">The following table shows the properties that are required when you create the mobileAppInstallStatus.</span></span>

|<span data-ttu-id="ced99-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ced99-130">Property</span></span>|<span data-ttu-id="ced99-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="ced99-131">Type</span></span>|<span data-ttu-id="ced99-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="ced99-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ced99-133">id</span><span class="sxs-lookup"><span data-stu-id="ced99-133">id</span></span>|<span data-ttu-id="ced99-134">String</span><span class="sxs-lookup"><span data-stu-id="ced99-134">String</span></span>|<span data-ttu-id="ced99-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="ced99-135">Key of the entity.</span></span>|
|<span data-ttu-id="ced99-136">deviceName</span><span class="sxs-lookup"><span data-stu-id="ced99-136">deviceName</span></span>|<span data-ttu-id="ced99-137">String</span><span class="sxs-lookup"><span data-stu-id="ced99-137">String</span></span>|<span data-ttu-id="ced99-138">Nome do dispositivo</span><span class="sxs-lookup"><span data-stu-id="ced99-138">Device name</span></span>|
|<span data-ttu-id="ced99-139">deviceId</span><span class="sxs-lookup"><span data-stu-id="ced99-139">deviceId</span></span>|<span data-ttu-id="ced99-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ced99-140">String</span></span>|<span data-ttu-id="ced99-141">ID do dispositivo</span><span class="sxs-lookup"><span data-stu-id="ced99-141">Device ID</span></span>|
|<span data-ttu-id="ced99-142">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="ced99-142">lastSyncDateTime</span></span>|<span data-ttu-id="ced99-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ced99-143">DateTimeOffset</span></span>|<span data-ttu-id="ced99-144">Hora da data da última sincronização</span><span class="sxs-lookup"><span data-stu-id="ced99-144">Last sync date time</span></span>|
|<span data-ttu-id="ced99-145">mobileAppInstallStatusValue</span><span class="sxs-lookup"><span data-stu-id="ced99-145">mobileAppInstallStatusValue</span></span>|[<span data-ttu-id="ced99-146">resultantAppState</span><span class="sxs-lookup"><span data-stu-id="ced99-146">resultantAppState</span></span>](../resources/intune-shared-resultantappstate.md)|<span data-ttu-id="ced99-147">O estado de instalação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="ced99-147">The install state of the app.</span></span> <span data-ttu-id="ced99-148">Os valores possíveis são: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span><span class="sxs-lookup"><span data-stu-id="ced99-148">Possible values are: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span></span>|
|<span data-ttu-id="ced99-149">installState</span><span class="sxs-lookup"><span data-stu-id="ced99-149">installState</span></span>|[<span data-ttu-id="ced99-150">resultantAppState</span><span class="sxs-lookup"><span data-stu-id="ced99-150">resultantAppState</span></span>](../resources/intune-shared-resultantappstate.md)|<span data-ttu-id="ced99-151">O estado de instalação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="ced99-151">The install state of the app.</span></span> <span data-ttu-id="ced99-152">Os valores possíveis são: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span><span class="sxs-lookup"><span data-stu-id="ced99-152">Possible values are: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span></span>|
|<span data-ttu-id="ced99-153">installStateDetail</span><span class="sxs-lookup"><span data-stu-id="ced99-153">installStateDetail</span></span>|[<span data-ttu-id="ced99-154">resultantAppStateDetail</span><span class="sxs-lookup"><span data-stu-id="ced99-154">resultantAppStateDetail</span></span>](../resources/intune-apps-resultantappstatedetail.md)|<span data-ttu-id="ced99-155">Os detalhes do estado de instalação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="ced99-155">The install state detail of the app.</span></span> <span data-ttu-id="ced99-156">Os valores possíveis são:,,,,,,,,,,,,,,, `noAdditionalDetails` `dependencyFailedToInstall` `dependencyWithRequirementsNotMet` `dependencyPendingReboot` `dependencyWithAutoInstallDisabled` `iosAppStoreUpdateFailedToInstall` `vppAppHasUpdateAvailable` `userRejectedUpdate` `seeInstallErrorCode` `autoInstallDisabled` `managedAppNoLongerPresent` `userRejectedInstall` `userIsNotLoggedIntoAppStore` `seeUninstallErrorCode` `pendingReboot` `installingDependencies` `contentDownloaded` , `powerShellScriptRequirementNotMet` , `registryRequirementNotMet` , `fileSystemRequirementNotMet` `platformNotApplicable` `minimumCpuSpeedNotMet` `minimumLogicalProcessorCountNotMet` `minimumPhysicalMemoryNotMet` `minimumOsVersionNotMet` `minimumDiskSpaceNotMet` `processorArchitectureNotApplicable` ,,,,,,,,,,,,.</span><span class="sxs-lookup"><span data-stu-id="ced99-156">Possible values are: `noAdditionalDetails`, `dependencyFailedToInstall`, `dependencyWithRequirementsNotMet`, `dependencyPendingReboot`, `dependencyWithAutoInstallDisabled`, `iosAppStoreUpdateFailedToInstall`, `vppAppHasUpdateAvailable`, `userRejectedUpdate`, `seeInstallErrorCode`, `autoInstallDisabled`, `managedAppNoLongerPresent`, `userRejectedInstall`, `userIsNotLoggedIntoAppStore`, `seeUninstallErrorCode`, `pendingReboot`, `installingDependencies`, `contentDownloaded`, `powerShellScriptRequirementNotMet`, `registryRequirementNotMet`, `fileSystemRequirementNotMet`, `platformNotApplicable`, `minimumCpuSpeedNotMet`, `minimumLogicalProcessorCountNotMet`, `minimumPhysicalMemoryNotMet`, `minimumOsVersionNotMet`, `minimumDiskSpaceNotMet`, `processorArchitectureNotApplicable`.</span></span>|
|<span data-ttu-id="ced99-157">errorCode</span><span class="sxs-lookup"><span data-stu-id="ced99-157">errorCode</span></span>|<span data-ttu-id="ced99-158">Int32</span><span class="sxs-lookup"><span data-stu-id="ced99-158">Int32</span></span>|<span data-ttu-id="ced99-159">O código de erro para instalação ou desinstalação de falhas.</span><span class="sxs-lookup"><span data-stu-id="ced99-159">The error code for install or uninstall failures.</span></span>|
|<span data-ttu-id="ced99-160">osVersion</span><span class="sxs-lookup"><span data-stu-id="ced99-160">osVersion</span></span>|<span data-ttu-id="ced99-161">String</span><span class="sxs-lookup"><span data-stu-id="ced99-161">String</span></span>|<span data-ttu-id="ced99-162">Versão do sistema operacional</span><span class="sxs-lookup"><span data-stu-id="ced99-162">OS Version</span></span>|
|<span data-ttu-id="ced99-163">osDescription</span><span class="sxs-lookup"><span data-stu-id="ced99-163">osDescription</span></span>|<span data-ttu-id="ced99-164">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ced99-164">String</span></span>|<span data-ttu-id="ced99-165">Descrição do sistema operacional</span><span class="sxs-lookup"><span data-stu-id="ced99-165">OS Description</span></span>|
|<span data-ttu-id="ced99-166">userName</span><span class="sxs-lookup"><span data-stu-id="ced99-166">userName</span></span>|<span data-ttu-id="ced99-167">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ced99-167">String</span></span>|<span data-ttu-id="ced99-168">Nome de usuário do dispositivo</span><span class="sxs-lookup"><span data-stu-id="ced99-168">Device User Name</span></span>|
|<span data-ttu-id="ced99-169">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="ced99-169">userPrincipalName</span></span>|<span data-ttu-id="ced99-170">String</span><span class="sxs-lookup"><span data-stu-id="ced99-170">String</span></span>|<span data-ttu-id="ced99-171">Nome UPN</span><span class="sxs-lookup"><span data-stu-id="ced99-171">User Principal Name</span></span>|
|<span data-ttu-id="ced99-172">displayVersion</span><span class="sxs-lookup"><span data-stu-id="ced99-172">displayVersion</span></span>|<span data-ttu-id="ced99-173">String</span><span class="sxs-lookup"><span data-stu-id="ced99-173">String</span></span>|<span data-ttu-id="ced99-174">Versão de leitura humana do aplicativo</span><span class="sxs-lookup"><span data-stu-id="ced99-174">Human readable version of the application</span></span>|



## <a name="response"></a><span data-ttu-id="ced99-175">Resposta</span><span class="sxs-lookup"><span data-stu-id="ced99-175">Response</span></span>
<span data-ttu-id="ced99-176">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ced99-176">If successful, this method returns a `201 Created` response code and a [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ced99-177">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ced99-177">Example</span></span>

### <a name="request"></a><span data-ttu-id="ced99-178">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ced99-178">Request</span></span>
<span data-ttu-id="ced99-179">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ced99-179">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="ced99-180">Resposta</span><span class="sxs-lookup"><span data-stu-id="ced99-180">Response</span></span>
<span data-ttu-id="ced99-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ced99-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




