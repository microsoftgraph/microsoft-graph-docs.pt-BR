---
title: Criar windowsUpdateState
description: Criar um novo objeto windowsUpdateState.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0b428197cea201bffc59153d3df561ea7ddacea4
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35725828"
---
# <a name="create-windowsupdatestate"></a><span data-ttu-id="1bc7c-103">Criar windowsUpdateState</span><span class="sxs-lookup"><span data-stu-id="1bc7c-103">Create windowsUpdateState</span></span>

> <span data-ttu-id="1bc7c-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="1bc7c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1bc7c-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1bc7c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1bc7c-106">Criar um novo objeto [windowsUpdateState](../resources/intune-deviceconfig-windowsupdatestate.md) .</span><span class="sxs-lookup"><span data-stu-id="1bc7c-106">Create a new [windowsUpdateState](../resources/intune-deviceconfig-windowsupdatestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1bc7c-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="1bc7c-107">Prerequisites</span></span>
<span data-ttu-id="1bc7c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1bc7c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1bc7c-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1bc7c-110">Permission type</span></span>|<span data-ttu-id="1bc7c-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="1bc7c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1bc7c-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1bc7c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="1bc7c-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1bc7c-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="1bc7c-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1bc7c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1bc7c-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1bc7c-115">Not supported.</span></span>|
|<span data-ttu-id="1bc7c-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1bc7c-116">Application</span></span>|<span data-ttu-id="1bc7c-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1bc7c-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1bc7c-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1bc7c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsUpdateForBusinessConfiguration/deviceUpdateStates
```

## <a name="request-headers"></a><span data-ttu-id="1bc7c-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1bc7c-119">Request headers</span></span>
|<span data-ttu-id="1bc7c-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1bc7c-120">Header</span></span>|<span data-ttu-id="1bc7c-121">Valor</span><span class="sxs-lookup"><span data-stu-id="1bc7c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1bc7c-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="1bc7c-122">Authorization</span></span>|<span data-ttu-id="1bc7c-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1bc7c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1bc7c-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="1bc7c-124">Accept</span></span>|<span data-ttu-id="1bc7c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="1bc7c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1bc7c-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1bc7c-126">Request body</span></span>
<span data-ttu-id="1bc7c-127">No corpo da solicitação, forneça uma representação JSON do objeto windowsUpdateState.</span><span class="sxs-lookup"><span data-stu-id="1bc7c-127">In the request body, supply a JSON representation for the windowsUpdateState object.</span></span>

<span data-ttu-id="1bc7c-128">A tabela a seguir mostra as propriedades que são necessárias ao criar windowsUpdateState.</span><span class="sxs-lookup"><span data-stu-id="1bc7c-128">The following table shows the properties that are required when you create the windowsUpdateState.</span></span>

|<span data-ttu-id="1bc7c-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1bc7c-129">Property</span></span>|<span data-ttu-id="1bc7c-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="1bc7c-130">Type</span></span>|<span data-ttu-id="1bc7c-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="1bc7c-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1bc7c-132">id</span><span class="sxs-lookup"><span data-stu-id="1bc7c-132">id</span></span>|<span data-ttu-id="1bc7c-133">String</span><span class="sxs-lookup"><span data-stu-id="1bc7c-133">String</span></span>|<span data-ttu-id="1bc7c-134">Esta é a ID da entidade.</span><span class="sxs-lookup"><span data-stu-id="1bc7c-134">This is Id of the entity.</span></span>|
|<span data-ttu-id="1bc7c-135">deviceId</span><span class="sxs-lookup"><span data-stu-id="1bc7c-135">deviceId</span></span>|<span data-ttu-id="1bc7c-136">String</span><span class="sxs-lookup"><span data-stu-id="1bc7c-136">String</span></span>|<span data-ttu-id="1bc7c-137">A ID do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="1bc7c-137">The id of the device.</span></span>|
|<span data-ttu-id="1bc7c-138">userId</span><span class="sxs-lookup"><span data-stu-id="1bc7c-138">userId</span></span>|<span data-ttu-id="1bc7c-139">String</span><span class="sxs-lookup"><span data-stu-id="1bc7c-139">String</span></span>|<span data-ttu-id="1bc7c-140">A ID do usuário.</span><span class="sxs-lookup"><span data-stu-id="1bc7c-140">The id of the user.</span></span>|
|<span data-ttu-id="1bc7c-141">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="1bc7c-141">deviceDisplayName</span></span>|<span data-ttu-id="1bc7c-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1bc7c-142">String</span></span>|<span data-ttu-id="1bc7c-143">Nome de exibição do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="1bc7c-143">Device display name.</span></span>|
|<span data-ttu-id="1bc7c-144">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="1bc7c-144">userPrincipalName</span></span>|<span data-ttu-id="1bc7c-145">String</span><span class="sxs-lookup"><span data-stu-id="1bc7c-145">String</span></span>|<span data-ttu-id="1bc7c-146">Nome principal do usuário.</span><span class="sxs-lookup"><span data-stu-id="1bc7c-146">User principal name.</span></span>|
|<span data-ttu-id="1bc7c-147">status</span><span class="sxs-lookup"><span data-stu-id="1bc7c-147">status</span></span>|[<span data-ttu-id="1bc7c-148">windowsUpdateStatus</span><span class="sxs-lookup"><span data-stu-id="1bc7c-148">windowsUpdateStatus</span></span>](../resources/intune-deviceconfig-windowsupdatestatus.md)|<span data-ttu-id="1bc7c-149">Status do Windows UDPATE.</span><span class="sxs-lookup"><span data-stu-id="1bc7c-149">Windows udpate status.</span></span> <span data-ttu-id="1bc7c-150">Os valores possíveis são: `upToDate`, `pendingInstallation`, `pendingReboot`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="1bc7c-150">Possible values are: `upToDate`, `pendingInstallation`, `pendingReboot`, `failed`.</span></span>|
|<span data-ttu-id="1bc7c-151">qualityUpdateVersion</span><span class="sxs-lookup"><span data-stu-id="1bc7c-151">qualityUpdateVersion</span></span>|<span data-ttu-id="1bc7c-152">String</span><span class="sxs-lookup"><span data-stu-id="1bc7c-152">String</span></span>|<span data-ttu-id="1bc7c-153">A versão de atualização de qualidade do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="1bc7c-153">The Quality Update Version of the device.</span></span>|
|<span data-ttu-id="1bc7c-154">featureUpdateVersion</span><span class="sxs-lookup"><span data-stu-id="1bc7c-154">featureUpdateVersion</span></span>|<span data-ttu-id="1bc7c-155">String</span><span class="sxs-lookup"><span data-stu-id="1bc7c-155">String</span></span>|<span data-ttu-id="1bc7c-156">A versão atual de atualização de recursos do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="1bc7c-156">The current feature update version of the device.</span></span>|
|<span data-ttu-id="1bc7c-157">lastScanDateTime</span><span class="sxs-lookup"><span data-stu-id="1bc7c-157">lastScanDateTime</span></span>|<span data-ttu-id="1bc7c-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1bc7c-158">DateTimeOffset</span></span>|<span data-ttu-id="1bc7c-159">A data e hora em que o agente do Windows Update realizou uma verificação bem-sucedida.</span><span class="sxs-lookup"><span data-stu-id="1bc7c-159">The date time that the Windows Update Agent did a successful scan.</span></span>|
|<span data-ttu-id="1bc7c-160">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="1bc7c-160">lastSyncDateTime</span></span>|<span data-ttu-id="1bc7c-161">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1bc7c-161">DateTimeOffset</span></span>|<span data-ttu-id="1bc7c-162">Data e hora da última sincronização do dispositivo com o Microsoft Intune.</span><span class="sxs-lookup"><span data-stu-id="1bc7c-162">Last date time that the device sync with with Microsoft Intune.</span></span>|



## <a name="response"></a><span data-ttu-id="1bc7c-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="1bc7c-163">Response</span></span>
<span data-ttu-id="1bc7c-164">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [windowsUpdateState](../resources/intune-deviceconfig-windowsupdatestate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1bc7c-164">If successful, this method returns a `201 Created` response code and a [windowsUpdateState](../resources/intune-deviceconfig-windowsupdatestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1bc7c-165">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1bc7c-165">Example</span></span>

### <a name="request"></a><span data-ttu-id="1bc7c-166">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1bc7c-166">Request</span></span>
<span data-ttu-id="1bc7c-167">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1bc7c-167">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="1bc7c-168">Resposta</span><span class="sxs-lookup"><span data-stu-id="1bc7c-168">Response</span></span>
<span data-ttu-id="1bc7c-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1bc7c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





