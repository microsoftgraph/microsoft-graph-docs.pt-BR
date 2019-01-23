---
title: Criar mobileAppInstallStatus
description: Crie um novo objeto de mobileAppInstallStatus.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 123a07d7b7576bfc94011e20d45a6d0c8e65abc0
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29394191"
---
# <a name="create-mobileappinstallstatus"></a><span data-ttu-id="89784-103">Criar mobileAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="89784-103">Create mobileAppInstallStatus</span></span>

> <span data-ttu-id="89784-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="89784-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="89784-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="89784-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="89784-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="89784-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="89784-107">Crie um novo objeto de [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) .</span><span class="sxs-lookup"><span data-stu-id="89784-107">Create a new [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="89784-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="89784-108">Prerequisites</span></span>
<span data-ttu-id="89784-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="89784-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="89784-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="89784-111">Permission type</span></span>|<span data-ttu-id="89784-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="89784-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="89784-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="89784-113">Delegated (work or school account)</span></span>|<span data-ttu-id="89784-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="89784-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="89784-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="89784-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="89784-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="89784-116">Not supported.</span></span>|
|<span data-ttu-id="89784-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="89784-117">Application</span></span>|<span data-ttu-id="89784-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="89784-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="89784-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="89784-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses
POST /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/deviceStatuses
```

## <a name="request-headers"></a><span data-ttu-id="89784-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="89784-120">Request headers</span></span>
|<span data-ttu-id="89784-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="89784-121">Header</span></span>|<span data-ttu-id="89784-122">Valor</span><span class="sxs-lookup"><span data-stu-id="89784-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="89784-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="89784-123">Authorization</span></span>|<span data-ttu-id="89784-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="89784-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="89784-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="89784-125">Accept</span></span>|<span data-ttu-id="89784-126">application/json</span><span class="sxs-lookup"><span data-stu-id="89784-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="89784-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="89784-127">Request body</span></span>
<span data-ttu-id="89784-128">No corpo da solicitação, fornece uma representação JSON para o objeto mobileAppInstallStatus.</span><span class="sxs-lookup"><span data-stu-id="89784-128">In the request body, supply a JSON representation for the mobileAppInstallStatus object.</span></span>

<span data-ttu-id="89784-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o mobileAppInstallStatus.</span><span class="sxs-lookup"><span data-stu-id="89784-129">The following table shows the properties that are required when you create the mobileAppInstallStatus.</span></span>

|<span data-ttu-id="89784-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="89784-130">Property</span></span>|<span data-ttu-id="89784-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="89784-131">Type</span></span>|<span data-ttu-id="89784-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="89784-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="89784-133">id</span><span class="sxs-lookup"><span data-stu-id="89784-133">id</span></span>|<span data-ttu-id="89784-134">String</span><span class="sxs-lookup"><span data-stu-id="89784-134">String</span></span>|<span data-ttu-id="89784-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="89784-135">Key of the entity.</span></span>|
|<span data-ttu-id="89784-136">deviceName</span><span class="sxs-lookup"><span data-stu-id="89784-136">deviceName</span></span>|<span data-ttu-id="89784-137">String</span><span class="sxs-lookup"><span data-stu-id="89784-137">String</span></span>|<span data-ttu-id="89784-138">Nome do dispositivo</span><span class="sxs-lookup"><span data-stu-id="89784-138">Device name</span></span>|
|<span data-ttu-id="89784-139">deviceId</span><span class="sxs-lookup"><span data-stu-id="89784-139">deviceId</span></span>|<span data-ttu-id="89784-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="89784-140">String</span></span>|<span data-ttu-id="89784-141">ID do dispositivo</span><span class="sxs-lookup"><span data-stu-id="89784-141">Device ID</span></span>|
|<span data-ttu-id="89784-142">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="89784-142">lastSyncDateTime</span></span>|<span data-ttu-id="89784-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="89784-143">DateTimeOffset</span></span>|<span data-ttu-id="89784-144">Última sincronização data hora</span><span class="sxs-lookup"><span data-stu-id="89784-144">Last sync date time</span></span>|
|<span data-ttu-id="89784-145">mobileAppInstallStatusValue</span><span class="sxs-lookup"><span data-stu-id="89784-145">mobileAppInstallStatusValue</span></span>|[<span data-ttu-id="89784-146">resultantAppState</span><span class="sxs-lookup"><span data-stu-id="89784-146">resultantAppState</span></span>](../resources/intune-shared-resultantappstate.md)|<span data-ttu-id="89784-147">O estado de instalação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="89784-147">The install state of the app.</span></span> <span data-ttu-id="89784-148">Os valores possíveis são: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span><span class="sxs-lookup"><span data-stu-id="89784-148">Possible values are: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span></span>|
|<span data-ttu-id="89784-149">installState</span><span class="sxs-lookup"><span data-stu-id="89784-149">installState</span></span>|[<span data-ttu-id="89784-150">resultantAppState</span><span class="sxs-lookup"><span data-stu-id="89784-150">resultantAppState</span></span>](../resources/intune-shared-resultantappstate.md)|<span data-ttu-id="89784-151">O estado de instalação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="89784-151">The install state of the app.</span></span> <span data-ttu-id="89784-152">Os valores possíveis são: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span><span class="sxs-lookup"><span data-stu-id="89784-152">Possible values are: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span></span>|
|<span data-ttu-id="89784-153">installStateDetail</span><span class="sxs-lookup"><span data-stu-id="89784-153">installStateDetail</span></span>|[<span data-ttu-id="89784-154">resultantAppStateDetail</span><span class="sxs-lookup"><span data-stu-id="89784-154">resultantAppStateDetail</span></span>](../resources/intune-apps-resultantappstatedetail.md)|<span data-ttu-id="89784-155">Os detalhes de estado de instalação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="89784-155">The install state detail of the app.</span></span> <span data-ttu-id="89784-156">Os valores possíveis são: `noAdditionalDetails`, `seeInstallErrorCode`, `seeUninstallErrorCode`, `pendingReboot`, `platformNotApplicable`, `minimumCpuSpeedNotMet`, `minimumLogicalProcessorCountNotMet`, `minimumPhysicalMemoryNotMet`, `minimumOsVersionNotMet`, `minimumDiskSpaceNotMet`, `processorArchitectureNotApplicable`.</span><span class="sxs-lookup"><span data-stu-id="89784-156">Possible values are: `noAdditionalDetails`, `seeInstallErrorCode`, `seeUninstallErrorCode`, `pendingReboot`, `platformNotApplicable`, `minimumCpuSpeedNotMet`, `minimumLogicalProcessorCountNotMet`, `minimumPhysicalMemoryNotMet`, `minimumOsVersionNotMet`, `minimumDiskSpaceNotMet`, `processorArchitectureNotApplicable`.</span></span>|
|<span data-ttu-id="89784-157">errorCode</span><span class="sxs-lookup"><span data-stu-id="89784-157">errorCode</span></span>|<span data-ttu-id="89784-158">Int32</span><span class="sxs-lookup"><span data-stu-id="89784-158">Int32</span></span>|<span data-ttu-id="89784-159">O erro de código para instalar ou desinstalar falhas.</span><span class="sxs-lookup"><span data-stu-id="89784-159">The error code for install or uninstall failures.</span></span>|
|<span data-ttu-id="89784-160">osVersion</span><span class="sxs-lookup"><span data-stu-id="89784-160">osVersion</span></span>|<span data-ttu-id="89784-161">String</span><span class="sxs-lookup"><span data-stu-id="89784-161">String</span></span>|<span data-ttu-id="89784-162">Versão do sistema operacional</span><span class="sxs-lookup"><span data-stu-id="89784-162">OS Version</span></span>|
|<span data-ttu-id="89784-163">osDescription</span><span class="sxs-lookup"><span data-stu-id="89784-163">osDescription</span></span>|<span data-ttu-id="89784-164">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="89784-164">String</span></span>|<span data-ttu-id="89784-165">Descrição do sistema operacional</span><span class="sxs-lookup"><span data-stu-id="89784-165">OS Description</span></span>|
|<span data-ttu-id="89784-166">userName</span><span class="sxs-lookup"><span data-stu-id="89784-166">userName</span></span>|<span data-ttu-id="89784-167">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="89784-167">String</span></span>|<span data-ttu-id="89784-168">Nome de usuário do dispositivo</span><span class="sxs-lookup"><span data-stu-id="89784-168">Device User Name</span></span>|
|<span data-ttu-id="89784-169">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="89784-169">userPrincipalName</span></span>|<span data-ttu-id="89784-170">String</span><span class="sxs-lookup"><span data-stu-id="89784-170">String</span></span>|<span data-ttu-id="89784-171">Nome UPN</span><span class="sxs-lookup"><span data-stu-id="89784-171">User Principal Name</span></span>|
|<span data-ttu-id="89784-172">displayVersion</span><span class="sxs-lookup"><span data-stu-id="89784-172">displayVersion</span></span>|<span data-ttu-id="89784-173">String</span><span class="sxs-lookup"><span data-stu-id="89784-173">String</span></span>|<span data-ttu-id="89784-174">Versão legível humana do aplicativo</span><span class="sxs-lookup"><span data-stu-id="89784-174">Human readable version of the application</span></span>|



## <a name="response"></a><span data-ttu-id="89784-175">Resposta</span><span class="sxs-lookup"><span data-stu-id="89784-175">Response</span></span>
<span data-ttu-id="89784-176">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="89784-176">If successful, this method returns a `201 Created` response code and a [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="89784-177">Exemplo</span><span class="sxs-lookup"><span data-stu-id="89784-177">Example</span></span>

### <a name="request"></a><span data-ttu-id="89784-178">Solicitação</span><span class="sxs-lookup"><span data-stu-id="89784-178">Request</span></span>
<span data-ttu-id="89784-179">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="89784-179">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="89784-180">Resposta</span><span class="sxs-lookup"><span data-stu-id="89784-180">Response</span></span>
<span data-ttu-id="89784-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="89784-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




