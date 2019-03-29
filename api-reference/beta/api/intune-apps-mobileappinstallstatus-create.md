---
title: Criar mobileAppInstallStatus
description: Criar um novo objeto mobileAppInstallStatus.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 13fae27ccc022ce8795d787dbd86923d71e2ab24
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/29/2019
ms.locfileid: "30969887"
---
# <a name="create-mobileappinstallstatus"></a><span data-ttu-id="b2543-103">Criar mobileAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="b2543-103">Create mobileAppInstallStatus</span></span>

> <span data-ttu-id="b2543-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b2543-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b2543-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b2543-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b2543-106">Criar um novo objeto [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) .</span><span class="sxs-lookup"><span data-stu-id="b2543-106">Create a new [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b2543-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b2543-107">Prerequisites</span></span>
<span data-ttu-id="b2543-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b2543-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b2543-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b2543-110">Permission type</span></span>|<span data-ttu-id="b2543-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b2543-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b2543-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b2543-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b2543-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b2543-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="b2543-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b2543-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b2543-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b2543-115">Not supported.</span></span>|
|<span data-ttu-id="b2543-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b2543-116">Application</span></span>|<span data-ttu-id="b2543-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b2543-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b2543-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b2543-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses
POST /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/deviceStatuses
```

## <a name="request-headers"></a><span data-ttu-id="b2543-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b2543-119">Request headers</span></span>
|<span data-ttu-id="b2543-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b2543-120">Header</span></span>|<span data-ttu-id="b2543-121">Valor</span><span class="sxs-lookup"><span data-stu-id="b2543-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b2543-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="b2543-122">Authorization</span></span>|<span data-ttu-id="b2543-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b2543-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b2543-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b2543-124">Accept</span></span>|<span data-ttu-id="b2543-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b2543-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b2543-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b2543-126">Request body</span></span>
<span data-ttu-id="b2543-127">No corpo da solicitação, forneça uma representação JSON do objeto mobileAppInstallStatus.</span><span class="sxs-lookup"><span data-stu-id="b2543-127">In the request body, supply a JSON representation for the mobileAppInstallStatus object.</span></span>

<span data-ttu-id="b2543-128">A tabela a seguir mostra as propriedades que são necessárias ao criar mobileAppInstallStatus.</span><span class="sxs-lookup"><span data-stu-id="b2543-128">The following table shows the properties that are required when you create the mobileAppInstallStatus.</span></span>

|<span data-ttu-id="b2543-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b2543-129">Property</span></span>|<span data-ttu-id="b2543-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="b2543-130">Type</span></span>|<span data-ttu-id="b2543-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="b2543-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b2543-132">id</span><span class="sxs-lookup"><span data-stu-id="b2543-132">id</span></span>|<span data-ttu-id="b2543-133">String</span><span class="sxs-lookup"><span data-stu-id="b2543-133">String</span></span>|<span data-ttu-id="b2543-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="b2543-134">Key of the entity.</span></span>|
|<span data-ttu-id="b2543-135">deviceName</span><span class="sxs-lookup"><span data-stu-id="b2543-135">deviceName</span></span>|<span data-ttu-id="b2543-136">String</span><span class="sxs-lookup"><span data-stu-id="b2543-136">String</span></span>|<span data-ttu-id="b2543-137">Nome do dispositivo</span><span class="sxs-lookup"><span data-stu-id="b2543-137">Device name</span></span>|
|<span data-ttu-id="b2543-138">deviceId</span><span class="sxs-lookup"><span data-stu-id="b2543-138">deviceId</span></span>|<span data-ttu-id="b2543-139">String</span><span class="sxs-lookup"><span data-stu-id="b2543-139">String</span></span>|<span data-ttu-id="b2543-140">ID do dispositivo</span><span class="sxs-lookup"><span data-stu-id="b2543-140">Device ID</span></span>|
|<span data-ttu-id="b2543-141">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="b2543-141">lastSyncDateTime</span></span>|<span data-ttu-id="b2543-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b2543-142">DateTimeOffset</span></span>|<span data-ttu-id="b2543-143">Hora da data da última sincronização</span><span class="sxs-lookup"><span data-stu-id="b2543-143">Last sync date time</span></span>|
|<span data-ttu-id="b2543-144">mobileAppInstallStatusValue</span><span class="sxs-lookup"><span data-stu-id="b2543-144">mobileAppInstallStatusValue</span></span>|[<span data-ttu-id="b2543-145">resultantAppState</span><span class="sxs-lookup"><span data-stu-id="b2543-145">resultantAppState</span></span>](../resources/intune-shared-resultantappstate.md)|<span data-ttu-id="b2543-146">O estado de instalação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b2543-146">The install state of the app.</span></span> <span data-ttu-id="b2543-147">Os valores possíveis são: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span><span class="sxs-lookup"><span data-stu-id="b2543-147">Possible values are: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span></span>|
|<span data-ttu-id="b2543-148">installState</span><span class="sxs-lookup"><span data-stu-id="b2543-148">installState</span></span>|[<span data-ttu-id="b2543-149">resultantAppState</span><span class="sxs-lookup"><span data-stu-id="b2543-149">resultantAppState</span></span>](../resources/intune-shared-resultantappstate.md)|<span data-ttu-id="b2543-150">O estado de instalação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b2543-150">The install state of the app.</span></span> <span data-ttu-id="b2543-151">Os valores possíveis são: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span><span class="sxs-lookup"><span data-stu-id="b2543-151">Possible values are: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span></span>|
|<span data-ttu-id="b2543-152">installStateDetail</span><span class="sxs-lookup"><span data-stu-id="b2543-152">installStateDetail</span></span>|[<span data-ttu-id="b2543-153">resultantAppStateDetail</span><span class="sxs-lookup"><span data-stu-id="b2543-153">resultantAppStateDetail</span></span>](../resources/intune-apps-resultantappstatedetail.md)|<span data-ttu-id="b2543-154">Os detalhes do estado de instalação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b2543-154">The install state detail of the app.</span></span> <span data-ttu-id="b2543-155">Os valores possíveis são: `noAdditionalDetails`, `seeInstallErrorCode`, `seeUninstallErrorCode`, `pendingReboot`, `platformNotApplicable`, `minimumCpuSpeedNotMet`, `minimumLogicalProcessorCountNotMet`, `minimumPhysicalMemoryNotMet`, `minimumOsVersionNotMet`, `minimumDiskSpaceNotMet`, `processorArchitectureNotApplicable`.</span><span class="sxs-lookup"><span data-stu-id="b2543-155">Possible values are: `noAdditionalDetails`, `seeInstallErrorCode`, `seeUninstallErrorCode`, `pendingReboot`, `platformNotApplicable`, `minimumCpuSpeedNotMet`, `minimumLogicalProcessorCountNotMet`, `minimumPhysicalMemoryNotMet`, `minimumOsVersionNotMet`, `minimumDiskSpaceNotMet`, `processorArchitectureNotApplicable`.</span></span>|
|<span data-ttu-id="b2543-156">errorCode</span><span class="sxs-lookup"><span data-stu-id="b2543-156">errorCode</span></span>|<span data-ttu-id="b2543-157">Int32</span><span class="sxs-lookup"><span data-stu-id="b2543-157">Int32</span></span>|<span data-ttu-id="b2543-158">O código de erro para instalação ou desinstalação de falhas.</span><span class="sxs-lookup"><span data-stu-id="b2543-158">The error code for install or uninstall failures.</span></span>|
|<span data-ttu-id="b2543-159">osVersion</span><span class="sxs-lookup"><span data-stu-id="b2543-159">osVersion</span></span>|<span data-ttu-id="b2543-160">String</span><span class="sxs-lookup"><span data-stu-id="b2543-160">String</span></span>|<span data-ttu-id="b2543-161">Versão do sistema operacional</span><span class="sxs-lookup"><span data-stu-id="b2543-161">OS Version</span></span>|
|<span data-ttu-id="b2543-162">osDescription</span><span class="sxs-lookup"><span data-stu-id="b2543-162">osDescription</span></span>|<span data-ttu-id="b2543-163">String</span><span class="sxs-lookup"><span data-stu-id="b2543-163">String</span></span>|<span data-ttu-id="b2543-164">Descrição do sistema operacional</span><span class="sxs-lookup"><span data-stu-id="b2543-164">OS Description</span></span>|
|<span data-ttu-id="b2543-165">userName</span><span class="sxs-lookup"><span data-stu-id="b2543-165">userName</span></span>|<span data-ttu-id="b2543-166">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b2543-166">String</span></span>|<span data-ttu-id="b2543-167">Nome de usuário do dispositivo</span><span class="sxs-lookup"><span data-stu-id="b2543-167">Device User Name</span></span>|
|<span data-ttu-id="b2543-168">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="b2543-168">userPrincipalName</span></span>|<span data-ttu-id="b2543-169">String</span><span class="sxs-lookup"><span data-stu-id="b2543-169">String</span></span>|<span data-ttu-id="b2543-170">Nome UPN</span><span class="sxs-lookup"><span data-stu-id="b2543-170">User Principal Name</span></span>|
|<span data-ttu-id="b2543-171">displayVersion</span><span class="sxs-lookup"><span data-stu-id="b2543-171">displayVersion</span></span>|<span data-ttu-id="b2543-172">String</span><span class="sxs-lookup"><span data-stu-id="b2543-172">String</span></span>|<span data-ttu-id="b2543-173">Versão de leitura humana do aplicativo</span><span class="sxs-lookup"><span data-stu-id="b2543-173">Human readable version of the application</span></span>|



## <a name="response"></a><span data-ttu-id="b2543-174">Resposta</span><span class="sxs-lookup"><span data-stu-id="b2543-174">Response</span></span>
<span data-ttu-id="b2543-175">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b2543-175">If successful, this method returns a `201 Created` response code and a [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b2543-176">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b2543-176">Example</span></span>

### <a name="request"></a><span data-ttu-id="b2543-177">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b2543-177">Request</span></span>
<span data-ttu-id="b2543-178">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b2543-178">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="b2543-179">Resposta</span><span class="sxs-lookup"><span data-stu-id="b2543-179">Response</span></span>
<span data-ttu-id="b2543-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b2543-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




