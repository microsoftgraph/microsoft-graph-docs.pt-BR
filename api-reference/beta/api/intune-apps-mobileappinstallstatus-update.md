---
title: Atualizar mobileAppInstallStatus
description: Atualiza as propriedades de um objeto mobileAppInstallStatus.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b4c10190f7cc675b5444a6238060703b852d44b4
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34973751"
---
# <a name="update-mobileappinstallstatus"></a><span data-ttu-id="10bcb-103">Atualizar mobileAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="10bcb-103">Update mobileAppInstallStatus</span></span>

> <span data-ttu-id="10bcb-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="10bcb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="10bcb-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="10bcb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="10bcb-106">Atualiza as propriedades de um objeto [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) .</span><span class="sxs-lookup"><span data-stu-id="10bcb-106">Update the properties of a [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="10bcb-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="10bcb-107">Prerequisites</span></span>
<span data-ttu-id="10bcb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="10bcb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="10bcb-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="10bcb-110">Permission type</span></span>|<span data-ttu-id="10bcb-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="10bcb-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="10bcb-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="10bcb-112">Delegated (work or school account)</span></span>|<span data-ttu-id="10bcb-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="10bcb-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="10bcb-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="10bcb-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="10bcb-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="10bcb-115">Not supported.</span></span>|
|<span data-ttu-id="10bcb-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="10bcb-116">Application</span></span>|<span data-ttu-id="10bcb-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="10bcb-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="10bcb-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="10bcb-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/deviceStatuses/{mobileAppInstallStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="10bcb-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="10bcb-119">Request headers</span></span>
|<span data-ttu-id="10bcb-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="10bcb-120">Header</span></span>|<span data-ttu-id="10bcb-121">Valor</span><span class="sxs-lookup"><span data-stu-id="10bcb-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="10bcb-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="10bcb-122">Authorization</span></span>|<span data-ttu-id="10bcb-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="10bcb-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="10bcb-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="10bcb-124">Accept</span></span>|<span data-ttu-id="10bcb-125">application/json</span><span class="sxs-lookup"><span data-stu-id="10bcb-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="10bcb-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="10bcb-126">Request body</span></span>
<span data-ttu-id="10bcb-127">No corpo da solicitação, forneça uma representação JSON do objeto [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) .</span><span class="sxs-lookup"><span data-stu-id="10bcb-127">In the request body, supply a JSON representation for the [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) object.</span></span>

<span data-ttu-id="10bcb-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md).</span><span class="sxs-lookup"><span data-stu-id="10bcb-128">The following table shows the properties that are required when you create the [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md).</span></span>

|<span data-ttu-id="10bcb-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="10bcb-129">Property</span></span>|<span data-ttu-id="10bcb-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="10bcb-130">Type</span></span>|<span data-ttu-id="10bcb-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="10bcb-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="10bcb-132">id</span><span class="sxs-lookup"><span data-stu-id="10bcb-132">id</span></span>|<span data-ttu-id="10bcb-133">String</span><span class="sxs-lookup"><span data-stu-id="10bcb-133">String</span></span>|<span data-ttu-id="10bcb-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="10bcb-134">Key of the entity.</span></span>|
|<span data-ttu-id="10bcb-135">deviceName</span><span class="sxs-lookup"><span data-stu-id="10bcb-135">deviceName</span></span>|<span data-ttu-id="10bcb-136">String</span><span class="sxs-lookup"><span data-stu-id="10bcb-136">String</span></span>|<span data-ttu-id="10bcb-137">Nome do dispositivo</span><span class="sxs-lookup"><span data-stu-id="10bcb-137">Device name</span></span>|
|<span data-ttu-id="10bcb-138">deviceId</span><span class="sxs-lookup"><span data-stu-id="10bcb-138">deviceId</span></span>|<span data-ttu-id="10bcb-139">String</span><span class="sxs-lookup"><span data-stu-id="10bcb-139">String</span></span>|<span data-ttu-id="10bcb-140">ID do dispositivo</span><span class="sxs-lookup"><span data-stu-id="10bcb-140">Device ID</span></span>|
|<span data-ttu-id="10bcb-141">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="10bcb-141">lastSyncDateTime</span></span>|<span data-ttu-id="10bcb-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="10bcb-142">DateTimeOffset</span></span>|<span data-ttu-id="10bcb-143">Hora da data da última sincronização</span><span class="sxs-lookup"><span data-stu-id="10bcb-143">Last sync date time</span></span>|
|<span data-ttu-id="10bcb-144">mobileAppInstallStatusValue</span><span class="sxs-lookup"><span data-stu-id="10bcb-144">mobileAppInstallStatusValue</span></span>|[<span data-ttu-id="10bcb-145">resultantAppState</span><span class="sxs-lookup"><span data-stu-id="10bcb-145">resultantAppState</span></span>](../resources/intune-shared-resultantappstate.md)|<span data-ttu-id="10bcb-146">O estado de instalação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="10bcb-146">The install state of the app.</span></span> <span data-ttu-id="10bcb-147">Os valores possíveis são: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span><span class="sxs-lookup"><span data-stu-id="10bcb-147">Possible values are: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span></span>|
|<span data-ttu-id="10bcb-148">installState</span><span class="sxs-lookup"><span data-stu-id="10bcb-148">installState</span></span>|[<span data-ttu-id="10bcb-149">resultantAppState</span><span class="sxs-lookup"><span data-stu-id="10bcb-149">resultantAppState</span></span>](../resources/intune-shared-resultantappstate.md)|<span data-ttu-id="10bcb-150">O estado de instalação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="10bcb-150">The install state of the app.</span></span> <span data-ttu-id="10bcb-151">Os valores possíveis são: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span><span class="sxs-lookup"><span data-stu-id="10bcb-151">Possible values are: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span></span>|
|<span data-ttu-id="10bcb-152">installStateDetail</span><span class="sxs-lookup"><span data-stu-id="10bcb-152">installStateDetail</span></span>|[<span data-ttu-id="10bcb-153">resultantAppStateDetail</span><span class="sxs-lookup"><span data-stu-id="10bcb-153">resultantAppStateDetail</span></span>](../resources/intune-apps-resultantappstatedetail.md)|<span data-ttu-id="10bcb-154">Os detalhes do estado de instalação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="10bcb-154">The install state detail of the app.</span></span> <span data-ttu-id="10bcb-155">Os valores possíveis são `noAdditionalDetails`: `dependencyFailedToInstall`, `dependencyWithRequirementsNotMet`, `dependencyPendingReboot`, `dependencyWithAutoInstallDisabled`, `seeInstallErrorCode`, `autoInstallDisabled`, `seeUninstallErrorCode`, `pendingReboot`, `installingDependencies` `powerShellScriptRequirementNotMet` `registryRequirementNotMet`,,, `fileSystemRequirementNotMet`, `platformNotApplicable`, `minimumCpuSpeedNotMet`, `minimumLogicalProcessorCountNotMet`, `minimumPhysicalMemoryNotMet`, `minimumOsVersionNotMet`, `minimumDiskSpaceNotMet` ,,,,,,,, , `processorArchitectureNotApplicable`.</span><span class="sxs-lookup"><span data-stu-id="10bcb-155">Possible values are: `noAdditionalDetails`, `dependencyFailedToInstall`, `dependencyWithRequirementsNotMet`, `dependencyPendingReboot`, `dependencyWithAutoInstallDisabled`, `seeInstallErrorCode`, `autoInstallDisabled`, `seeUninstallErrorCode`, `pendingReboot`, `installingDependencies`, `powerShellScriptRequirementNotMet`, `registryRequirementNotMet`, `fileSystemRequirementNotMet`, `platformNotApplicable`, `minimumCpuSpeedNotMet`, `minimumLogicalProcessorCountNotMet`, `minimumPhysicalMemoryNotMet`, `minimumOsVersionNotMet`, `minimumDiskSpaceNotMet`, `processorArchitectureNotApplicable`.</span></span>|
|<span data-ttu-id="10bcb-156">errorCode</span><span class="sxs-lookup"><span data-stu-id="10bcb-156">errorCode</span></span>|<span data-ttu-id="10bcb-157">Int32</span><span class="sxs-lookup"><span data-stu-id="10bcb-157">Int32</span></span>|<span data-ttu-id="10bcb-158">O código de erro para instalação ou desinstalação de falhas.</span><span class="sxs-lookup"><span data-stu-id="10bcb-158">The error code for install or uninstall failures.</span></span>|
|<span data-ttu-id="10bcb-159">osVersion</span><span class="sxs-lookup"><span data-stu-id="10bcb-159">osVersion</span></span>|<span data-ttu-id="10bcb-160">String</span><span class="sxs-lookup"><span data-stu-id="10bcb-160">String</span></span>|<span data-ttu-id="10bcb-161">Versão do sistema operacional</span><span class="sxs-lookup"><span data-stu-id="10bcb-161">OS Version</span></span>|
|<span data-ttu-id="10bcb-162">osDescription</span><span class="sxs-lookup"><span data-stu-id="10bcb-162">osDescription</span></span>|<span data-ttu-id="10bcb-163">String</span><span class="sxs-lookup"><span data-stu-id="10bcb-163">String</span></span>|<span data-ttu-id="10bcb-164">Descrição do sistema operacional</span><span class="sxs-lookup"><span data-stu-id="10bcb-164">OS Description</span></span>|
|<span data-ttu-id="10bcb-165">userName</span><span class="sxs-lookup"><span data-stu-id="10bcb-165">userName</span></span>|<span data-ttu-id="10bcb-166">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="10bcb-166">String</span></span>|<span data-ttu-id="10bcb-167">Nome de usuário do dispositivo</span><span class="sxs-lookup"><span data-stu-id="10bcb-167">Device User Name</span></span>|
|<span data-ttu-id="10bcb-168">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="10bcb-168">userPrincipalName</span></span>|<span data-ttu-id="10bcb-169">String</span><span class="sxs-lookup"><span data-stu-id="10bcb-169">String</span></span>|<span data-ttu-id="10bcb-170">Nome UPN</span><span class="sxs-lookup"><span data-stu-id="10bcb-170">User Principal Name</span></span>|
|<span data-ttu-id="10bcb-171">displayVersion</span><span class="sxs-lookup"><span data-stu-id="10bcb-171">displayVersion</span></span>|<span data-ttu-id="10bcb-172">String</span><span class="sxs-lookup"><span data-stu-id="10bcb-172">String</span></span>|<span data-ttu-id="10bcb-173">Versão de leitura humana do aplicativo</span><span class="sxs-lookup"><span data-stu-id="10bcb-173">Human readable version of the application</span></span>|



## <a name="response"></a><span data-ttu-id="10bcb-174">Resposta</span><span class="sxs-lookup"><span data-stu-id="10bcb-174">Response</span></span>
<span data-ttu-id="10bcb-175">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="10bcb-175">If successful, this method returns a `200 OK` response code and an updated [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="10bcb-176">Exemplo</span><span class="sxs-lookup"><span data-stu-id="10bcb-176">Example</span></span>

### <a name="request"></a><span data-ttu-id="10bcb-177">Solicitação</span><span class="sxs-lookup"><span data-stu-id="10bcb-177">Request</span></span>
<span data-ttu-id="10bcb-178">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="10bcb-178">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="10bcb-179">Resposta</span><span class="sxs-lookup"><span data-stu-id="10bcb-179">Response</span></span>
<span data-ttu-id="10bcb-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="10bcb-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





