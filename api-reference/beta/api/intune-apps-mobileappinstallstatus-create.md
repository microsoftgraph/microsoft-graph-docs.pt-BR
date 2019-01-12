---
title: Criar mobileAppInstallStatus
description: Crie um novo objeto de mobileAppInstallStatus.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: eb2425ee773068eea2446b19534f907f48a43fe5
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27970763"
---
# <a name="create-mobileappinstallstatus"></a><span data-ttu-id="7706b-103">Criar mobileAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="7706b-103">Create mobileAppInstallStatus</span></span>

> <span data-ttu-id="7706b-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="7706b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7706b-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="7706b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7706b-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="7706b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7706b-107">Crie um novo objeto de [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) .</span><span class="sxs-lookup"><span data-stu-id="7706b-107">Create a new [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="7706b-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="7706b-108">Prerequisites</span></span>
<span data-ttu-id="7706b-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7706b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7706b-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7706b-111">Permission type</span></span>|<span data-ttu-id="7706b-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="7706b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7706b-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7706b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7706b-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7706b-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="7706b-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7706b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7706b-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7706b-116">Not supported.</span></span>|
|<span data-ttu-id="7706b-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7706b-117">Application</span></span>|<span data-ttu-id="7706b-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7706b-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7706b-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7706b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses
POST /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/deviceStatuses
```

## <a name="request-headers"></a><span data-ttu-id="7706b-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7706b-120">Request headers</span></span>
|<span data-ttu-id="7706b-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="7706b-121">Header</span></span>|<span data-ttu-id="7706b-122">Valor</span><span class="sxs-lookup"><span data-stu-id="7706b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7706b-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="7706b-123">Authorization</span></span>|<span data-ttu-id="7706b-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7706b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7706b-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="7706b-125">Accept</span></span>|<span data-ttu-id="7706b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7706b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7706b-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7706b-127">Request body</span></span>
<span data-ttu-id="7706b-128">No corpo da solicitação, fornece uma representação JSON para o objeto mobileAppInstallStatus.</span><span class="sxs-lookup"><span data-stu-id="7706b-128">In the request body, supply a JSON representation for the mobileAppInstallStatus object.</span></span>

<span data-ttu-id="7706b-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o mobileAppInstallStatus.</span><span class="sxs-lookup"><span data-stu-id="7706b-129">The following table shows the properties that are required when you create the mobileAppInstallStatus.</span></span>

|<span data-ttu-id="7706b-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7706b-130">Property</span></span>|<span data-ttu-id="7706b-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="7706b-131">Type</span></span>|<span data-ttu-id="7706b-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="7706b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7706b-133">id</span><span class="sxs-lookup"><span data-stu-id="7706b-133">id</span></span>|<span data-ttu-id="7706b-134">String</span><span class="sxs-lookup"><span data-stu-id="7706b-134">String</span></span>|<span data-ttu-id="7706b-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="7706b-135">Key of the entity.</span></span>|
|<span data-ttu-id="7706b-136">deviceName</span><span class="sxs-lookup"><span data-stu-id="7706b-136">deviceName</span></span>|<span data-ttu-id="7706b-137">String</span><span class="sxs-lookup"><span data-stu-id="7706b-137">String</span></span>|<span data-ttu-id="7706b-138">Nome do dispositivo</span><span class="sxs-lookup"><span data-stu-id="7706b-138">Device name</span></span>|
|<span data-ttu-id="7706b-139">deviceId</span><span class="sxs-lookup"><span data-stu-id="7706b-139">deviceId</span></span>|<span data-ttu-id="7706b-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7706b-140">String</span></span>|<span data-ttu-id="7706b-141">ID do dispositivo</span><span class="sxs-lookup"><span data-stu-id="7706b-141">Device ID</span></span>|
|<span data-ttu-id="7706b-142">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="7706b-142">lastSyncDateTime</span></span>|<span data-ttu-id="7706b-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7706b-143">DateTimeOffset</span></span>|<span data-ttu-id="7706b-144">Última sincronização data hora</span><span class="sxs-lookup"><span data-stu-id="7706b-144">Last sync date time</span></span>|
|<span data-ttu-id="7706b-145">mobileAppInstallStatusValue</span><span class="sxs-lookup"><span data-stu-id="7706b-145">mobileAppInstallStatusValue</span></span>|[<span data-ttu-id="7706b-146">resultantAppState</span><span class="sxs-lookup"><span data-stu-id="7706b-146">resultantAppState</span></span>](../resources/intune-shared-resultantappstate.md)|<span data-ttu-id="7706b-147">O estado de instalação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="7706b-147">The install state of the app.</span></span> <span data-ttu-id="7706b-148">Os valores possíveis são: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span><span class="sxs-lookup"><span data-stu-id="7706b-148">Possible values are: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span></span>|
|<span data-ttu-id="7706b-149">installState</span><span class="sxs-lookup"><span data-stu-id="7706b-149">installState</span></span>|[<span data-ttu-id="7706b-150">resultantAppState</span><span class="sxs-lookup"><span data-stu-id="7706b-150">resultantAppState</span></span>](../resources/intune-shared-resultantappstate.md)|<span data-ttu-id="7706b-151">O estado de instalação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="7706b-151">The install state of the app.</span></span> <span data-ttu-id="7706b-152">Os valores possíveis são: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span><span class="sxs-lookup"><span data-stu-id="7706b-152">Possible values are: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span></span>|
|<span data-ttu-id="7706b-153">installStateDetail</span><span class="sxs-lookup"><span data-stu-id="7706b-153">installStateDetail</span></span>|[<span data-ttu-id="7706b-154">resultantAppStateDetail</span><span class="sxs-lookup"><span data-stu-id="7706b-154">resultantAppStateDetail</span></span>](../resources/intune-apps-resultantappstatedetail.md)|<span data-ttu-id="7706b-155">Os detalhes de estado de instalação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="7706b-155">The install state detail of the app.</span></span> <span data-ttu-id="7706b-156">Os valores possíveis são: `noAdditionalDetails`, `seeInstallErrorCode`, `seeUninstallErrorCode`, `pendingReboot`, `platformNotApplicable`, `minimumCpuSpeedNotMet`, `minimumLogicalProcessorCountNotMet`, `minimumPhysicalMemoryNotMet`, `minimumOsVersionNotMet`, `minimumDiskSpaceNotMet`, `processorArchitectureNotApplicable`.</span><span class="sxs-lookup"><span data-stu-id="7706b-156">Possible values are: `noAdditionalDetails`, `seeInstallErrorCode`, `seeUninstallErrorCode`, `pendingReboot`, `platformNotApplicable`, `minimumCpuSpeedNotMet`, `minimumLogicalProcessorCountNotMet`, `minimumPhysicalMemoryNotMet`, `minimumOsVersionNotMet`, `minimumDiskSpaceNotMet`, `processorArchitectureNotApplicable`.</span></span>|
|<span data-ttu-id="7706b-157">errorCode</span><span class="sxs-lookup"><span data-stu-id="7706b-157">errorCode</span></span>|<span data-ttu-id="7706b-158">Int32</span><span class="sxs-lookup"><span data-stu-id="7706b-158">Int32</span></span>|<span data-ttu-id="7706b-159">O erro de código para instalar ou desinstalar falhas.</span><span class="sxs-lookup"><span data-stu-id="7706b-159">The error code for install or uninstall failures.</span></span>|
|<span data-ttu-id="7706b-160">osVersion</span><span class="sxs-lookup"><span data-stu-id="7706b-160">osVersion</span></span>|<span data-ttu-id="7706b-161">String</span><span class="sxs-lookup"><span data-stu-id="7706b-161">String</span></span>|<span data-ttu-id="7706b-162">Versão do sistema operacional</span><span class="sxs-lookup"><span data-stu-id="7706b-162">OS Version</span></span>|
|<span data-ttu-id="7706b-163">osDescription</span><span class="sxs-lookup"><span data-stu-id="7706b-163">osDescription</span></span>|<span data-ttu-id="7706b-164">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7706b-164">String</span></span>|<span data-ttu-id="7706b-165">Descrição do sistema operacional</span><span class="sxs-lookup"><span data-stu-id="7706b-165">OS Description</span></span>|
|<span data-ttu-id="7706b-166">userName</span><span class="sxs-lookup"><span data-stu-id="7706b-166">userName</span></span>|<span data-ttu-id="7706b-167">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7706b-167">String</span></span>|<span data-ttu-id="7706b-168">Nome de usuário do dispositivo</span><span class="sxs-lookup"><span data-stu-id="7706b-168">Device User Name</span></span>|
|<span data-ttu-id="7706b-169">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="7706b-169">userPrincipalName</span></span>|<span data-ttu-id="7706b-170">String</span><span class="sxs-lookup"><span data-stu-id="7706b-170">String</span></span>|<span data-ttu-id="7706b-171">Nome UPN</span><span class="sxs-lookup"><span data-stu-id="7706b-171">User Principal Name</span></span>|
|<span data-ttu-id="7706b-172">displayVersion</span><span class="sxs-lookup"><span data-stu-id="7706b-172">displayVersion</span></span>|<span data-ttu-id="7706b-173">String</span><span class="sxs-lookup"><span data-stu-id="7706b-173">String</span></span>|<span data-ttu-id="7706b-174">Versão legível humana do aplicativo</span><span class="sxs-lookup"><span data-stu-id="7706b-174">Human readable version of the application</span></span>|



## <a name="response"></a><span data-ttu-id="7706b-175">Resposta</span><span class="sxs-lookup"><span data-stu-id="7706b-175">Response</span></span>
<span data-ttu-id="7706b-176">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7706b-176">If successful, this method returns a `201 Created` response code and a [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7706b-177">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7706b-177">Example</span></span>
### <a name="request"></a><span data-ttu-id="7706b-178">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7706b-178">Request</span></span>
<span data-ttu-id="7706b-179">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7706b-179">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="7706b-180">Resposta</span><span class="sxs-lookup"><span data-stu-id="7706b-180">Response</span></span>
<span data-ttu-id="7706b-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7706b-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





