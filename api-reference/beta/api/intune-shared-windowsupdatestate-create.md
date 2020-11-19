---
title: Criar windowsUpdateState
description: Criar um novo objeto windowsUpdateState.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 41ac2bafcdcc077080f34fa6c9b87f0a8f9393d9
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49295786"
---
# <a name="create-windowsupdatestate"></a><span data-ttu-id="67a81-103">Criar windowsUpdateState</span><span class="sxs-lookup"><span data-stu-id="67a81-103">Create windowsUpdateState</span></span>

<span data-ttu-id="67a81-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="67a81-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="67a81-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="67a81-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="67a81-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="67a81-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="67a81-107">Criar um novo objeto [windowsUpdateState](../resources/intune-shared-windowsupdatestate.md) .</span><span class="sxs-lookup"><span data-stu-id="67a81-107">Create a new [windowsUpdateState](../resources/intune-shared-windowsupdatestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="67a81-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="67a81-108">Prerequisites</span></span>
<span data-ttu-id="67a81-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="67a81-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="67a81-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="67a81-111">Permission type</span></span>|<span data-ttu-id="67a81-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="67a81-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="67a81-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="67a81-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="67a81-114">&nbsp; &nbsp; **Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="67a81-114">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="67a81-115">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="67a81-115">DeviceManagementConfiguration.ReadWrite.All</span></span>|
| <span data-ttu-id="67a81-116">&nbsp;&nbsp; **Atualização de software**</span><span class="sxs-lookup"><span data-stu-id="67a81-116">&nbsp; &nbsp; **Software Update**</span></span> | <span data-ttu-id="67a81-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="67a81-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="67a81-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="67a81-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="67a81-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="67a81-119">Not supported.</span></span>|
|<span data-ttu-id="67a81-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="67a81-120">Application</span></span>||
| <span data-ttu-id="67a81-121">&nbsp; &nbsp; **Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="67a81-121">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="67a81-122">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="67a81-122">DeviceManagementConfiguration.ReadWrite.All</span></span>|
| <span data-ttu-id="67a81-123">&nbsp;&nbsp; **Atualização de software**</span><span class="sxs-lookup"><span data-stu-id="67a81-123">&nbsp; &nbsp; **Software Update**</span></span> | <span data-ttu-id="67a81-124">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="67a81-124">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="67a81-125">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="67a81-125">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsUpdateForBusinessConfiguration/deviceUpdateStates
```

## <a name="request-headers"></a><span data-ttu-id="67a81-126">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="67a81-126">Request headers</span></span>
|<span data-ttu-id="67a81-127">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="67a81-127">Header</span></span>|<span data-ttu-id="67a81-128">Valor</span><span class="sxs-lookup"><span data-stu-id="67a81-128">Value</span></span>|
|:---|:---|
|<span data-ttu-id="67a81-129">Autorização</span><span class="sxs-lookup"><span data-stu-id="67a81-129">Authorization</span></span>|<span data-ttu-id="67a81-130">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="67a81-130">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="67a81-131">Aceitar</span><span class="sxs-lookup"><span data-stu-id="67a81-131">Accept</span></span>|<span data-ttu-id="67a81-132">application/json</span><span class="sxs-lookup"><span data-stu-id="67a81-132">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="67a81-133">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="67a81-133">Request body</span></span>
<span data-ttu-id="67a81-134">No corpo da solicitação, forneça uma representação JSON do objeto windowsUpdateState.</span><span class="sxs-lookup"><span data-stu-id="67a81-134">In the request body, supply a JSON representation for the windowsUpdateState object.</span></span>

<span data-ttu-id="67a81-135">A tabela a seguir mostra as propriedades que são necessárias ao criar windowsUpdateState.</span><span class="sxs-lookup"><span data-stu-id="67a81-135">The following table shows the properties that are required when you create the windowsUpdateState.</span></span>

|<span data-ttu-id="67a81-136">Propriedade</span><span class="sxs-lookup"><span data-stu-id="67a81-136">Property</span></span>|<span data-ttu-id="67a81-137">Tipo</span><span class="sxs-lookup"><span data-stu-id="67a81-137">Type</span></span>|<span data-ttu-id="67a81-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="67a81-138">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="67a81-139">id</span><span class="sxs-lookup"><span data-stu-id="67a81-139">id</span></span>|<span data-ttu-id="67a81-140">String</span><span class="sxs-lookup"><span data-stu-id="67a81-140">String</span></span>|<span data-ttu-id="67a81-141">Esta é a ID da entidade.</span><span class="sxs-lookup"><span data-stu-id="67a81-141">This is Id of the entity.</span></span>|
|<span data-ttu-id="67a81-142">deviceId</span><span class="sxs-lookup"><span data-stu-id="67a81-142">deviceId</span></span>|<span data-ttu-id="67a81-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="67a81-143">String</span></span>|<span data-ttu-id="67a81-144">A ID do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="67a81-144">The id of the device.</span></span>|
|<span data-ttu-id="67a81-145">userId</span><span class="sxs-lookup"><span data-stu-id="67a81-145">userId</span></span>|<span data-ttu-id="67a81-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="67a81-146">String</span></span>|<span data-ttu-id="67a81-147">A ID do usuário.</span><span class="sxs-lookup"><span data-stu-id="67a81-147">The id of the user.</span></span>|
|<span data-ttu-id="67a81-148">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="67a81-148">deviceDisplayName</span></span>|<span data-ttu-id="67a81-149">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="67a81-149">String</span></span>|<span data-ttu-id="67a81-150">Nome de exibição do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="67a81-150">Device display name.</span></span>|
|<span data-ttu-id="67a81-151">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="67a81-151">userPrincipalName</span></span>|<span data-ttu-id="67a81-152">String</span><span class="sxs-lookup"><span data-stu-id="67a81-152">String</span></span>|<span data-ttu-id="67a81-153">Nome principal do usuário.</span><span class="sxs-lookup"><span data-stu-id="67a81-153">User principal name.</span></span>|
|<span data-ttu-id="67a81-154">status</span><span class="sxs-lookup"><span data-stu-id="67a81-154">status</span></span>|[<span data-ttu-id="67a81-155">windowsUpdateStatus</span><span class="sxs-lookup"><span data-stu-id="67a81-155">windowsUpdateStatus</span></span>](../resources/intune-deviceconfig-windowsupdatestatus.md)|<span data-ttu-id="67a81-156">Status do Windows UDPATE.</span><span class="sxs-lookup"><span data-stu-id="67a81-156">Windows udpate status.</span></span> <span data-ttu-id="67a81-157">Os valores possíveis são: `upToDate`, `pendingInstallation`, `pendingReboot`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="67a81-157">Possible values are: `upToDate`, `pendingInstallation`, `pendingReboot`, `failed`.</span></span>|
|<span data-ttu-id="67a81-158">qualityUpdateVersion</span><span class="sxs-lookup"><span data-stu-id="67a81-158">qualityUpdateVersion</span></span>|<span data-ttu-id="67a81-159">String</span><span class="sxs-lookup"><span data-stu-id="67a81-159">String</span></span>|<span data-ttu-id="67a81-160">A versão de atualização de qualidade do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="67a81-160">The Quality Update Version of the device.</span></span>|
|<span data-ttu-id="67a81-161">featureUpdateVersion</span><span class="sxs-lookup"><span data-stu-id="67a81-161">featureUpdateVersion</span></span>|<span data-ttu-id="67a81-162">String</span><span class="sxs-lookup"><span data-stu-id="67a81-162">String</span></span>|<span data-ttu-id="67a81-163">A versão atual de atualização de recursos do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="67a81-163">The current feature update version of the device.</span></span>|
|<span data-ttu-id="67a81-164">lastScanDateTime</span><span class="sxs-lookup"><span data-stu-id="67a81-164">lastScanDateTime</span></span>|<span data-ttu-id="67a81-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="67a81-165">DateTimeOffset</span></span>|<span data-ttu-id="67a81-166">A data e hora em que o agente do Windows Update realizou uma verificação bem-sucedida.</span><span class="sxs-lookup"><span data-stu-id="67a81-166">The date time that the Windows Update Agent did a successful scan.</span></span>|
|<span data-ttu-id="67a81-167">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="67a81-167">lastSyncDateTime</span></span>|<span data-ttu-id="67a81-168">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="67a81-168">DateTimeOffset</span></span>|<span data-ttu-id="67a81-169">Data e hora da última sincronização do dispositivo com o Microsoft Intune.</span><span class="sxs-lookup"><span data-stu-id="67a81-169">Last date time that the device sync with with Microsoft Intune.</span></span>|



## <a name="response"></a><span data-ttu-id="67a81-170">Resposta</span><span class="sxs-lookup"><span data-stu-id="67a81-170">Response</span></span>
<span data-ttu-id="67a81-171">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [windowsUpdateState](../resources/intune-shared-windowsupdatestate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="67a81-171">If successful, this method returns a `201 Created` response code and a [windowsUpdateState](../resources/intune-shared-windowsupdatestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="67a81-172">Exemplo</span><span class="sxs-lookup"><span data-stu-id="67a81-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="67a81-173">Solicitação</span><span class="sxs-lookup"><span data-stu-id="67a81-173">Request</span></span>
<span data-ttu-id="67a81-174">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="67a81-174">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="67a81-175">Resposta</span><span class="sxs-lookup"><span data-stu-id="67a81-175">Response</span></span>
<span data-ttu-id="67a81-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="67a81-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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







