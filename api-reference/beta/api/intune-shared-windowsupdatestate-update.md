---
title: Atualizar windowsUpdateState
description: Atualiza as propriedades de um objeto windowsUpdateState.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: c235781a73059830a3b0085bb7602e5484da7988
ms.sourcegitcommit: 0545b031585e605dc3a0fde481015f51f79819c4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/22/2020
ms.locfileid: "45225015"
---
# <a name="update-windowsupdatestate"></a><span data-ttu-id="8e301-103">Atualizar windowsUpdateState</span><span class="sxs-lookup"><span data-stu-id="8e301-103">Update windowsUpdateState</span></span>

<span data-ttu-id="8e301-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8e301-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8e301-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="8e301-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8e301-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="8e301-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8e301-107">Atualiza as propriedades de um objeto [windowsUpdateState](../resources/intune-shared-windowsupdatestate.md) .</span><span class="sxs-lookup"><span data-stu-id="8e301-107">Update the properties of a [windowsUpdateState](../resources/intune-shared-windowsupdatestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8e301-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="8e301-108">Prerequisites</span></span>
<span data-ttu-id="8e301-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8e301-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8e301-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8e301-111">Permission type</span></span>|<span data-ttu-id="8e301-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="8e301-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8e301-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8e301-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="8e301-114">&nbsp;&nbsp; **Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="8e301-114">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="8e301-115">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8e301-115">DeviceManagementConfiguration.ReadWrite.All</span></span>|
| <span data-ttu-id="8e301-116">&nbsp;&nbsp; **Atualização de software**</span><span class="sxs-lookup"><span data-stu-id="8e301-116">&nbsp; &nbsp; **Software Update**</span></span> | <span data-ttu-id="8e301-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8e301-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8e301-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8e301-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8e301-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8e301-119">Not supported.</span></span>|
|<span data-ttu-id="8e301-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8e301-120">Application</span></span>||
| <span data-ttu-id="8e301-121">&nbsp;&nbsp; **Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="8e301-121">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="8e301-122">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8e301-122">DeviceManagementConfiguration.ReadWrite.All</span></span>|
| <span data-ttu-id="8e301-123">&nbsp;&nbsp; **Atualização de software**</span><span class="sxs-lookup"><span data-stu-id="8e301-123">&nbsp; &nbsp; **Software Update**</span></span> | <span data-ttu-id="8e301-124">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8e301-124">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8e301-125">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8e301-125">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsUpdateForBusinessConfiguration/deviceUpdateStates/{windowsUpdateStateId}
```

## <a name="request-headers"></a><span data-ttu-id="8e301-126">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8e301-126">Request headers</span></span>
|<span data-ttu-id="8e301-127">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8e301-127">Header</span></span>|<span data-ttu-id="8e301-128">Valor</span><span class="sxs-lookup"><span data-stu-id="8e301-128">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8e301-129">Autorização</span><span class="sxs-lookup"><span data-stu-id="8e301-129">Authorization</span></span>|<span data-ttu-id="8e301-130">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8e301-130">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8e301-131">Aceitar</span><span class="sxs-lookup"><span data-stu-id="8e301-131">Accept</span></span>|<span data-ttu-id="8e301-132">application/json</span><span class="sxs-lookup"><span data-stu-id="8e301-132">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8e301-133">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8e301-133">Request body</span></span>
<span data-ttu-id="8e301-134">No corpo da solicitação, forneça uma representação JSON do objeto [windowsUpdateState](../resources/intune-shared-windowsupdatestate.md) .</span><span class="sxs-lookup"><span data-stu-id="8e301-134">In the request body, supply a JSON representation for the [windowsUpdateState](../resources/intune-shared-windowsupdatestate.md) object.</span></span>

<span data-ttu-id="8e301-135">A tabela a seguir mostra as propriedades que são necessárias ao criar [windowsUpdateState](../resources/intune-shared-windowsupdatestate.md).</span><span class="sxs-lookup"><span data-stu-id="8e301-135">The following table shows the properties that are required when you create the [windowsUpdateState](../resources/intune-shared-windowsupdatestate.md).</span></span>

|<span data-ttu-id="8e301-136">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8e301-136">Property</span></span>|<span data-ttu-id="8e301-137">Tipo</span><span class="sxs-lookup"><span data-stu-id="8e301-137">Type</span></span>|<span data-ttu-id="8e301-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="8e301-138">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8e301-139">id</span><span class="sxs-lookup"><span data-stu-id="8e301-139">id</span></span>|<span data-ttu-id="8e301-140">String</span><span class="sxs-lookup"><span data-stu-id="8e301-140">String</span></span>|<span data-ttu-id="8e301-141">Esta é a ID da entidade.</span><span class="sxs-lookup"><span data-stu-id="8e301-141">This is Id of the entity.</span></span>|
|<span data-ttu-id="8e301-142">deviceId</span><span class="sxs-lookup"><span data-stu-id="8e301-142">deviceId</span></span>|<span data-ttu-id="8e301-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8e301-143">String</span></span>|<span data-ttu-id="8e301-144">A ID do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="8e301-144">The id of the device.</span></span>|
|<span data-ttu-id="8e301-145">userId</span><span class="sxs-lookup"><span data-stu-id="8e301-145">userId</span></span>|<span data-ttu-id="8e301-146">String</span><span class="sxs-lookup"><span data-stu-id="8e301-146">String</span></span>|<span data-ttu-id="8e301-147">A ID do usuário.</span><span class="sxs-lookup"><span data-stu-id="8e301-147">The id of the user.</span></span>|
|<span data-ttu-id="8e301-148">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="8e301-148">deviceDisplayName</span></span>|<span data-ttu-id="8e301-149">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8e301-149">String</span></span>|<span data-ttu-id="8e301-150">Nome de exibição do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="8e301-150">Device display name.</span></span>|
|<span data-ttu-id="8e301-151">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="8e301-151">userPrincipalName</span></span>|<span data-ttu-id="8e301-152">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8e301-152">String</span></span>|<span data-ttu-id="8e301-153">Nome principal do usuário.</span><span class="sxs-lookup"><span data-stu-id="8e301-153">User principal name.</span></span>|
|<span data-ttu-id="8e301-154">status</span><span class="sxs-lookup"><span data-stu-id="8e301-154">status</span></span>||<span data-ttu-id="8e301-155">Status do Windows UDPATE.</span><span class="sxs-lookup"><span data-stu-id="8e301-155">Windows udpate status.</span></span> <span data-ttu-id="8e301-156">Os valores possíveis são: `upToDate`, `pendingInstallation`, `pendingReboot`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="8e301-156">Possible values are: `upToDate`, `pendingInstallation`, `pendingReboot`, `failed`.</span></span>|
|<span data-ttu-id="8e301-157">qualityUpdateVersion</span><span class="sxs-lookup"><span data-stu-id="8e301-157">qualityUpdateVersion</span></span>|<span data-ttu-id="8e301-158">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8e301-158">String</span></span>|<span data-ttu-id="8e301-159">A versão de atualização de qualidade do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="8e301-159">The Quality Update Version of the device.</span></span>|
|<span data-ttu-id="8e301-160">featureUpdateVersion</span><span class="sxs-lookup"><span data-stu-id="8e301-160">featureUpdateVersion</span></span>|<span data-ttu-id="8e301-161">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8e301-161">String</span></span>|<span data-ttu-id="8e301-162">A versão atual de atualização de recursos do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="8e301-162">The current feature update version of the device.</span></span>|
|<span data-ttu-id="8e301-163">lastScanDateTime</span><span class="sxs-lookup"><span data-stu-id="8e301-163">lastScanDateTime</span></span>|<span data-ttu-id="8e301-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8e301-164">DateTimeOffset</span></span>|<span data-ttu-id="8e301-165">A data e hora em que o agente do Windows Update realizou uma verificação bem-sucedida.</span><span class="sxs-lookup"><span data-stu-id="8e301-165">The date time that the Windows Update Agent did a successful scan.</span></span>|
|<span data-ttu-id="8e301-166">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="8e301-166">lastSyncDateTime</span></span>|<span data-ttu-id="8e301-167">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8e301-167">DateTimeOffset</span></span>|<span data-ttu-id="8e301-168">Data e hora da última sincronização do dispositivo com o Microsoft Intune.</span><span class="sxs-lookup"><span data-stu-id="8e301-168">Last date time that the device sync with with Microsoft Intune.</span></span>|



## <a name="response"></a><span data-ttu-id="8e301-169">Resposta</span><span class="sxs-lookup"><span data-stu-id="8e301-169">Response</span></span>
<span data-ttu-id="8e301-170">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [windowsUpdateState](../resources/intune-shared-windowsupdatestate.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8e301-170">If successful, this method returns a `200 OK` response code and an updated [windowsUpdateState](../resources/intune-shared-windowsupdatestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8e301-171">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8e301-171">Example</span></span>

### <a name="request"></a><span data-ttu-id="8e301-172">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8e301-172">Request</span></span>
<span data-ttu-id="8e301-173">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8e301-173">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="8e301-174">Resposta</span><span class="sxs-lookup"><span data-stu-id="8e301-174">Response</span></span>
<span data-ttu-id="8e301-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8e301-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






