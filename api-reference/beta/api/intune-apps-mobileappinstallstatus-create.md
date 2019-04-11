---
title: Criar mobileAppInstallStatus
description: Criar um novo objeto mobileAppInstallStatus.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: bc9e512419110c610397e4655022f00249d4b3cb
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31792073"
---
# <a name="create-mobileappinstallstatus"></a><span data-ttu-id="14ed9-103">Criar mobileAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="14ed9-103">Create mobileAppInstallStatus</span></span>

> <span data-ttu-id="14ed9-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="14ed9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="14ed9-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="14ed9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="14ed9-106">Criar um novo objeto [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) .</span><span class="sxs-lookup"><span data-stu-id="14ed9-106">Create a new [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="14ed9-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="14ed9-107">Prerequisites</span></span>
<span data-ttu-id="14ed9-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="14ed9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="14ed9-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="14ed9-110">Permission type</span></span>|<span data-ttu-id="14ed9-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="14ed9-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="14ed9-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="14ed9-112">Delegated (work or school account)</span></span>|<span data-ttu-id="14ed9-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="14ed9-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="14ed9-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="14ed9-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="14ed9-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="14ed9-115">Not supported.</span></span>|
|<span data-ttu-id="14ed9-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="14ed9-116">Application</span></span>|<span data-ttu-id="14ed9-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="14ed9-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="14ed9-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="14ed9-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses
POST /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/deviceStatuses
```

## <a name="request-headers"></a><span data-ttu-id="14ed9-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="14ed9-119">Request headers</span></span>
|<span data-ttu-id="14ed9-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="14ed9-120">Header</span></span>|<span data-ttu-id="14ed9-121">Valor</span><span class="sxs-lookup"><span data-stu-id="14ed9-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="14ed9-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="14ed9-122">Authorization</span></span>|<span data-ttu-id="14ed9-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="14ed9-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="14ed9-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="14ed9-124">Accept</span></span>|<span data-ttu-id="14ed9-125">application/json</span><span class="sxs-lookup"><span data-stu-id="14ed9-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="14ed9-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="14ed9-126">Request body</span></span>
<span data-ttu-id="14ed9-127">No corpo da solicitação, forneça uma representação JSON do objeto mobileAppInstallStatus.</span><span class="sxs-lookup"><span data-stu-id="14ed9-127">In the request body, supply a JSON representation for the mobileAppInstallStatus object.</span></span>

<span data-ttu-id="14ed9-128">A tabela a seguir mostra as propriedades que são necessárias ao criar mobileAppInstallStatus.</span><span class="sxs-lookup"><span data-stu-id="14ed9-128">The following table shows the properties that are required when you create the mobileAppInstallStatus.</span></span>

|<span data-ttu-id="14ed9-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="14ed9-129">Property</span></span>|<span data-ttu-id="14ed9-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="14ed9-130">Type</span></span>|<span data-ttu-id="14ed9-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="14ed9-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="14ed9-132">id</span><span class="sxs-lookup"><span data-stu-id="14ed9-132">id</span></span>|<span data-ttu-id="14ed9-133">String</span><span class="sxs-lookup"><span data-stu-id="14ed9-133">String</span></span>|<span data-ttu-id="14ed9-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="14ed9-134">Key of the entity.</span></span>|
|<span data-ttu-id="14ed9-135">deviceName</span><span class="sxs-lookup"><span data-stu-id="14ed9-135">deviceName</span></span>|<span data-ttu-id="14ed9-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="14ed9-136">String</span></span>|<span data-ttu-id="14ed9-137">Nome do dispositivo</span><span class="sxs-lookup"><span data-stu-id="14ed9-137">Device name</span></span>|
|<span data-ttu-id="14ed9-138">deviceId</span><span class="sxs-lookup"><span data-stu-id="14ed9-138">deviceId</span></span>|<span data-ttu-id="14ed9-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="14ed9-139">String</span></span>|<span data-ttu-id="14ed9-140">ID do dispositivo</span><span class="sxs-lookup"><span data-stu-id="14ed9-140">Device ID</span></span>|
|<span data-ttu-id="14ed9-141">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="14ed9-141">lastSyncDateTime</span></span>|<span data-ttu-id="14ed9-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="14ed9-142">DateTimeOffset</span></span>|<span data-ttu-id="14ed9-143">Hora da data da última sincronização</span><span class="sxs-lookup"><span data-stu-id="14ed9-143">Last sync date time</span></span>|
|<span data-ttu-id="14ed9-144">mobileAppInstallStatusValue</span><span class="sxs-lookup"><span data-stu-id="14ed9-144">mobileAppInstallStatusValue</span></span>|[<span data-ttu-id="14ed9-145">resultantAppState</span><span class="sxs-lookup"><span data-stu-id="14ed9-145">resultantAppState</span></span>](../resources/intune-shared-resultantappstate.md)|<span data-ttu-id="14ed9-146">O estado de instalação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="14ed9-146">The install state of the app.</span></span> <span data-ttu-id="14ed9-147">Os valores possíveis são: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span><span class="sxs-lookup"><span data-stu-id="14ed9-147">Possible values are: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span></span>|
|<span data-ttu-id="14ed9-148">installState</span><span class="sxs-lookup"><span data-stu-id="14ed9-148">installState</span></span>|[<span data-ttu-id="14ed9-149">resultantAppState</span><span class="sxs-lookup"><span data-stu-id="14ed9-149">resultantAppState</span></span>](../resources/intune-shared-resultantappstate.md)|<span data-ttu-id="14ed9-150">O estado de instalação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="14ed9-150">The install state of the app.</span></span> <span data-ttu-id="14ed9-151">Os valores possíveis são: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span><span class="sxs-lookup"><span data-stu-id="14ed9-151">Possible values are: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span></span>|
|<span data-ttu-id="14ed9-152">installStateDetail</span><span class="sxs-lookup"><span data-stu-id="14ed9-152">installStateDetail</span></span>|[<span data-ttu-id="14ed9-153">resultantAppStateDetail</span><span class="sxs-lookup"><span data-stu-id="14ed9-153">resultantAppStateDetail</span></span>](../resources/intune-apps-resultantappstatedetail.md)|<span data-ttu-id="14ed9-154">Os detalhes do estado de instalação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="14ed9-154">The install state detail of the app.</span></span> <span data-ttu-id="14ed9-155">Os valores possíveis são `noAdditionalDetails`: `dependencyFailedToInstall`, `dependencyWithRequirementsNotMet`, `dependencyPendingReboot`, `dependencyWithAutoInstallDisabled`, `seeInstallErrorCode`, `autoInstallDisabled`, `seeUninstallErrorCode`, `pendingReboot`, `installingDependencies` `powerShellScriptRequirementNotMet` `registryRequirementNotMet`,,, `fileSystemRequirementNotMet`, `platformNotApplicable`, `minimumCpuSpeedNotMet`, `minimumLogicalProcessorCountNotMet`, `minimumPhysicalMemoryNotMet`, `minimumOsVersionNotMet`, `minimumDiskSpaceNotMet` ,,,,,,,, , `processorArchitectureNotApplicable`.</span><span class="sxs-lookup"><span data-stu-id="14ed9-155">Possible values are: `noAdditionalDetails`, `dependencyFailedToInstall`, `dependencyWithRequirementsNotMet`, `dependencyPendingReboot`, `dependencyWithAutoInstallDisabled`, `seeInstallErrorCode`, `autoInstallDisabled`, `seeUninstallErrorCode`, `pendingReboot`, `installingDependencies`, `powerShellScriptRequirementNotMet`, `registryRequirementNotMet`, `fileSystemRequirementNotMet`, `platformNotApplicable`, `minimumCpuSpeedNotMet`, `minimumLogicalProcessorCountNotMet`, `minimumPhysicalMemoryNotMet`, `minimumOsVersionNotMet`, `minimumDiskSpaceNotMet`, `processorArchitectureNotApplicable`.</span></span>|
|<span data-ttu-id="14ed9-156">errorCode</span><span class="sxs-lookup"><span data-stu-id="14ed9-156">errorCode</span></span>|<span data-ttu-id="14ed9-157">Int32</span><span class="sxs-lookup"><span data-stu-id="14ed9-157">Int32</span></span>|<span data-ttu-id="14ed9-158">O código de erro para instalação ou desinstalação de falhas.</span><span class="sxs-lookup"><span data-stu-id="14ed9-158">The error code for install or uninstall failures.</span></span>|
|<span data-ttu-id="14ed9-159">osVersion</span><span class="sxs-lookup"><span data-stu-id="14ed9-159">osVersion</span></span>|<span data-ttu-id="14ed9-160">String</span><span class="sxs-lookup"><span data-stu-id="14ed9-160">String</span></span>|<span data-ttu-id="14ed9-161">Versão do sistema operacional</span><span class="sxs-lookup"><span data-stu-id="14ed9-161">OS Version</span></span>|
|<span data-ttu-id="14ed9-162">osDescription</span><span class="sxs-lookup"><span data-stu-id="14ed9-162">osDescription</span></span>|<span data-ttu-id="14ed9-163">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="14ed9-163">String</span></span>|<span data-ttu-id="14ed9-164">Descrição do sistema operacional</span><span class="sxs-lookup"><span data-stu-id="14ed9-164">OS Description</span></span>|
|<span data-ttu-id="14ed9-165">userName</span><span class="sxs-lookup"><span data-stu-id="14ed9-165">userName</span></span>|<span data-ttu-id="14ed9-166">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="14ed9-166">String</span></span>|<span data-ttu-id="14ed9-167">Nome de usuário do dispositivo</span><span class="sxs-lookup"><span data-stu-id="14ed9-167">Device User Name</span></span>|
|<span data-ttu-id="14ed9-168">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="14ed9-168">userPrincipalName</span></span>|<span data-ttu-id="14ed9-169">String</span><span class="sxs-lookup"><span data-stu-id="14ed9-169">String</span></span>|<span data-ttu-id="14ed9-170">Nome UPN</span><span class="sxs-lookup"><span data-stu-id="14ed9-170">User Principal Name</span></span>|
|<span data-ttu-id="14ed9-171">displayVersion</span><span class="sxs-lookup"><span data-stu-id="14ed9-171">displayVersion</span></span>|<span data-ttu-id="14ed9-172">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="14ed9-172">String</span></span>|<span data-ttu-id="14ed9-173">Versão de leitura humana do aplicativo</span><span class="sxs-lookup"><span data-stu-id="14ed9-173">Human readable version of the application</span></span>|



## <a name="response"></a><span data-ttu-id="14ed9-174">Resposta</span><span class="sxs-lookup"><span data-stu-id="14ed9-174">Response</span></span>
<span data-ttu-id="14ed9-175">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="14ed9-175">If successful, this method returns a `201 Created` response code and a [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="14ed9-176">Exemplo</span><span class="sxs-lookup"><span data-stu-id="14ed9-176">Example</span></span>

### <a name="request"></a><span data-ttu-id="14ed9-177">Solicitação</span><span class="sxs-lookup"><span data-stu-id="14ed9-177">Request</span></span>
<span data-ttu-id="14ed9-178">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="14ed9-178">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="14ed9-179">Resposta</span><span class="sxs-lookup"><span data-stu-id="14ed9-179">Response</span></span>
<span data-ttu-id="14ed9-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="14ed9-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





