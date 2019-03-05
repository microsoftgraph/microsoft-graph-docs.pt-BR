---
title: Criar mobileAppInstallStatus
description: Criar um novo objeto mobileAppInstallStatus.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 800845615e730c8e9da4573f499728b349121461
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30149837"
---
# <a name="create-mobileappinstallstatus"></a><span data-ttu-id="12a8f-103">Criar mobileAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="12a8f-103">Create mobileAppInstallStatus</span></span>

> <span data-ttu-id="12a8f-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="12a8f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="12a8f-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="12a8f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="12a8f-106">Criar um novo objeto [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) .</span><span class="sxs-lookup"><span data-stu-id="12a8f-106">Create a new [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="12a8f-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="12a8f-107">Prerequisites</span></span>
<span data-ttu-id="12a8f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="12a8f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="12a8f-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="12a8f-110">Permission type</span></span>|<span data-ttu-id="12a8f-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="12a8f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="12a8f-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="12a8f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="12a8f-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="12a8f-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="12a8f-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="12a8f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="12a8f-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="12a8f-115">Not supported.</span></span>|
|<span data-ttu-id="12a8f-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="12a8f-116">Application</span></span>|<span data-ttu-id="12a8f-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="12a8f-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="12a8f-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="12a8f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses
POST /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/deviceStatuses
```

## <a name="request-headers"></a><span data-ttu-id="12a8f-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="12a8f-119">Request headers</span></span>
|<span data-ttu-id="12a8f-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="12a8f-120">Header</span></span>|<span data-ttu-id="12a8f-121">Valor</span><span class="sxs-lookup"><span data-stu-id="12a8f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="12a8f-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="12a8f-122">Authorization</span></span>|<span data-ttu-id="12a8f-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="12a8f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="12a8f-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="12a8f-124">Accept</span></span>|<span data-ttu-id="12a8f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="12a8f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="12a8f-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="12a8f-126">Request body</span></span>
<span data-ttu-id="12a8f-127">No corpo da solicitação, forneça uma representação JSON do objeto mobileAppInstallStatus.</span><span class="sxs-lookup"><span data-stu-id="12a8f-127">In the request body, supply a JSON representation for the mobileAppInstallStatus object.</span></span>

<span data-ttu-id="12a8f-128">A tabela a seguir mostra as propriedades que são necessárias ao criar mobileAppInstallStatus.</span><span class="sxs-lookup"><span data-stu-id="12a8f-128">The following table shows the properties that are required when you create the mobileAppInstallStatus.</span></span>

|<span data-ttu-id="12a8f-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="12a8f-129">Property</span></span>|<span data-ttu-id="12a8f-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="12a8f-130">Type</span></span>|<span data-ttu-id="12a8f-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="12a8f-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="12a8f-132">id</span><span class="sxs-lookup"><span data-stu-id="12a8f-132">id</span></span>|<span data-ttu-id="12a8f-133">String</span><span class="sxs-lookup"><span data-stu-id="12a8f-133">String</span></span>|<span data-ttu-id="12a8f-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="12a8f-134">Key of the entity.</span></span>|
|<span data-ttu-id="12a8f-135">deviceName</span><span class="sxs-lookup"><span data-stu-id="12a8f-135">deviceName</span></span>|<span data-ttu-id="12a8f-136">String</span><span class="sxs-lookup"><span data-stu-id="12a8f-136">String</span></span>|<span data-ttu-id="12a8f-137">Nome do dispositivo</span><span class="sxs-lookup"><span data-stu-id="12a8f-137">Device name</span></span>|
|<span data-ttu-id="12a8f-138">deviceId</span><span class="sxs-lookup"><span data-stu-id="12a8f-138">deviceId</span></span>|<span data-ttu-id="12a8f-139">String</span><span class="sxs-lookup"><span data-stu-id="12a8f-139">String</span></span>|<span data-ttu-id="12a8f-140">ID do dispositivo</span><span class="sxs-lookup"><span data-stu-id="12a8f-140">Device ID</span></span>|
|<span data-ttu-id="12a8f-141">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="12a8f-141">lastSyncDateTime</span></span>|<span data-ttu-id="12a8f-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="12a8f-142">DateTimeOffset</span></span>|<span data-ttu-id="12a8f-143">Hora da data da última sincronização</span><span class="sxs-lookup"><span data-stu-id="12a8f-143">Last sync date time</span></span>|
|<span data-ttu-id="12a8f-144">mobileAppInstallStatusValue</span><span class="sxs-lookup"><span data-stu-id="12a8f-144">mobileAppInstallStatusValue</span></span>|[<span data-ttu-id="12a8f-145">resultantAppState</span><span class="sxs-lookup"><span data-stu-id="12a8f-145">resultantAppState</span></span>](../resources/intune-shared-resultantappstate.md)|<span data-ttu-id="12a8f-146">O estado de instalação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="12a8f-146">The install state of the app.</span></span> <span data-ttu-id="12a8f-147">Os valores possíveis são: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span><span class="sxs-lookup"><span data-stu-id="12a8f-147">Possible values are: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span></span>|
|<span data-ttu-id="12a8f-148">installState</span><span class="sxs-lookup"><span data-stu-id="12a8f-148">installState</span></span>|[<span data-ttu-id="12a8f-149">resultantAppState</span><span class="sxs-lookup"><span data-stu-id="12a8f-149">resultantAppState</span></span>](../resources/intune-shared-resultantappstate.md)|<span data-ttu-id="12a8f-150">O estado de instalação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="12a8f-150">The install state of the app.</span></span> <span data-ttu-id="12a8f-151">Os valores possíveis são: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span><span class="sxs-lookup"><span data-stu-id="12a8f-151">Possible values are: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span></span>|
|<span data-ttu-id="12a8f-152">installStateDetail</span><span class="sxs-lookup"><span data-stu-id="12a8f-152">installStateDetail</span></span>|[<span data-ttu-id="12a8f-153">resultantAppStateDetail</span><span class="sxs-lookup"><span data-stu-id="12a8f-153">resultantAppStateDetail</span></span>](../resources/intune-apps-resultantappstatedetail.md)|<span data-ttu-id="12a8f-154">Os detalhes do estado de instalação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="12a8f-154">The install state detail of the app.</span></span> <span data-ttu-id="12a8f-155">Os valores possíveis são: `noAdditionalDetails`, `seeInstallErrorCode`, `seeUninstallErrorCode`, `pendingReboot`, `platformNotApplicable`, `minimumCpuSpeedNotMet`, `minimumLogicalProcessorCountNotMet`, `minimumPhysicalMemoryNotMet`, `minimumOsVersionNotMet`, `minimumDiskSpaceNotMet`, `processorArchitectureNotApplicable`.</span><span class="sxs-lookup"><span data-stu-id="12a8f-155">Possible values are: `noAdditionalDetails`, `seeInstallErrorCode`, `seeUninstallErrorCode`, `pendingReboot`, `platformNotApplicable`, `minimumCpuSpeedNotMet`, `minimumLogicalProcessorCountNotMet`, `minimumPhysicalMemoryNotMet`, `minimumOsVersionNotMet`, `minimumDiskSpaceNotMet`, `processorArchitectureNotApplicable`.</span></span>|
|<span data-ttu-id="12a8f-156">errorCode</span><span class="sxs-lookup"><span data-stu-id="12a8f-156">errorCode</span></span>|<span data-ttu-id="12a8f-157">Int32</span><span class="sxs-lookup"><span data-stu-id="12a8f-157">Int32</span></span>|<span data-ttu-id="12a8f-158">O código de erro para instalação ou desinstalação de falhas.</span><span class="sxs-lookup"><span data-stu-id="12a8f-158">The error code for install or uninstall failures.</span></span>|
|<span data-ttu-id="12a8f-159">osVersion</span><span class="sxs-lookup"><span data-stu-id="12a8f-159">osVersion</span></span>|<span data-ttu-id="12a8f-160">String</span><span class="sxs-lookup"><span data-stu-id="12a8f-160">String</span></span>|<span data-ttu-id="12a8f-161">Versão do sistema operacional</span><span class="sxs-lookup"><span data-stu-id="12a8f-161">OS Version</span></span>|
|<span data-ttu-id="12a8f-162">osDescription</span><span class="sxs-lookup"><span data-stu-id="12a8f-162">osDescription</span></span>|<span data-ttu-id="12a8f-163">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="12a8f-163">String</span></span>|<span data-ttu-id="12a8f-164">Descrição do sistema operacional</span><span class="sxs-lookup"><span data-stu-id="12a8f-164">OS Description</span></span>|
|<span data-ttu-id="12a8f-165">userName</span><span class="sxs-lookup"><span data-stu-id="12a8f-165">userName</span></span>|<span data-ttu-id="12a8f-166">String</span><span class="sxs-lookup"><span data-stu-id="12a8f-166">String</span></span>|<span data-ttu-id="12a8f-167">Nome de usuário do dispositivo</span><span class="sxs-lookup"><span data-stu-id="12a8f-167">Device User Name</span></span>|
|<span data-ttu-id="12a8f-168">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="12a8f-168">userPrincipalName</span></span>|<span data-ttu-id="12a8f-169">String</span><span class="sxs-lookup"><span data-stu-id="12a8f-169">String</span></span>|<span data-ttu-id="12a8f-170">Nome UPN</span><span class="sxs-lookup"><span data-stu-id="12a8f-170">User Principal Name</span></span>|
|<span data-ttu-id="12a8f-171">displayVersion</span><span class="sxs-lookup"><span data-stu-id="12a8f-171">displayVersion</span></span>|<span data-ttu-id="12a8f-172">String</span><span class="sxs-lookup"><span data-stu-id="12a8f-172">String</span></span>|<span data-ttu-id="12a8f-173">Versão de leitura humana do aplicativo</span><span class="sxs-lookup"><span data-stu-id="12a8f-173">Human readable version of the application</span></span>|



## <a name="response"></a><span data-ttu-id="12a8f-174">Resposta</span><span class="sxs-lookup"><span data-stu-id="12a8f-174">Response</span></span>
<span data-ttu-id="12a8f-175">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="12a8f-175">If successful, this method returns a `201 Created` response code and a [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="12a8f-176">Exemplo</span><span class="sxs-lookup"><span data-stu-id="12a8f-176">Example</span></span>

### <a name="request"></a><span data-ttu-id="12a8f-177">Solicitação</span><span class="sxs-lookup"><span data-stu-id="12a8f-177">Request</span></span>
<span data-ttu-id="12a8f-178">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="12a8f-178">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses
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

### <a name="response"></a><span data-ttu-id="12a8f-179">Resposta</span><span class="sxs-lookup"><span data-stu-id="12a8f-179">Response</span></span>
<span data-ttu-id="12a8f-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="12a8f-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




