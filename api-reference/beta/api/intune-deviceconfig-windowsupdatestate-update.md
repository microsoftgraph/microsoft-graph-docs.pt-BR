---
title: Atualizar windowsUpdateState
description: Atualiza as propriedades de um objeto windowsUpdateState.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 35a56a0dea3174a7f196a3cee62a46edd35eafce
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36344130"
---
# <a name="update-windowsupdatestate"></a><span data-ttu-id="c6aae-103">Atualizar windowsUpdateState</span><span class="sxs-lookup"><span data-stu-id="c6aae-103">Update windowsUpdateState</span></span>

> <span data-ttu-id="c6aae-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c6aae-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c6aae-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c6aae-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c6aae-106">Atualiza as propriedades de um objeto [windowsUpdateState](../resources/intune-deviceconfig-windowsupdatestate.md) .</span><span class="sxs-lookup"><span data-stu-id="c6aae-106">Update the properties of a [windowsUpdateState](../resources/intune-deviceconfig-windowsupdatestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c6aae-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c6aae-107">Prerequisites</span></span>
<span data-ttu-id="c6aae-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c6aae-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c6aae-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c6aae-110">Permission type</span></span>|<span data-ttu-id="c6aae-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="c6aae-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c6aae-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c6aae-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c6aae-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c6aae-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c6aae-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c6aae-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c6aae-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c6aae-115">Not supported.</span></span>|
|<span data-ttu-id="c6aae-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c6aae-116">Application</span></span>|<span data-ttu-id="c6aae-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c6aae-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c6aae-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c6aae-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsUpdateForBusinessConfiguration/deviceUpdateStates/{windowsUpdateStateId}
```

## <a name="request-headers"></a><span data-ttu-id="c6aae-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c6aae-119">Request headers</span></span>
|<span data-ttu-id="c6aae-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c6aae-120">Header</span></span>|<span data-ttu-id="c6aae-121">Valor</span><span class="sxs-lookup"><span data-stu-id="c6aae-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c6aae-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="c6aae-122">Authorization</span></span>|<span data-ttu-id="c6aae-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c6aae-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c6aae-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="c6aae-124">Accept</span></span>|<span data-ttu-id="c6aae-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c6aae-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c6aae-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c6aae-126">Request body</span></span>
<span data-ttu-id="c6aae-127">No corpo da solicitação, forneça uma representação JSON do objeto [windowsUpdateState](../resources/intune-deviceconfig-windowsupdatestate.md) .</span><span class="sxs-lookup"><span data-stu-id="c6aae-127">In the request body, supply a JSON representation for the [windowsUpdateState](../resources/intune-deviceconfig-windowsupdatestate.md) object.</span></span>

<span data-ttu-id="c6aae-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [windowsUpdateState](../resources/intune-deviceconfig-windowsupdatestate.md).</span><span class="sxs-lookup"><span data-stu-id="c6aae-128">The following table shows the properties that are required when you create the [windowsUpdateState](../resources/intune-deviceconfig-windowsupdatestate.md).</span></span>

|<span data-ttu-id="c6aae-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c6aae-129">Property</span></span>|<span data-ttu-id="c6aae-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="c6aae-130">Type</span></span>|<span data-ttu-id="c6aae-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="c6aae-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c6aae-132">id</span><span class="sxs-lookup"><span data-stu-id="c6aae-132">id</span></span>|<span data-ttu-id="c6aae-133">String</span><span class="sxs-lookup"><span data-stu-id="c6aae-133">String</span></span>|<span data-ttu-id="c6aae-134">Esta é a ID da entidade.</span><span class="sxs-lookup"><span data-stu-id="c6aae-134">This is Id of the entity.</span></span>|
|<span data-ttu-id="c6aae-135">deviceId</span><span class="sxs-lookup"><span data-stu-id="c6aae-135">deviceId</span></span>|<span data-ttu-id="c6aae-136">String</span><span class="sxs-lookup"><span data-stu-id="c6aae-136">String</span></span>|<span data-ttu-id="c6aae-137">A ID do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="c6aae-137">The id of the device.</span></span>|
|<span data-ttu-id="c6aae-138">userId</span><span class="sxs-lookup"><span data-stu-id="c6aae-138">userId</span></span>|<span data-ttu-id="c6aae-139">String</span><span class="sxs-lookup"><span data-stu-id="c6aae-139">String</span></span>|<span data-ttu-id="c6aae-140">A ID do usuário.</span><span class="sxs-lookup"><span data-stu-id="c6aae-140">The id of the user.</span></span>|
|<span data-ttu-id="c6aae-141">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="c6aae-141">deviceDisplayName</span></span>|<span data-ttu-id="c6aae-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c6aae-142">String</span></span>|<span data-ttu-id="c6aae-143">Nome de exibição do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="c6aae-143">Device display name.</span></span>|
|<span data-ttu-id="c6aae-144">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="c6aae-144">userPrincipalName</span></span>|<span data-ttu-id="c6aae-145">String</span><span class="sxs-lookup"><span data-stu-id="c6aae-145">String</span></span>|<span data-ttu-id="c6aae-146">Nome principal do usuário.</span><span class="sxs-lookup"><span data-stu-id="c6aae-146">User principal name.</span></span>|
|<span data-ttu-id="c6aae-147">status</span><span class="sxs-lookup"><span data-stu-id="c6aae-147">status</span></span>|[<span data-ttu-id="c6aae-148">windowsUpdateStatus</span><span class="sxs-lookup"><span data-stu-id="c6aae-148">windowsUpdateStatus</span></span>](../resources/intune-deviceconfig-windowsupdatestatus.md)|<span data-ttu-id="c6aae-149">Status do Windows UDPATE.</span><span class="sxs-lookup"><span data-stu-id="c6aae-149">Windows udpate status.</span></span> <span data-ttu-id="c6aae-150">Os valores possíveis são: `upToDate`, `pendingInstallation`, `pendingReboot`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="c6aae-150">Possible values are: `upToDate`, `pendingInstallation`, `pendingReboot`, `failed`.</span></span>|
|<span data-ttu-id="c6aae-151">qualityUpdateVersion</span><span class="sxs-lookup"><span data-stu-id="c6aae-151">qualityUpdateVersion</span></span>|<span data-ttu-id="c6aae-152">String</span><span class="sxs-lookup"><span data-stu-id="c6aae-152">String</span></span>|<span data-ttu-id="c6aae-153">A versão de atualização de qualidade do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="c6aae-153">The Quality Update Version of the device.</span></span>|
|<span data-ttu-id="c6aae-154">featureUpdateVersion</span><span class="sxs-lookup"><span data-stu-id="c6aae-154">featureUpdateVersion</span></span>|<span data-ttu-id="c6aae-155">String</span><span class="sxs-lookup"><span data-stu-id="c6aae-155">String</span></span>|<span data-ttu-id="c6aae-156">A versão atual de atualização de recursos do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="c6aae-156">The current feature update version of the device.</span></span>|
|<span data-ttu-id="c6aae-157">lastScanDateTime</span><span class="sxs-lookup"><span data-stu-id="c6aae-157">lastScanDateTime</span></span>|<span data-ttu-id="c6aae-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c6aae-158">DateTimeOffset</span></span>|<span data-ttu-id="c6aae-159">A data e hora em que o agente do Windows Update realizou uma verificação bem-sucedida.</span><span class="sxs-lookup"><span data-stu-id="c6aae-159">The date time that the Windows Update Agent did a successful scan.</span></span>|
|<span data-ttu-id="c6aae-160">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="c6aae-160">lastSyncDateTime</span></span>|<span data-ttu-id="c6aae-161">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c6aae-161">DateTimeOffset</span></span>|<span data-ttu-id="c6aae-162">Data e hora da última sincronização do dispositivo com o Microsoft Intune.</span><span class="sxs-lookup"><span data-stu-id="c6aae-162">Last date time that the device sync with with Microsoft Intune.</span></span>|



## <a name="response"></a><span data-ttu-id="c6aae-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="c6aae-163">Response</span></span>
<span data-ttu-id="c6aae-164">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [windowsUpdateState](../resources/intune-deviceconfig-windowsupdatestate.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c6aae-164">If successful, this method returns a `200 OK` response code and an updated [windowsUpdateState](../resources/intune-deviceconfig-windowsupdatestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c6aae-165">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c6aae-165">Example</span></span>

### <a name="request"></a><span data-ttu-id="c6aae-166">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c6aae-166">Request</span></span>
<span data-ttu-id="c6aae-167">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c6aae-167">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="c6aae-168">Resposta</span><span class="sxs-lookup"><span data-stu-id="c6aae-168">Response</span></span>
<span data-ttu-id="c6aae-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c6aae-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






