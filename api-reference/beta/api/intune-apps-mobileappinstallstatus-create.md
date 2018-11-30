---
title: Criar mobileAppInstallStatus
description: Crie um novo objeto de mobileAppInstallStatus.
ms.openlocfilehash: 5aba88a33b5072f1426878eeaf32a0771ee250b7
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27037348"
---
# <a name="create-mobileappinstallstatus"></a><span data-ttu-id="a180c-103">Criar mobileAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="a180c-103">Create mobileAppInstallStatus</span></span>

> <span data-ttu-id="a180c-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="a180c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a180c-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="a180c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a180c-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="a180c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a180c-107">Crie um novo objeto de [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) .</span><span class="sxs-lookup"><span data-stu-id="a180c-107">Create a new [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a180c-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a180c-108">Prerequisites</span></span>
<span data-ttu-id="a180c-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a180c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a180c-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a180c-111">Permission type</span></span>|<span data-ttu-id="a180c-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a180c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a180c-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a180c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a180c-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a180c-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="a180c-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a180c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a180c-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a180c-116">Not supported.</span></span>|
|<span data-ttu-id="a180c-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a180c-117">Application</span></span>|<span data-ttu-id="a180c-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a180c-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a180c-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a180c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses
POST /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/deviceStatuses
```

## <a name="request-headers"></a><span data-ttu-id="a180c-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a180c-120">Request headers</span></span>
|<span data-ttu-id="a180c-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a180c-121">Header</span></span>|<span data-ttu-id="a180c-122">Valor</span><span class="sxs-lookup"><span data-stu-id="a180c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a180c-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="a180c-123">Authorization</span></span>|<span data-ttu-id="a180c-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a180c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a180c-125">Accept</span><span class="sxs-lookup"><span data-stu-id="a180c-125">Accept</span></span>|<span data-ttu-id="a180c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a180c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a180c-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a180c-127">Request body</span></span>
<span data-ttu-id="a180c-128">No corpo da solicitação, fornece uma representação JSON para o objeto mobileAppInstallStatus.</span><span class="sxs-lookup"><span data-stu-id="a180c-128">In the request body, supply a JSON representation for the mobileAppInstallStatus object.</span></span>

<span data-ttu-id="a180c-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o mobileAppInstallStatus.</span><span class="sxs-lookup"><span data-stu-id="a180c-129">The following table shows the properties that are required when you create the mobileAppInstallStatus.</span></span>

|<span data-ttu-id="a180c-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a180c-130">Property</span></span>|<span data-ttu-id="a180c-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="a180c-131">Type</span></span>|<span data-ttu-id="a180c-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="a180c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a180c-133">id</span><span class="sxs-lookup"><span data-stu-id="a180c-133">id</span></span>|<span data-ttu-id="a180c-134">String</span><span class="sxs-lookup"><span data-stu-id="a180c-134">String</span></span>|<span data-ttu-id="a180c-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="a180c-135">Key of the entity.</span></span>|
|<span data-ttu-id="a180c-136">deviceName</span><span class="sxs-lookup"><span data-stu-id="a180c-136">deviceName</span></span>|<span data-ttu-id="a180c-137">String</span><span class="sxs-lookup"><span data-stu-id="a180c-137">String</span></span>|<span data-ttu-id="a180c-138">Nome do dispositivo</span><span class="sxs-lookup"><span data-stu-id="a180c-138">Device name</span></span>|
|<span data-ttu-id="a180c-139">deviceId</span><span class="sxs-lookup"><span data-stu-id="a180c-139">deviceId</span></span>|<span data-ttu-id="a180c-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a180c-140">String</span></span>|<span data-ttu-id="a180c-141">ID do dispositivo</span><span class="sxs-lookup"><span data-stu-id="a180c-141">Device ID</span></span>|
|<span data-ttu-id="a180c-142">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="a180c-142">lastSyncDateTime</span></span>|<span data-ttu-id="a180c-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a180c-143">DateTimeOffset</span></span>|<span data-ttu-id="a180c-144">Última sincronização data hora</span><span class="sxs-lookup"><span data-stu-id="a180c-144">Last sync date time</span></span>|
|<span data-ttu-id="a180c-145">mobileAppInstallStatusValue</span><span class="sxs-lookup"><span data-stu-id="a180c-145">mobileAppInstallStatusValue</span></span>|[<span data-ttu-id="a180c-146">resultantAppState</span><span class="sxs-lookup"><span data-stu-id="a180c-146">resultantAppState</span></span>](../resources/intune-shared-resultantappstate.md)|<span data-ttu-id="a180c-147">O estado de instalação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="a180c-147">The install state of the app.</span></span> <span data-ttu-id="a180c-148">Os valores possíveis são: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span><span class="sxs-lookup"><span data-stu-id="a180c-148">Possible values are: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span></span>|
|<span data-ttu-id="a180c-149">installState</span><span class="sxs-lookup"><span data-stu-id="a180c-149">installState</span></span>|[<span data-ttu-id="a180c-150">resultantAppState</span><span class="sxs-lookup"><span data-stu-id="a180c-150">resultantAppState</span></span>](../resources/intune-shared-resultantappstate.md)|<span data-ttu-id="a180c-151">O estado de instalação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="a180c-151">The install state of the app.</span></span> <span data-ttu-id="a180c-152">Os valores possíveis são: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span><span class="sxs-lookup"><span data-stu-id="a180c-152">Possible values are: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span></span>|
|<span data-ttu-id="a180c-153">installStateDetail</span><span class="sxs-lookup"><span data-stu-id="a180c-153">installStateDetail</span></span>|[<span data-ttu-id="a180c-154">resultantAppStateDetail</span><span class="sxs-lookup"><span data-stu-id="a180c-154">resultantAppStateDetail</span></span>](../resources/intune-apps-resultantappstatedetail.md)|<span data-ttu-id="a180c-155">Os detalhes de estado de instalação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="a180c-155">The install state detail of the app.</span></span> <span data-ttu-id="a180c-156">Os valores possíveis são: `noAdditionalDetails`, `seeInstallErrorCode`, `seeUninstallErrorCode`, `pendingReboot`, `platformNotApplicable`, `minimumCpuSpeedNotMet`, `minimumLogicalProcessorCountNotMet`, `minimumPhysicalMemoryNotMet`, `minimumOsVersionNotMet`, `minimumDiskSpaceNotMet`, `processorArchitectureNotApplicable`.</span><span class="sxs-lookup"><span data-stu-id="a180c-156">Possible values are: `noAdditionalDetails`, `seeInstallErrorCode`, `seeUninstallErrorCode`, `pendingReboot`, `platformNotApplicable`, `minimumCpuSpeedNotMet`, `minimumLogicalProcessorCountNotMet`, `minimumPhysicalMemoryNotMet`, `minimumOsVersionNotMet`, `minimumDiskSpaceNotMet`, `processorArchitectureNotApplicable`.</span></span>|
|<span data-ttu-id="a180c-157">errorCode</span><span class="sxs-lookup"><span data-stu-id="a180c-157">errorCode</span></span>|<span data-ttu-id="a180c-158">Int32</span><span class="sxs-lookup"><span data-stu-id="a180c-158">Int32</span></span>|<span data-ttu-id="a180c-159">O erro de código para instalar ou desinstalar falhas.</span><span class="sxs-lookup"><span data-stu-id="a180c-159">The error code for install or uninstall failures.</span></span>|
|<span data-ttu-id="a180c-160">osVersion</span><span class="sxs-lookup"><span data-stu-id="a180c-160">osVersion</span></span>|<span data-ttu-id="a180c-161">String</span><span class="sxs-lookup"><span data-stu-id="a180c-161">String</span></span>|<span data-ttu-id="a180c-162">Versão do sistema operacional</span><span class="sxs-lookup"><span data-stu-id="a180c-162">OS Version</span></span>|
|<span data-ttu-id="a180c-163">osDescription</span><span class="sxs-lookup"><span data-stu-id="a180c-163">osDescription</span></span>|<span data-ttu-id="a180c-164">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a180c-164">String</span></span>|<span data-ttu-id="a180c-165">Descrição do sistema operacional</span><span class="sxs-lookup"><span data-stu-id="a180c-165">OS Description</span></span>|
|<span data-ttu-id="a180c-166">userName</span><span class="sxs-lookup"><span data-stu-id="a180c-166">userName</span></span>|<span data-ttu-id="a180c-167">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a180c-167">String</span></span>|<span data-ttu-id="a180c-168">Nome de usuário do dispositivo</span><span class="sxs-lookup"><span data-stu-id="a180c-168">Device User Name</span></span>|
|<span data-ttu-id="a180c-169">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="a180c-169">userPrincipalName</span></span>|<span data-ttu-id="a180c-170">String</span><span class="sxs-lookup"><span data-stu-id="a180c-170">String</span></span>|<span data-ttu-id="a180c-171">Nome UPN</span><span class="sxs-lookup"><span data-stu-id="a180c-171">User Principal Name</span></span>|
|<span data-ttu-id="a180c-172">displayVersion</span><span class="sxs-lookup"><span data-stu-id="a180c-172">displayVersion</span></span>|<span data-ttu-id="a180c-173">String</span><span class="sxs-lookup"><span data-stu-id="a180c-173">String</span></span>|<span data-ttu-id="a180c-174">Versão legível humana do aplicativo</span><span class="sxs-lookup"><span data-stu-id="a180c-174">Human readable version of the application</span></span>|



## <a name="response"></a><span data-ttu-id="a180c-175">Resposta</span><span class="sxs-lookup"><span data-stu-id="a180c-175">Response</span></span>
<span data-ttu-id="a180c-176">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a180c-176">If successful, this method returns a `201 Created` response code and a [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a180c-177">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a180c-177">Example</span></span>
### <a name="request"></a><span data-ttu-id="a180c-178">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a180c-178">Request</span></span>
<span data-ttu-id="a180c-179">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a180c-179">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="a180c-180">Resposta</span><span class="sxs-lookup"><span data-stu-id="a180c-180">Response</span></span>
<span data-ttu-id="a180c-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a180c-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





