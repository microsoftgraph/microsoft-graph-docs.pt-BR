---
title: Atualizar mobileAppInstallStatus
description: Atualiza as propriedades de um objeto mobileAppInstallStatus.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 4a6fe1c21271578012545527647a11030dfe2218
ms.sourcegitcommit: dc3bade0c096d5ce716d4bc07cd9c7cabb52477b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/18/2020
ms.locfileid: "46791033"
---
# <a name="update-mobileappinstallstatus"></a><span data-ttu-id="079df-103">Atualizar mobileAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="079df-103">Update mobileAppInstallStatus</span></span>

<span data-ttu-id="079df-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="079df-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="079df-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="079df-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="079df-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="079df-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="079df-107">Atualiza as propriedades de um objeto [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) .</span><span class="sxs-lookup"><span data-stu-id="079df-107">Update the properties of a [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="079df-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="079df-108">Prerequisites</span></span>
<span data-ttu-id="079df-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="079df-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="079df-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="079df-111">Permission type</span></span>|<span data-ttu-id="079df-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="079df-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="079df-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="079df-113">Delegated (work or school account)</span></span>|<span data-ttu-id="079df-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="079df-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="079df-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="079df-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="079df-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="079df-116">Not supported.</span></span>|
|<span data-ttu-id="079df-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="079df-117">Application</span></span>|<span data-ttu-id="079df-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="079df-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="079df-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="079df-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/deviceStatuses/{mobileAppInstallStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="079df-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="079df-120">Request headers</span></span>
|<span data-ttu-id="079df-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="079df-121">Header</span></span>|<span data-ttu-id="079df-122">Valor</span><span class="sxs-lookup"><span data-stu-id="079df-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="079df-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="079df-123">Authorization</span></span>|<span data-ttu-id="079df-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="079df-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="079df-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="079df-125">Accept</span></span>|<span data-ttu-id="079df-126">application/json</span><span class="sxs-lookup"><span data-stu-id="079df-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="079df-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="079df-127">Request body</span></span>
<span data-ttu-id="079df-128">No corpo da solicitação, forneça uma representação JSON do objeto [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) .</span><span class="sxs-lookup"><span data-stu-id="079df-128">In the request body, supply a JSON representation for the [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) object.</span></span>

<span data-ttu-id="079df-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md).</span><span class="sxs-lookup"><span data-stu-id="079df-129">The following table shows the properties that are required when you create the [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md).</span></span>

|<span data-ttu-id="079df-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="079df-130">Property</span></span>|<span data-ttu-id="079df-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="079df-131">Type</span></span>|<span data-ttu-id="079df-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="079df-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="079df-133">id</span><span class="sxs-lookup"><span data-stu-id="079df-133">id</span></span>|<span data-ttu-id="079df-134">String</span><span class="sxs-lookup"><span data-stu-id="079df-134">String</span></span>|<span data-ttu-id="079df-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="079df-135">Key of the entity.</span></span>|
|<span data-ttu-id="079df-136">deviceName</span><span class="sxs-lookup"><span data-stu-id="079df-136">deviceName</span></span>|<span data-ttu-id="079df-137">String</span><span class="sxs-lookup"><span data-stu-id="079df-137">String</span></span>|<span data-ttu-id="079df-138">Nome do dispositivo</span><span class="sxs-lookup"><span data-stu-id="079df-138">Device name</span></span>|
|<span data-ttu-id="079df-139">deviceId</span><span class="sxs-lookup"><span data-stu-id="079df-139">deviceId</span></span>|<span data-ttu-id="079df-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="079df-140">String</span></span>|<span data-ttu-id="079df-141">ID do dispositivo</span><span class="sxs-lookup"><span data-stu-id="079df-141">Device ID</span></span>|
|<span data-ttu-id="079df-142">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="079df-142">lastSyncDateTime</span></span>|<span data-ttu-id="079df-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="079df-143">DateTimeOffset</span></span>|<span data-ttu-id="079df-144">Hora da data da última sincronização</span><span class="sxs-lookup"><span data-stu-id="079df-144">Last sync date time</span></span>|
|<span data-ttu-id="079df-145">mobileAppInstallStatusValue</span><span class="sxs-lookup"><span data-stu-id="079df-145">mobileAppInstallStatusValue</span></span>|[<span data-ttu-id="079df-146">resultantAppState</span><span class="sxs-lookup"><span data-stu-id="079df-146">resultantAppState</span></span>](../resources/intune-shared-resultantappstate.md)|<span data-ttu-id="079df-147">O estado de instalação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="079df-147">The install state of the app.</span></span> <span data-ttu-id="079df-148">Os valores possíveis são: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span><span class="sxs-lookup"><span data-stu-id="079df-148">Possible values are: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span></span>|
|<span data-ttu-id="079df-149">installState</span><span class="sxs-lookup"><span data-stu-id="079df-149">installState</span></span>|[<span data-ttu-id="079df-150">resultantAppState</span><span class="sxs-lookup"><span data-stu-id="079df-150">resultantAppState</span></span>](../resources/intune-shared-resultantappstate.md)|<span data-ttu-id="079df-151">O estado de instalação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="079df-151">The install state of the app.</span></span> <span data-ttu-id="079df-152">Os valores possíveis são: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span><span class="sxs-lookup"><span data-stu-id="079df-152">Possible values are: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span></span>|
|<span data-ttu-id="079df-153">installStateDetail</span><span class="sxs-lookup"><span data-stu-id="079df-153">installStateDetail</span></span>|[<span data-ttu-id="079df-154">resultantAppStateDetail</span><span class="sxs-lookup"><span data-stu-id="079df-154">resultantAppStateDetail</span></span>](../resources/intune-apps-resultantappstatedetail.md)|<span data-ttu-id="079df-155">Os detalhes do estado de instalação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="079df-155">The install state detail of the app.</span></span> <span data-ttu-id="079df-156">Os valores possíveis são:,,,,,,,,,,,,,,, `noAdditionalDetails` `dependencyFailedToInstall` `dependencyWithRequirementsNotMet` `dependencyPendingReboot` `dependencyWithAutoInstallDisabled` `iosAppStoreUpdateFailedToInstall` `vppAppHasUpdateAvailable` `userRejectedUpdate` `seeInstallErrorCode` `autoInstallDisabled` `managedAppNoLongerPresent` `userRejectedInstall` `userIsNotLoggedIntoAppStore` `seeUninstallErrorCode` `pendingReboot` `installingDependencies` `contentDownloaded` , `powerShellScriptRequirementNotMet` , `registryRequirementNotMet` , `fileSystemRequirementNotMet` `platformNotApplicable` `minimumCpuSpeedNotMet` `minimumLogicalProcessorCountNotMet` `minimumPhysicalMemoryNotMet` `minimumOsVersionNotMet` `minimumDiskSpaceNotMet` `processorArchitectureNotApplicable` ,,,,,,,,,,,,.</span><span class="sxs-lookup"><span data-stu-id="079df-156">Possible values are: `noAdditionalDetails`, `dependencyFailedToInstall`, `dependencyWithRequirementsNotMet`, `dependencyPendingReboot`, `dependencyWithAutoInstallDisabled`, `iosAppStoreUpdateFailedToInstall`, `vppAppHasUpdateAvailable`, `userRejectedUpdate`, `seeInstallErrorCode`, `autoInstallDisabled`, `managedAppNoLongerPresent`, `userRejectedInstall`, `userIsNotLoggedIntoAppStore`, `seeUninstallErrorCode`, `pendingReboot`, `installingDependencies`, `contentDownloaded`, `powerShellScriptRequirementNotMet`, `registryRequirementNotMet`, `fileSystemRequirementNotMet`, `platformNotApplicable`, `minimumCpuSpeedNotMet`, `minimumLogicalProcessorCountNotMet`, `minimumPhysicalMemoryNotMet`, `minimumOsVersionNotMet`, `minimumDiskSpaceNotMet`, `processorArchitectureNotApplicable`.</span></span>|
|<span data-ttu-id="079df-157">errorCode</span><span class="sxs-lookup"><span data-stu-id="079df-157">errorCode</span></span>|<span data-ttu-id="079df-158">Int32</span><span class="sxs-lookup"><span data-stu-id="079df-158">Int32</span></span>|<span data-ttu-id="079df-159">O código de erro para instalação ou desinstalação de falhas.</span><span class="sxs-lookup"><span data-stu-id="079df-159">The error code for install or uninstall failures.</span></span>|
|<span data-ttu-id="079df-160">osVersion</span><span class="sxs-lookup"><span data-stu-id="079df-160">osVersion</span></span>|<span data-ttu-id="079df-161">String</span><span class="sxs-lookup"><span data-stu-id="079df-161">String</span></span>|<span data-ttu-id="079df-162">Versão do sistema operacional</span><span class="sxs-lookup"><span data-stu-id="079df-162">OS Version</span></span>|
|<span data-ttu-id="079df-163">osDescription</span><span class="sxs-lookup"><span data-stu-id="079df-163">osDescription</span></span>|<span data-ttu-id="079df-164">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="079df-164">String</span></span>|<span data-ttu-id="079df-165">Descrição do sistema operacional</span><span class="sxs-lookup"><span data-stu-id="079df-165">OS Description</span></span>|
|<span data-ttu-id="079df-166">userName</span><span class="sxs-lookup"><span data-stu-id="079df-166">userName</span></span>|<span data-ttu-id="079df-167">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="079df-167">String</span></span>|<span data-ttu-id="079df-168">Nome de usuário do dispositivo</span><span class="sxs-lookup"><span data-stu-id="079df-168">Device User Name</span></span>|
|<span data-ttu-id="079df-169">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="079df-169">userPrincipalName</span></span>|<span data-ttu-id="079df-170">String</span><span class="sxs-lookup"><span data-stu-id="079df-170">String</span></span>|<span data-ttu-id="079df-171">Nome UPN</span><span class="sxs-lookup"><span data-stu-id="079df-171">User Principal Name</span></span>|
|<span data-ttu-id="079df-172">displayVersion</span><span class="sxs-lookup"><span data-stu-id="079df-172">displayVersion</span></span>|<span data-ttu-id="079df-173">String</span><span class="sxs-lookup"><span data-stu-id="079df-173">String</span></span>|<span data-ttu-id="079df-174">Versão de leitura humana do aplicativo</span><span class="sxs-lookup"><span data-stu-id="079df-174">Human readable version of the application</span></span>|



## <a name="response"></a><span data-ttu-id="079df-175">Resposta</span><span class="sxs-lookup"><span data-stu-id="079df-175">Response</span></span>
<span data-ttu-id="079df-176">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="079df-176">If successful, this method returns a `200 OK` response code and an updated [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="079df-177">Exemplo</span><span class="sxs-lookup"><span data-stu-id="079df-177">Example</span></span>

### <a name="request"></a><span data-ttu-id="079df-178">Solicitação</span><span class="sxs-lookup"><span data-stu-id="079df-178">Request</span></span>
<span data-ttu-id="079df-179">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="079df-179">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="079df-180">Resposta</span><span class="sxs-lookup"><span data-stu-id="079df-180">Response</span></span>
<span data-ttu-id="079df-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="079df-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



