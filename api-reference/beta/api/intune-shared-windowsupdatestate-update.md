---
title: Atualizar windowsUpdateState
description: Atualiza as propriedades de um objeto windowsUpdateState.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 47021216905227509d2c97c38cbfa464764e79af
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39939308"
---
# <a name="update-windowsupdatestate"></a><span data-ttu-id="52b4e-103">Atualizar windowsUpdateState</span><span class="sxs-lookup"><span data-stu-id="52b4e-103">Update windowsUpdateState</span></span>

> <span data-ttu-id="52b4e-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="52b4e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="52b4e-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="52b4e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="52b4e-106">Atualiza as propriedades de um objeto [windowsUpdateState](../resources/intune-shared-windowsupdatestate.md) .</span><span class="sxs-lookup"><span data-stu-id="52b4e-106">Update the properties of a [windowsUpdateState](../resources/intune-shared-windowsupdatestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="52b4e-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="52b4e-107">Prerequisites</span></span>
<span data-ttu-id="52b4e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="52b4e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="52b4e-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="52b4e-110">Permission type</span></span>|<span data-ttu-id="52b4e-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="52b4e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="52b4e-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="52b4e-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="52b4e-113">&nbsp; &nbsp; **Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="52b4e-113">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="52b4e-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="52b4e-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
| <span data-ttu-id="52b4e-115">&nbsp;&nbsp; **Atualização de software**</span><span class="sxs-lookup"><span data-stu-id="52b4e-115">&nbsp; &nbsp; **Software Update**</span></span> | <span data-ttu-id="52b4e-116">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="52b4e-116">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="52b4e-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="52b4e-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="52b4e-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="52b4e-118">Not supported.</span></span>|
|<span data-ttu-id="52b4e-119">Application</span><span class="sxs-lookup"><span data-stu-id="52b4e-119">Application</span></span>||
| <span data-ttu-id="52b4e-120">&nbsp; &nbsp; **Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="52b4e-120">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="52b4e-121">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="52b4e-121">DeviceManagementConfiguration.ReadWrite.All</span></span>|
| <span data-ttu-id="52b4e-122">&nbsp;&nbsp; **Atualização de software**</span><span class="sxs-lookup"><span data-stu-id="52b4e-122">&nbsp; &nbsp; **Software Update**</span></span> | <span data-ttu-id="52b4e-123">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="52b4e-123">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="52b4e-124">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="52b4e-124">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsUpdateForBusinessConfiguration/deviceUpdateStates/{windowsUpdateStateId}
```

## <a name="request-headers"></a><span data-ttu-id="52b4e-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="52b4e-125">Request headers</span></span>
|<span data-ttu-id="52b4e-126">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="52b4e-126">Header</span></span>|<span data-ttu-id="52b4e-127">Valor</span><span class="sxs-lookup"><span data-stu-id="52b4e-127">Value</span></span>|
|:---|:---|
|<span data-ttu-id="52b4e-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="52b4e-128">Authorization</span></span>|<span data-ttu-id="52b4e-129">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="52b4e-129">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="52b4e-130">Aceitar</span><span class="sxs-lookup"><span data-stu-id="52b4e-130">Accept</span></span>|<span data-ttu-id="52b4e-131">application/json</span><span class="sxs-lookup"><span data-stu-id="52b4e-131">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="52b4e-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="52b4e-132">Request body</span></span>
<span data-ttu-id="52b4e-133">No corpo da solicitação, forneça uma representação JSON do objeto [windowsUpdateState](../resources/intune-shared-windowsupdatestate.md) .</span><span class="sxs-lookup"><span data-stu-id="52b4e-133">In the request body, supply a JSON representation for the [windowsUpdateState](../resources/intune-shared-windowsupdatestate.md) object.</span></span>

<span data-ttu-id="52b4e-134">A tabela a seguir mostra as propriedades que são necessárias ao criar [windowsUpdateState](../resources/intune-shared-windowsupdatestate.md).</span><span class="sxs-lookup"><span data-stu-id="52b4e-134">The following table shows the properties that are required when you create the [windowsUpdateState](../resources/intune-shared-windowsupdatestate.md).</span></span>

|<span data-ttu-id="52b4e-135">Propriedade</span><span class="sxs-lookup"><span data-stu-id="52b4e-135">Property</span></span>|<span data-ttu-id="52b4e-136">Tipo</span><span class="sxs-lookup"><span data-stu-id="52b4e-136">Type</span></span>|<span data-ttu-id="52b4e-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="52b4e-137">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="52b4e-138">id</span><span class="sxs-lookup"><span data-stu-id="52b4e-138">id</span></span>|<span data-ttu-id="52b4e-139">String</span><span class="sxs-lookup"><span data-stu-id="52b4e-139">String</span></span>|<span data-ttu-id="52b4e-140">Esta é a ID da entidade.</span><span class="sxs-lookup"><span data-stu-id="52b4e-140">This is Id of the entity.</span></span>|
|<span data-ttu-id="52b4e-141">deviceId</span><span class="sxs-lookup"><span data-stu-id="52b4e-141">deviceId</span></span>|<span data-ttu-id="52b4e-142">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="52b4e-142">String</span></span>|<span data-ttu-id="52b4e-143">A ID do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="52b4e-143">The id of the device.</span></span>|
|<span data-ttu-id="52b4e-144">userId</span><span class="sxs-lookup"><span data-stu-id="52b4e-144">userId</span></span>|<span data-ttu-id="52b4e-145">String</span><span class="sxs-lookup"><span data-stu-id="52b4e-145">String</span></span>|<span data-ttu-id="52b4e-146">A ID do usuário.</span><span class="sxs-lookup"><span data-stu-id="52b4e-146">The id of the user.</span></span>|
|<span data-ttu-id="52b4e-147">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="52b4e-147">deviceDisplayName</span></span>|<span data-ttu-id="52b4e-148">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="52b4e-148">String</span></span>|<span data-ttu-id="52b4e-149">Nome de exibição do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="52b4e-149">Device display name.</span></span>|
|<span data-ttu-id="52b4e-150">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="52b4e-150">userPrincipalName</span></span>|<span data-ttu-id="52b4e-151">String</span><span class="sxs-lookup"><span data-stu-id="52b4e-151">String</span></span>|<span data-ttu-id="52b4e-152">Nome principal do usuário.</span><span class="sxs-lookup"><span data-stu-id="52b4e-152">User principal name.</span></span>|
|<span data-ttu-id="52b4e-153">status</span><span class="sxs-lookup"><span data-stu-id="52b4e-153">status</span></span>|[<span data-ttu-id="52b4e-154">windowsUpdateStatus</span><span class="sxs-lookup"><span data-stu-id="52b4e-154">windowsUpdateStatus</span></span>](../resources/intune-shared-windowsupdatestatus.md)|<span data-ttu-id="52b4e-155">Status do Windows UDPATE.</span><span class="sxs-lookup"><span data-stu-id="52b4e-155">Windows udpate status.</span></span> <span data-ttu-id="52b4e-156">Os valores possíveis são: `upToDate`, `pendingInstallation`, `pendingReboot`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="52b4e-156">Possible values are: `upToDate`, `pendingInstallation`, `pendingReboot`, `failed`.</span></span>|
|<span data-ttu-id="52b4e-157">qualityUpdateVersion</span><span class="sxs-lookup"><span data-stu-id="52b4e-157">qualityUpdateVersion</span></span>|<span data-ttu-id="52b4e-158">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="52b4e-158">String</span></span>|<span data-ttu-id="52b4e-159">A versão de atualização de qualidade do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="52b4e-159">The Quality Update Version of the device.</span></span>|
|<span data-ttu-id="52b4e-160">featureUpdateVersion</span><span class="sxs-lookup"><span data-stu-id="52b4e-160">featureUpdateVersion</span></span>|<span data-ttu-id="52b4e-161">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="52b4e-161">String</span></span>|<span data-ttu-id="52b4e-162">A versão atual de atualização de recursos do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="52b4e-162">The current feature update version of the device.</span></span>|
|<span data-ttu-id="52b4e-163">lastScanDateTime</span><span class="sxs-lookup"><span data-stu-id="52b4e-163">lastScanDateTime</span></span>|<span data-ttu-id="52b4e-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="52b4e-164">DateTimeOffset</span></span>|<span data-ttu-id="52b4e-165">A data e hora em que o agente do Windows Update realizou uma verificação bem-sucedida.</span><span class="sxs-lookup"><span data-stu-id="52b4e-165">The date time that the Windows Update Agent did a successful scan.</span></span>|
|<span data-ttu-id="52b4e-166">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="52b4e-166">lastSyncDateTime</span></span>|<span data-ttu-id="52b4e-167">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="52b4e-167">DateTimeOffset</span></span>|<span data-ttu-id="52b4e-168">Data e hora da última sincronização do dispositivo com o Microsoft Intune.</span><span class="sxs-lookup"><span data-stu-id="52b4e-168">Last date time that the device sync with with Microsoft Intune.</span></span>|



## <a name="response"></a><span data-ttu-id="52b4e-169">Resposta</span><span class="sxs-lookup"><span data-stu-id="52b4e-169">Response</span></span>
<span data-ttu-id="52b4e-170">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [windowsUpdateState](../resources/intune-shared-windowsupdatestate.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="52b4e-170">If successful, this method returns a `200 OK` response code and an updated [windowsUpdateState](../resources/intune-shared-windowsupdatestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="52b4e-171">Exemplo</span><span class="sxs-lookup"><span data-stu-id="52b4e-171">Example</span></span>

### <a name="request"></a><span data-ttu-id="52b4e-172">Solicitação</span><span class="sxs-lookup"><span data-stu-id="52b4e-172">Request</span></span>
<span data-ttu-id="52b4e-173">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="52b4e-173">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsUpdateForBusinessConfiguration/deviceUpdateStates/{windowsUpdateStateId}
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

### <a name="response"></a><span data-ttu-id="52b4e-174">Resposta</span><span class="sxs-lookup"><span data-stu-id="52b4e-174">Response</span></span>
<span data-ttu-id="52b4e-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="52b4e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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








