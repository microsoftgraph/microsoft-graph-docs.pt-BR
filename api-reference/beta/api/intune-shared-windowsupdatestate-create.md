---
title: Criar windowsUpdateState
description: Criar um novo objeto windowsUpdateState.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 32f3bd844ad028a894eeacdf0cc5a052053fa124
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37199522"
---
# <a name="create-windowsupdatestate"></a><span data-ttu-id="04163-103">Criar windowsUpdateState</span><span class="sxs-lookup"><span data-stu-id="04163-103">Create windowsUpdateState</span></span>

> <span data-ttu-id="04163-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="04163-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="04163-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="04163-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="04163-106">Criar um novo objeto [windowsUpdateState](../resources/intune-shared-windowsupdatestate.md) .</span><span class="sxs-lookup"><span data-stu-id="04163-106">Create a new [windowsUpdateState](../resources/intune-shared-windowsupdatestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="04163-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="04163-107">Prerequisites</span></span>
<span data-ttu-id="04163-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="04163-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="04163-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="04163-110">Permission type</span></span>|<span data-ttu-id="04163-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="04163-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="04163-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="04163-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="04163-113">&nbsp; &nbsp; **Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="04163-113">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="04163-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="04163-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
| <span data-ttu-id="04163-115">&nbsp;&nbsp; **Atualização de software**</span><span class="sxs-lookup"><span data-stu-id="04163-115">&nbsp; &nbsp; **Software Update**</span></span> | <span data-ttu-id="04163-116">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="04163-116">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="04163-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="04163-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="04163-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="04163-118">Not supported.</span></span>|
|<span data-ttu-id="04163-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="04163-119">Application</span></span>||
| <span data-ttu-id="04163-120">&nbsp; &nbsp; **Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="04163-120">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="04163-121">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="04163-121">DeviceManagementConfiguration.ReadWrite.All</span></span>|
| <span data-ttu-id="04163-122">&nbsp;&nbsp; **Atualização de software**</span><span class="sxs-lookup"><span data-stu-id="04163-122">&nbsp; &nbsp; **Software Update**</span></span> | <span data-ttu-id="04163-123">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="04163-123">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="04163-124">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="04163-124">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsUpdateForBusinessConfiguration/deviceUpdateStates
```

## <a name="request-headers"></a><span data-ttu-id="04163-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="04163-125">Request headers</span></span>
|<span data-ttu-id="04163-126">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="04163-126">Header</span></span>|<span data-ttu-id="04163-127">Valor</span><span class="sxs-lookup"><span data-stu-id="04163-127">Value</span></span>|
|:---|:---|
|<span data-ttu-id="04163-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="04163-128">Authorization</span></span>|<span data-ttu-id="04163-129">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="04163-129">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="04163-130">Aceitar</span><span class="sxs-lookup"><span data-stu-id="04163-130">Accept</span></span>|<span data-ttu-id="04163-131">application/json</span><span class="sxs-lookup"><span data-stu-id="04163-131">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="04163-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="04163-132">Request body</span></span>
<span data-ttu-id="04163-133">No corpo da solicitação, forneça uma representação JSON do objeto windowsUpdateState.</span><span class="sxs-lookup"><span data-stu-id="04163-133">In the request body, supply a JSON representation for the windowsUpdateState object.</span></span>

<span data-ttu-id="04163-134">A tabela a seguir mostra as propriedades que são necessárias ao criar windowsUpdateState.</span><span class="sxs-lookup"><span data-stu-id="04163-134">The following table shows the properties that are required when you create the windowsUpdateState.</span></span>

|<span data-ttu-id="04163-135">Propriedade</span><span class="sxs-lookup"><span data-stu-id="04163-135">Property</span></span>|<span data-ttu-id="04163-136">Tipo</span><span class="sxs-lookup"><span data-stu-id="04163-136">Type</span></span>|<span data-ttu-id="04163-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="04163-137">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="04163-138">id</span><span class="sxs-lookup"><span data-stu-id="04163-138">id</span></span>|<span data-ttu-id="04163-139">String</span><span class="sxs-lookup"><span data-stu-id="04163-139">String</span></span>|<span data-ttu-id="04163-140">Esta é a ID da entidade.</span><span class="sxs-lookup"><span data-stu-id="04163-140">This is Id of the entity.</span></span>|
|<span data-ttu-id="04163-141">deviceId</span><span class="sxs-lookup"><span data-stu-id="04163-141">deviceId</span></span>|<span data-ttu-id="04163-142">String</span><span class="sxs-lookup"><span data-stu-id="04163-142">String</span></span>|<span data-ttu-id="04163-143">A ID do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="04163-143">The id of the device.</span></span>|
|<span data-ttu-id="04163-144">userId</span><span class="sxs-lookup"><span data-stu-id="04163-144">userId</span></span>|<span data-ttu-id="04163-145">String</span><span class="sxs-lookup"><span data-stu-id="04163-145">String</span></span>|<span data-ttu-id="04163-146">A ID do usuário.</span><span class="sxs-lookup"><span data-stu-id="04163-146">The id of the user.</span></span>|
|<span data-ttu-id="04163-147">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="04163-147">deviceDisplayName</span></span>|<span data-ttu-id="04163-148">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="04163-148">String</span></span>|<span data-ttu-id="04163-149">Nome de exibição do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="04163-149">Device display name.</span></span>|
|<span data-ttu-id="04163-150">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="04163-150">userPrincipalName</span></span>|<span data-ttu-id="04163-151">String</span><span class="sxs-lookup"><span data-stu-id="04163-151">String</span></span>|<span data-ttu-id="04163-152">Nome principal do usuário.</span><span class="sxs-lookup"><span data-stu-id="04163-152">User principal name.</span></span>|
|<span data-ttu-id="04163-153">status</span><span class="sxs-lookup"><span data-stu-id="04163-153">status</span></span>|[<span data-ttu-id="04163-154">windowsUpdateStatus</span><span class="sxs-lookup"><span data-stu-id="04163-154">windowsUpdateStatus</span></span>](../resources/intune-shared-windowsupdatestatus.md)|<span data-ttu-id="04163-155">Status do Windows UDPATE.</span><span class="sxs-lookup"><span data-stu-id="04163-155">Windows udpate status.</span></span> <span data-ttu-id="04163-156">Os valores possíveis são: `upToDate`, `pendingInstallation`, `pendingReboot`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="04163-156">Possible values are: `upToDate`, `pendingInstallation`, `pendingReboot`, `failed`.</span></span>|
|<span data-ttu-id="04163-157">qualityUpdateVersion</span><span class="sxs-lookup"><span data-stu-id="04163-157">qualityUpdateVersion</span></span>|<span data-ttu-id="04163-158">String</span><span class="sxs-lookup"><span data-stu-id="04163-158">String</span></span>|<span data-ttu-id="04163-159">A versão de atualização de qualidade do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="04163-159">The Quality Update Version of the device.</span></span>|
|<span data-ttu-id="04163-160">featureUpdateVersion</span><span class="sxs-lookup"><span data-stu-id="04163-160">featureUpdateVersion</span></span>|<span data-ttu-id="04163-161">String</span><span class="sxs-lookup"><span data-stu-id="04163-161">String</span></span>|<span data-ttu-id="04163-162">A versão atual de atualização de recursos do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="04163-162">The current feature update version of the device.</span></span>|
|<span data-ttu-id="04163-163">lastScanDateTime</span><span class="sxs-lookup"><span data-stu-id="04163-163">lastScanDateTime</span></span>|<span data-ttu-id="04163-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="04163-164">DateTimeOffset</span></span>|<span data-ttu-id="04163-165">A data e hora em que o agente do Windows Update realizou uma verificação bem-sucedida.</span><span class="sxs-lookup"><span data-stu-id="04163-165">The date time that the Windows Update Agent did a successful scan.</span></span>|
|<span data-ttu-id="04163-166">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="04163-166">lastSyncDateTime</span></span>|<span data-ttu-id="04163-167">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="04163-167">DateTimeOffset</span></span>|<span data-ttu-id="04163-168">Data e hora da última sincronização do dispositivo com o Microsoft Intune.</span><span class="sxs-lookup"><span data-stu-id="04163-168">Last date time that the device sync with with Microsoft Intune.</span></span>|



## <a name="response"></a><span data-ttu-id="04163-169">Resposta</span><span class="sxs-lookup"><span data-stu-id="04163-169">Response</span></span>
<span data-ttu-id="04163-170">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [windowsUpdateState](../resources/intune-shared-windowsupdatestate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="04163-170">If successful, this method returns a `201 Created` response code and a [windowsUpdateState](../resources/intune-shared-windowsupdatestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="04163-171">Exemplo</span><span class="sxs-lookup"><span data-stu-id="04163-171">Example</span></span>

### <a name="request"></a><span data-ttu-id="04163-172">Solicitação</span><span class="sxs-lookup"><span data-stu-id="04163-172">Request</span></span>
<span data-ttu-id="04163-173">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="04163-173">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsUpdateForBusinessConfiguration/deviceUpdateStates
Content-type: application/json
Content-length: 504

{
  "@odata.type": "#microsoft.graph.windowsUpdateState",
  "deviceId": "Device Id value",
  "userId": "User Id value",
  "deviceDisplayName": "Device Display Name value",
  "userPrincipalName": "User Principal Name value",
  "status": "pendingInstallation",
  "qualityUpdateVersion": "Quality Update Version value",
  "featureUpdateVersion": "Feature Update Version value",
  "lastScanDateTime": "2016-12-31T23:59:18.0955018-08:00",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00"
}
```

### <a name="response"></a><span data-ttu-id="04163-174">Resposta</span><span class="sxs-lookup"><span data-stu-id="04163-174">Response</span></span>
<span data-ttu-id="04163-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="04163-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 553

{
  "@odata.type": "#microsoft.graph.windowsUpdateState",
  "id": "3d92af00-af00-3d92-00af-923d00af923d",
  "deviceId": "Device Id value",
  "userId": "User Id value",
  "deviceDisplayName": "Device Display Name value",
  "userPrincipalName": "User Principal Name value",
  "status": "pendingInstallation",
  "qualityUpdateVersion": "Quality Update Version value",
  "featureUpdateVersion": "Feature Update Version value",
  "lastScanDateTime": "2016-12-31T23:59:18.0955018-08:00",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00"
}
```




