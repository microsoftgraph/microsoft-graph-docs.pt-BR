---
title: Criar windowsUpdateState
description: Criar um novo objeto windowsUpdateState.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 9a5437321741131f2a341c07514e57e50c5ea2be
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36313696"
---
# <a name="create-windowsupdatestate"></a><span data-ttu-id="f1bf5-103">Criar windowsUpdateState</span><span class="sxs-lookup"><span data-stu-id="f1bf5-103">Create windowsUpdateState</span></span>

> <span data-ttu-id="f1bf5-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f1bf5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f1bf5-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f1bf5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f1bf5-106">Criar um novo objeto [windowsUpdateState](../resources/intune-deviceconfig-windowsupdatestate.md) .</span><span class="sxs-lookup"><span data-stu-id="f1bf5-106">Create a new [windowsUpdateState](../resources/intune-deviceconfig-windowsupdatestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f1bf5-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f1bf5-107">Prerequisites</span></span>
<span data-ttu-id="f1bf5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f1bf5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f1bf5-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f1bf5-110">Permission type</span></span>|<span data-ttu-id="f1bf5-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f1bf5-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f1bf5-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f1bf5-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f1bf5-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f1bf5-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f1bf5-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f1bf5-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f1bf5-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f1bf5-115">Not supported.</span></span>|
|<span data-ttu-id="f1bf5-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f1bf5-116">Application</span></span>|<span data-ttu-id="f1bf5-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f1bf5-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f1bf5-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f1bf5-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsUpdateForBusinessConfiguration/deviceUpdateStates
```

## <a name="request-headers"></a><span data-ttu-id="f1bf5-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f1bf5-119">Request headers</span></span>
|<span data-ttu-id="f1bf5-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f1bf5-120">Header</span></span>|<span data-ttu-id="f1bf5-121">Valor</span><span class="sxs-lookup"><span data-stu-id="f1bf5-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f1bf5-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="f1bf5-122">Authorization</span></span>|<span data-ttu-id="f1bf5-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f1bf5-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f1bf5-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f1bf5-124">Accept</span></span>|<span data-ttu-id="f1bf5-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f1bf5-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f1bf5-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f1bf5-126">Request body</span></span>
<span data-ttu-id="f1bf5-127">No corpo da solicitação, forneça uma representação JSON do objeto windowsUpdateState.</span><span class="sxs-lookup"><span data-stu-id="f1bf5-127">In the request body, supply a JSON representation for the windowsUpdateState object.</span></span>

<span data-ttu-id="f1bf5-128">A tabela a seguir mostra as propriedades que são necessárias ao criar windowsUpdateState.</span><span class="sxs-lookup"><span data-stu-id="f1bf5-128">The following table shows the properties that are required when you create the windowsUpdateState.</span></span>

|<span data-ttu-id="f1bf5-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f1bf5-129">Property</span></span>|<span data-ttu-id="f1bf5-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="f1bf5-130">Type</span></span>|<span data-ttu-id="f1bf5-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="f1bf5-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f1bf5-132">id</span><span class="sxs-lookup"><span data-stu-id="f1bf5-132">id</span></span>|<span data-ttu-id="f1bf5-133">String</span><span class="sxs-lookup"><span data-stu-id="f1bf5-133">String</span></span>|<span data-ttu-id="f1bf5-134">Esta é a ID da entidade.</span><span class="sxs-lookup"><span data-stu-id="f1bf5-134">This is Id of the entity.</span></span>|
|<span data-ttu-id="f1bf5-135">deviceId</span><span class="sxs-lookup"><span data-stu-id="f1bf5-135">deviceId</span></span>|<span data-ttu-id="f1bf5-136">String</span><span class="sxs-lookup"><span data-stu-id="f1bf5-136">String</span></span>|<span data-ttu-id="f1bf5-137">A ID do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f1bf5-137">The id of the device.</span></span>|
|<span data-ttu-id="f1bf5-138">userId</span><span class="sxs-lookup"><span data-stu-id="f1bf5-138">userId</span></span>|<span data-ttu-id="f1bf5-139">String</span><span class="sxs-lookup"><span data-stu-id="f1bf5-139">String</span></span>|<span data-ttu-id="f1bf5-140">A ID do usuário.</span><span class="sxs-lookup"><span data-stu-id="f1bf5-140">The id of the user.</span></span>|
|<span data-ttu-id="f1bf5-141">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="f1bf5-141">deviceDisplayName</span></span>|<span data-ttu-id="f1bf5-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f1bf5-142">String</span></span>|<span data-ttu-id="f1bf5-143">Nome de exibição do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f1bf5-143">Device display name.</span></span>|
|<span data-ttu-id="f1bf5-144">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="f1bf5-144">userPrincipalName</span></span>|<span data-ttu-id="f1bf5-145">String</span><span class="sxs-lookup"><span data-stu-id="f1bf5-145">String</span></span>|<span data-ttu-id="f1bf5-146">Nome principal do usuário.</span><span class="sxs-lookup"><span data-stu-id="f1bf5-146">User principal name.</span></span>|
|<span data-ttu-id="f1bf5-147">status</span><span class="sxs-lookup"><span data-stu-id="f1bf5-147">status</span></span>|[<span data-ttu-id="f1bf5-148">windowsUpdateStatus</span><span class="sxs-lookup"><span data-stu-id="f1bf5-148">windowsUpdateStatus</span></span>](../resources/intune-deviceconfig-windowsupdatestatus.md)|<span data-ttu-id="f1bf5-149">Status do Windows UDPATE.</span><span class="sxs-lookup"><span data-stu-id="f1bf5-149">Windows udpate status.</span></span> <span data-ttu-id="f1bf5-150">Os valores possíveis são: `upToDate`, `pendingInstallation`, `pendingReboot`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="f1bf5-150">Possible values are: `upToDate`, `pendingInstallation`, `pendingReboot`, `failed`.</span></span>|
|<span data-ttu-id="f1bf5-151">qualityUpdateVersion</span><span class="sxs-lookup"><span data-stu-id="f1bf5-151">qualityUpdateVersion</span></span>|<span data-ttu-id="f1bf5-152">String</span><span class="sxs-lookup"><span data-stu-id="f1bf5-152">String</span></span>|<span data-ttu-id="f1bf5-153">A versão de atualização de qualidade do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f1bf5-153">The Quality Update Version of the device.</span></span>|
|<span data-ttu-id="f1bf5-154">featureUpdateVersion</span><span class="sxs-lookup"><span data-stu-id="f1bf5-154">featureUpdateVersion</span></span>|<span data-ttu-id="f1bf5-155">String</span><span class="sxs-lookup"><span data-stu-id="f1bf5-155">String</span></span>|<span data-ttu-id="f1bf5-156">A versão atual de atualização de recursos do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f1bf5-156">The current feature update version of the device.</span></span>|
|<span data-ttu-id="f1bf5-157">lastScanDateTime</span><span class="sxs-lookup"><span data-stu-id="f1bf5-157">lastScanDateTime</span></span>|<span data-ttu-id="f1bf5-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f1bf5-158">DateTimeOffset</span></span>|<span data-ttu-id="f1bf5-159">A data e hora em que o agente do Windows Update realizou uma verificação bem-sucedida.</span><span class="sxs-lookup"><span data-stu-id="f1bf5-159">The date time that the Windows Update Agent did a successful scan.</span></span>|
|<span data-ttu-id="f1bf5-160">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="f1bf5-160">lastSyncDateTime</span></span>|<span data-ttu-id="f1bf5-161">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f1bf5-161">DateTimeOffset</span></span>|<span data-ttu-id="f1bf5-162">Data e hora da última sincronização do dispositivo com o Microsoft Intune.</span><span class="sxs-lookup"><span data-stu-id="f1bf5-162">Last date time that the device sync with with Microsoft Intune.</span></span>|



## <a name="response"></a><span data-ttu-id="f1bf5-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="f1bf5-163">Response</span></span>
<span data-ttu-id="f1bf5-164">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [windowsUpdateState](../resources/intune-deviceconfig-windowsupdatestate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f1bf5-164">If successful, this method returns a `201 Created` response code and a [windowsUpdateState](../resources/intune-deviceconfig-windowsupdatestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f1bf5-165">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f1bf5-165">Example</span></span>

### <a name="request"></a><span data-ttu-id="f1bf5-166">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f1bf5-166">Request</span></span>
<span data-ttu-id="f1bf5-167">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f1bf5-167">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f1bf5-168">Resposta</span><span class="sxs-lookup"><span data-stu-id="f1bf5-168">Response</span></span>
<span data-ttu-id="f1bf5-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f1bf5-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






