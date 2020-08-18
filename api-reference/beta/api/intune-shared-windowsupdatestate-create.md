---
title: Criar windowsUpdateState
description: Criar um novo objeto windowsUpdateState.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 0fbc9cb8668d8d7f7ca50cd875d3aa042a2002ad
ms.sourcegitcommit: dc3bade0c096d5ce716d4bc07cd9c7cabb52477b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/18/2020
ms.locfileid: "46790529"
---
# <a name="create-windowsupdatestate"></a><span data-ttu-id="4b5d8-103">Criar windowsUpdateState</span><span class="sxs-lookup"><span data-stu-id="4b5d8-103">Create windowsUpdateState</span></span>

<span data-ttu-id="4b5d8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4b5d8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4b5d8-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="4b5d8-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4b5d8-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="4b5d8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4b5d8-107">Criar um novo objeto [windowsUpdateState](../resources/intune-shared-windowsupdatestate.md) .</span><span class="sxs-lookup"><span data-stu-id="4b5d8-107">Create a new [windowsUpdateState](../resources/intune-shared-windowsupdatestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4b5d8-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="4b5d8-108">Prerequisites</span></span>
<span data-ttu-id="4b5d8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4b5d8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4b5d8-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4b5d8-111">Permission type</span></span>|<span data-ttu-id="4b5d8-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="4b5d8-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4b5d8-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4b5d8-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="4b5d8-114">&nbsp; &nbsp; **Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="4b5d8-114">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="4b5d8-115">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4b5d8-115">DeviceManagementConfiguration.ReadWrite.All</span></span>|
| <span data-ttu-id="4b5d8-116">&nbsp;&nbsp; **Atualização de software**</span><span class="sxs-lookup"><span data-stu-id="4b5d8-116">&nbsp; &nbsp; **Software Update**</span></span> | <span data-ttu-id="4b5d8-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4b5d8-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4b5d8-118">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4b5d8-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4b5d8-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4b5d8-119">Not supported.</span></span>|
|<span data-ttu-id="4b5d8-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4b5d8-120">Application</span></span>||
| <span data-ttu-id="4b5d8-121">&nbsp; &nbsp; **Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="4b5d8-121">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="4b5d8-122">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4b5d8-122">DeviceManagementConfiguration.ReadWrite.All</span></span>|
| <span data-ttu-id="4b5d8-123">&nbsp;&nbsp; **Atualização de software**</span><span class="sxs-lookup"><span data-stu-id="4b5d8-123">&nbsp; &nbsp; **Software Update**</span></span> | <span data-ttu-id="4b5d8-124">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4b5d8-124">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4b5d8-125">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4b5d8-125">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsUpdateForBusinessConfiguration/deviceUpdateStates
```

## <a name="request-headers"></a><span data-ttu-id="4b5d8-126">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4b5d8-126">Request headers</span></span>
|<span data-ttu-id="4b5d8-127">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4b5d8-127">Header</span></span>|<span data-ttu-id="4b5d8-128">Valor</span><span class="sxs-lookup"><span data-stu-id="4b5d8-128">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4b5d8-129">Autorização</span><span class="sxs-lookup"><span data-stu-id="4b5d8-129">Authorization</span></span>|<span data-ttu-id="4b5d8-130">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4b5d8-130">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4b5d8-131">Aceitar</span><span class="sxs-lookup"><span data-stu-id="4b5d8-131">Accept</span></span>|<span data-ttu-id="4b5d8-132">application/json</span><span class="sxs-lookup"><span data-stu-id="4b5d8-132">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4b5d8-133">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4b5d8-133">Request body</span></span>
<span data-ttu-id="4b5d8-134">No corpo da solicitação, forneça uma representação JSON do objeto windowsUpdateState.</span><span class="sxs-lookup"><span data-stu-id="4b5d8-134">In the request body, supply a JSON representation for the windowsUpdateState object.</span></span>

<span data-ttu-id="4b5d8-135">A tabela a seguir mostra as propriedades que são necessárias ao criar windowsUpdateState.</span><span class="sxs-lookup"><span data-stu-id="4b5d8-135">The following table shows the properties that are required when you create the windowsUpdateState.</span></span>

|<span data-ttu-id="4b5d8-136">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4b5d8-136">Property</span></span>|<span data-ttu-id="4b5d8-137">Tipo</span><span class="sxs-lookup"><span data-stu-id="4b5d8-137">Type</span></span>|<span data-ttu-id="4b5d8-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="4b5d8-138">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4b5d8-139">id</span><span class="sxs-lookup"><span data-stu-id="4b5d8-139">id</span></span>|<span data-ttu-id="4b5d8-140">String</span><span class="sxs-lookup"><span data-stu-id="4b5d8-140">String</span></span>|<span data-ttu-id="4b5d8-141">Esta é a ID da entidade.</span><span class="sxs-lookup"><span data-stu-id="4b5d8-141">This is Id of the entity.</span></span>|
|<span data-ttu-id="4b5d8-142">deviceId</span><span class="sxs-lookup"><span data-stu-id="4b5d8-142">deviceId</span></span>|<span data-ttu-id="4b5d8-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4b5d8-143">String</span></span>|<span data-ttu-id="4b5d8-144">A ID do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="4b5d8-144">The id of the device.</span></span>|
|<span data-ttu-id="4b5d8-145">userId</span><span class="sxs-lookup"><span data-stu-id="4b5d8-145">userId</span></span>|<span data-ttu-id="4b5d8-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4b5d8-146">String</span></span>|<span data-ttu-id="4b5d8-147">A ID do usuário.</span><span class="sxs-lookup"><span data-stu-id="4b5d8-147">The id of the user.</span></span>|
|<span data-ttu-id="4b5d8-148">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="4b5d8-148">deviceDisplayName</span></span>|<span data-ttu-id="4b5d8-149">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4b5d8-149">String</span></span>|<span data-ttu-id="4b5d8-150">Nome de exibição do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="4b5d8-150">Device display name.</span></span>|
|<span data-ttu-id="4b5d8-151">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="4b5d8-151">userPrincipalName</span></span>|<span data-ttu-id="4b5d8-152">String</span><span class="sxs-lookup"><span data-stu-id="4b5d8-152">String</span></span>|<span data-ttu-id="4b5d8-153">Nome principal do usuário.</span><span class="sxs-lookup"><span data-stu-id="4b5d8-153">User principal name.</span></span>|
|<span data-ttu-id="4b5d8-154">status</span><span class="sxs-lookup"><span data-stu-id="4b5d8-154">status</span></span>|[<span data-ttu-id="4b5d8-155">windowsUpdateStatus</span><span class="sxs-lookup"><span data-stu-id="4b5d8-155">windowsUpdateStatus</span></span>](../resources/intune-deviceconfig-windowsupdatestatus.md)|<span data-ttu-id="4b5d8-156">Status do Windows UDPATE.</span><span class="sxs-lookup"><span data-stu-id="4b5d8-156">Windows udpate status.</span></span> <span data-ttu-id="4b5d8-157">Os valores possíveis são: `upToDate`, `pendingInstallation`, `pendingReboot`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="4b5d8-157">Possible values are: `upToDate`, `pendingInstallation`, `pendingReboot`, `failed`.</span></span>|
|<span data-ttu-id="4b5d8-158">qualityUpdateVersion</span><span class="sxs-lookup"><span data-stu-id="4b5d8-158">qualityUpdateVersion</span></span>|<span data-ttu-id="4b5d8-159">String</span><span class="sxs-lookup"><span data-stu-id="4b5d8-159">String</span></span>|<span data-ttu-id="4b5d8-160">A versão de atualização de qualidade do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="4b5d8-160">The Quality Update Version of the device.</span></span>|
|<span data-ttu-id="4b5d8-161">featureUpdateVersion</span><span class="sxs-lookup"><span data-stu-id="4b5d8-161">featureUpdateVersion</span></span>|<span data-ttu-id="4b5d8-162">String</span><span class="sxs-lookup"><span data-stu-id="4b5d8-162">String</span></span>|<span data-ttu-id="4b5d8-163">A versão atual de atualização de recursos do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="4b5d8-163">The current feature update version of the device.</span></span>|
|<span data-ttu-id="4b5d8-164">lastScanDateTime</span><span class="sxs-lookup"><span data-stu-id="4b5d8-164">lastScanDateTime</span></span>|<span data-ttu-id="4b5d8-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4b5d8-165">DateTimeOffset</span></span>|<span data-ttu-id="4b5d8-166">A data e hora em que o agente do Windows Update realizou uma verificação bem-sucedida.</span><span class="sxs-lookup"><span data-stu-id="4b5d8-166">The date time that the Windows Update Agent did a successful scan.</span></span>|
|<span data-ttu-id="4b5d8-167">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="4b5d8-167">lastSyncDateTime</span></span>|<span data-ttu-id="4b5d8-168">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4b5d8-168">DateTimeOffset</span></span>|<span data-ttu-id="4b5d8-169">Data e hora da última sincronização do dispositivo com o Microsoft Intune.</span><span class="sxs-lookup"><span data-stu-id="4b5d8-169">Last date time that the device sync with with Microsoft Intune.</span></span>|



## <a name="response"></a><span data-ttu-id="4b5d8-170">Resposta</span><span class="sxs-lookup"><span data-stu-id="4b5d8-170">Response</span></span>
<span data-ttu-id="4b5d8-171">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [windowsUpdateState](../resources/intune-shared-windowsupdatestate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4b5d8-171">If successful, this method returns a `201 Created` response code and a [windowsUpdateState](../resources/intune-shared-windowsupdatestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4b5d8-172">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4b5d8-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="4b5d8-173">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4b5d8-173">Request</span></span>
<span data-ttu-id="4b5d8-174">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4b5d8-174">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="4b5d8-175">Resposta</span><span class="sxs-lookup"><span data-stu-id="4b5d8-175">Response</span></span>
<span data-ttu-id="4b5d8-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4b5d8-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






