---
title: Criar windowsUpdateState
description: Crie um novo objeto windowsUpdateState.
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: bad8d5a7d91e90e7907227d4091ef7cb5fefb8da
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/16/2021
ms.locfileid: "51866185"
---
# <a name="create-windowsupdatestate"></a><span data-ttu-id="21e2a-103">Criar windowsUpdateState</span><span class="sxs-lookup"><span data-stu-id="21e2a-103">Create windowsUpdateState</span></span>

<span data-ttu-id="21e2a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="21e2a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="21e2a-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="21e2a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="21e2a-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="21e2a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="21e2a-107">Crie um novo [objeto windowsUpdateState.](../resources/intune-shared-windowsupdatestate.md)</span><span class="sxs-lookup"><span data-stu-id="21e2a-107">Create a new [windowsUpdateState](../resources/intune-shared-windowsupdatestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="21e2a-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="21e2a-108">Prerequisites</span></span>
<span data-ttu-id="21e2a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="21e2a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="21e2a-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="21e2a-111">Permission type</span></span>|<span data-ttu-id="21e2a-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="21e2a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="21e2a-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="21e2a-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="21e2a-114">&nbsp; &nbsp; **Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="21e2a-114">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="21e2a-115">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="21e2a-115">DeviceManagementConfiguration.ReadWrite.All</span></span>|
| <span data-ttu-id="21e2a-116">&nbsp;&nbsp; **Atualização de Software**</span><span class="sxs-lookup"><span data-stu-id="21e2a-116">&nbsp; &nbsp; **Software Update**</span></span> | <span data-ttu-id="21e2a-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="21e2a-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="21e2a-118">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="21e2a-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="21e2a-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="21e2a-119">Not supported.</span></span>|
|<span data-ttu-id="21e2a-120">Application</span><span class="sxs-lookup"><span data-stu-id="21e2a-120">Application</span></span>||
| <span data-ttu-id="21e2a-121">&nbsp; &nbsp; **Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="21e2a-121">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="21e2a-122">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="21e2a-122">DeviceManagementConfiguration.ReadWrite.All</span></span>|
| <span data-ttu-id="21e2a-123">&nbsp;&nbsp; **Atualização de Software**</span><span class="sxs-lookup"><span data-stu-id="21e2a-123">&nbsp; &nbsp; **Software Update**</span></span> | <span data-ttu-id="21e2a-124">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="21e2a-124">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="21e2a-125">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="21e2a-125">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsUpdateForBusinessConfiguration/deviceUpdateStates
```

## <a name="request-headers"></a><span data-ttu-id="21e2a-126">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="21e2a-126">Request headers</span></span>
|<span data-ttu-id="21e2a-127">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="21e2a-127">Header</span></span>|<span data-ttu-id="21e2a-128">Valor</span><span class="sxs-lookup"><span data-stu-id="21e2a-128">Value</span></span>|
|:---|:---|
|<span data-ttu-id="21e2a-129">Autorização</span><span class="sxs-lookup"><span data-stu-id="21e2a-129">Authorization</span></span>|<span data-ttu-id="21e2a-130">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="21e2a-130">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="21e2a-131">Aceitar</span><span class="sxs-lookup"><span data-stu-id="21e2a-131">Accept</span></span>|<span data-ttu-id="21e2a-132">application/json</span><span class="sxs-lookup"><span data-stu-id="21e2a-132">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="21e2a-133">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="21e2a-133">Request body</span></span>
<span data-ttu-id="21e2a-134">No corpo da solicitação, fornece uma representação JSON para o objeto windowsUpdateState.</span><span class="sxs-lookup"><span data-stu-id="21e2a-134">In the request body, supply a JSON representation for the windowsUpdateState object.</span></span>

<span data-ttu-id="21e2a-135">A tabela a seguir mostra as propriedades que são necessárias ao criar o windowsUpdateState.</span><span class="sxs-lookup"><span data-stu-id="21e2a-135">The following table shows the properties that are required when you create the windowsUpdateState.</span></span>

|<span data-ttu-id="21e2a-136">Propriedade</span><span class="sxs-lookup"><span data-stu-id="21e2a-136">Property</span></span>|<span data-ttu-id="21e2a-137">Tipo</span><span class="sxs-lookup"><span data-stu-id="21e2a-137">Type</span></span>|<span data-ttu-id="21e2a-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="21e2a-138">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="21e2a-139">id</span><span class="sxs-lookup"><span data-stu-id="21e2a-139">id</span></span>|<span data-ttu-id="21e2a-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="21e2a-140">String</span></span>|<span data-ttu-id="21e2a-141">Esta é a ID da entidade.</span><span class="sxs-lookup"><span data-stu-id="21e2a-141">This is Id of the entity.</span></span>|
|<span data-ttu-id="21e2a-142">deviceId</span><span class="sxs-lookup"><span data-stu-id="21e2a-142">deviceId</span></span>|<span data-ttu-id="21e2a-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="21e2a-143">String</span></span>|<span data-ttu-id="21e2a-144">A id do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="21e2a-144">The id of the device.</span></span>|
|<span data-ttu-id="21e2a-145">userId</span><span class="sxs-lookup"><span data-stu-id="21e2a-145">userId</span></span>|<span data-ttu-id="21e2a-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="21e2a-146">String</span></span>|<span data-ttu-id="21e2a-147">A id do usuário.</span><span class="sxs-lookup"><span data-stu-id="21e2a-147">The id of the user.</span></span>|
|<span data-ttu-id="21e2a-148">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="21e2a-148">deviceDisplayName</span></span>|<span data-ttu-id="21e2a-149">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="21e2a-149">String</span></span>|<span data-ttu-id="21e2a-150">Nome de exibição do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="21e2a-150">Device display name.</span></span>|
|<span data-ttu-id="21e2a-151">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="21e2a-151">userPrincipalName</span></span>|<span data-ttu-id="21e2a-152">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="21e2a-152">String</span></span>|<span data-ttu-id="21e2a-153">Nome principal do usuário.</span><span class="sxs-lookup"><span data-stu-id="21e2a-153">User principal name.</span></span>|
|<span data-ttu-id="21e2a-154">status</span><span class="sxs-lookup"><span data-stu-id="21e2a-154">status</span></span>|[<span data-ttu-id="21e2a-155">windowsUpdateStatus</span><span class="sxs-lookup"><span data-stu-id="21e2a-155">windowsUpdateStatus</span></span>](../resources/intune-deviceconfig-windowsupdatestatus.md)|<span data-ttu-id="21e2a-156">Status udpate do Windows.</span><span class="sxs-lookup"><span data-stu-id="21e2a-156">Windows udpate status.</span></span> <span data-ttu-id="21e2a-157">Os valores possíveis são: `upToDate`, `pendingInstallation`, `pendingReboot`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="21e2a-157">Possible values are: `upToDate`, `pendingInstallation`, `pendingReboot`, `failed`.</span></span>|
|<span data-ttu-id="21e2a-158">qualityUpdateVersion</span><span class="sxs-lookup"><span data-stu-id="21e2a-158">qualityUpdateVersion</span></span>|<span data-ttu-id="21e2a-159">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="21e2a-159">String</span></span>|<span data-ttu-id="21e2a-160">A Versão de Atualização de Qualidade do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="21e2a-160">The Quality Update Version of the device.</span></span>|
|<span data-ttu-id="21e2a-161">featureUpdateVersion</span><span class="sxs-lookup"><span data-stu-id="21e2a-161">featureUpdateVersion</span></span>|<span data-ttu-id="21e2a-162">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="21e2a-162">String</span></span>|<span data-ttu-id="21e2a-163">A versão atual de atualização de recursos do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="21e2a-163">The current feature update version of the device.</span></span>|
|<span data-ttu-id="21e2a-164">lastScanDateTime</span><span class="sxs-lookup"><span data-stu-id="21e2a-164">lastScanDateTime</span></span>|<span data-ttu-id="21e2a-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="21e2a-165">DateTimeOffset</span></span>|<span data-ttu-id="21e2a-166">A data em que o Agente do Windows Update fez uma verificação bem-sucedida.</span><span class="sxs-lookup"><span data-stu-id="21e2a-166">The date time that the Windows Update Agent did a successful scan.</span></span>|
|<span data-ttu-id="21e2a-167">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="21e2a-167">lastSyncDateTime</span></span>|<span data-ttu-id="21e2a-168">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="21e2a-168">DateTimeOffset</span></span>|<span data-ttu-id="21e2a-169">Última data em que o dispositivo sincroniza com o Microsoft Intune.</span><span class="sxs-lookup"><span data-stu-id="21e2a-169">Last date time that the device sync with with Microsoft Intune.</span></span>|



## <a name="response"></a><span data-ttu-id="21e2a-170">Resposta</span><span class="sxs-lookup"><span data-stu-id="21e2a-170">Response</span></span>
<span data-ttu-id="21e2a-171">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto windowsUpdateState](../resources/intune-shared-windowsupdatestate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="21e2a-171">If successful, this method returns a `201 Created` response code and a [windowsUpdateState](../resources/intune-shared-windowsupdatestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="21e2a-172">Exemplo</span><span class="sxs-lookup"><span data-stu-id="21e2a-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="21e2a-173">Solicitação</span><span class="sxs-lookup"><span data-stu-id="21e2a-173">Request</span></span>
<span data-ttu-id="21e2a-174">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="21e2a-174">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="21e2a-175">Resposta</span><span class="sxs-lookup"><span data-stu-id="21e2a-175">Response</span></span>
<span data-ttu-id="21e2a-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="21e2a-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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







