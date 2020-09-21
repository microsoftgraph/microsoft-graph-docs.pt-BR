---
title: Atualizar windowsUpdateState
description: Atualiza as propriedades de um objeto windowsUpdateState.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 27b486f909e7bfcd11c4d354d5a60160e79024bf
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47966944"
---
# <a name="update-windowsupdatestate"></a><span data-ttu-id="49abc-103">Atualizar windowsUpdateState</span><span class="sxs-lookup"><span data-stu-id="49abc-103">Update windowsUpdateState</span></span>

<span data-ttu-id="49abc-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="49abc-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="49abc-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="49abc-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="49abc-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="49abc-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="49abc-107">Atualiza as propriedades de um objeto [windowsUpdateState](../resources/intune-shared-windowsupdatestate.md) .</span><span class="sxs-lookup"><span data-stu-id="49abc-107">Update the properties of a [windowsUpdateState](../resources/intune-shared-windowsupdatestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="49abc-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="49abc-108">Prerequisites</span></span>
<span data-ttu-id="49abc-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="49abc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="49abc-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="49abc-111">Permission type</span></span>|<span data-ttu-id="49abc-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="49abc-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="49abc-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="49abc-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="49abc-114">&nbsp; &nbsp; **Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="49abc-114">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="49abc-115">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="49abc-115">DeviceManagementConfiguration.ReadWrite.All</span></span>|
| <span data-ttu-id="49abc-116">&nbsp;&nbsp; **Atualização de software**</span><span class="sxs-lookup"><span data-stu-id="49abc-116">&nbsp; &nbsp; **Software Update**</span></span> | <span data-ttu-id="49abc-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="49abc-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="49abc-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="49abc-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="49abc-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="49abc-119">Not supported.</span></span>|
|<span data-ttu-id="49abc-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="49abc-120">Application</span></span>||
| <span data-ttu-id="49abc-121">&nbsp; &nbsp; **Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="49abc-121">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="49abc-122">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="49abc-122">DeviceManagementConfiguration.ReadWrite.All</span></span>|
| <span data-ttu-id="49abc-123">&nbsp;&nbsp; **Atualização de software**</span><span class="sxs-lookup"><span data-stu-id="49abc-123">&nbsp; &nbsp; **Software Update**</span></span> | <span data-ttu-id="49abc-124">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="49abc-124">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="49abc-125">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="49abc-125">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsUpdateForBusinessConfiguration/deviceUpdateStates/{windowsUpdateStateId}
```

## <a name="request-headers"></a><span data-ttu-id="49abc-126">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="49abc-126">Request headers</span></span>
|<span data-ttu-id="49abc-127">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="49abc-127">Header</span></span>|<span data-ttu-id="49abc-128">Valor</span><span class="sxs-lookup"><span data-stu-id="49abc-128">Value</span></span>|
|:---|:---|
|<span data-ttu-id="49abc-129">Autorização</span><span class="sxs-lookup"><span data-stu-id="49abc-129">Authorization</span></span>|<span data-ttu-id="49abc-130">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="49abc-130">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="49abc-131">Aceitar</span><span class="sxs-lookup"><span data-stu-id="49abc-131">Accept</span></span>|<span data-ttu-id="49abc-132">application/json</span><span class="sxs-lookup"><span data-stu-id="49abc-132">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="49abc-133">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="49abc-133">Request body</span></span>
<span data-ttu-id="49abc-134">No corpo da solicitação, forneça uma representação JSON do objeto [windowsUpdateState](../resources/intune-shared-windowsupdatestate.md) .</span><span class="sxs-lookup"><span data-stu-id="49abc-134">In the request body, supply a JSON representation for the [windowsUpdateState](../resources/intune-shared-windowsupdatestate.md) object.</span></span>

<span data-ttu-id="49abc-135">A tabela a seguir mostra as propriedades que são necessárias ao criar [windowsUpdateState](../resources/intune-shared-windowsupdatestate.md).</span><span class="sxs-lookup"><span data-stu-id="49abc-135">The following table shows the properties that are required when you create the [windowsUpdateState](../resources/intune-shared-windowsupdatestate.md).</span></span>

|<span data-ttu-id="49abc-136">Propriedade</span><span class="sxs-lookup"><span data-stu-id="49abc-136">Property</span></span>|<span data-ttu-id="49abc-137">Tipo</span><span class="sxs-lookup"><span data-stu-id="49abc-137">Type</span></span>|<span data-ttu-id="49abc-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="49abc-138">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="49abc-139">id</span><span class="sxs-lookup"><span data-stu-id="49abc-139">id</span></span>|<span data-ttu-id="49abc-140">String</span><span class="sxs-lookup"><span data-stu-id="49abc-140">String</span></span>|<span data-ttu-id="49abc-141">Esta é a ID da entidade.</span><span class="sxs-lookup"><span data-stu-id="49abc-141">This is Id of the entity.</span></span>|
|<span data-ttu-id="49abc-142">deviceId</span><span class="sxs-lookup"><span data-stu-id="49abc-142">deviceId</span></span>|<span data-ttu-id="49abc-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="49abc-143">String</span></span>|<span data-ttu-id="49abc-144">A ID do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="49abc-144">The id of the device.</span></span>|
|<span data-ttu-id="49abc-145">userId</span><span class="sxs-lookup"><span data-stu-id="49abc-145">userId</span></span>|<span data-ttu-id="49abc-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="49abc-146">String</span></span>|<span data-ttu-id="49abc-147">A ID do usuário.</span><span class="sxs-lookup"><span data-stu-id="49abc-147">The id of the user.</span></span>|
|<span data-ttu-id="49abc-148">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="49abc-148">deviceDisplayName</span></span>|<span data-ttu-id="49abc-149">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="49abc-149">String</span></span>|<span data-ttu-id="49abc-150">Nome de exibição do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="49abc-150">Device display name.</span></span>|
|<span data-ttu-id="49abc-151">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="49abc-151">userPrincipalName</span></span>|<span data-ttu-id="49abc-152">String</span><span class="sxs-lookup"><span data-stu-id="49abc-152">String</span></span>|<span data-ttu-id="49abc-153">Nome principal do usuário.</span><span class="sxs-lookup"><span data-stu-id="49abc-153">User principal name.</span></span>|
|<span data-ttu-id="49abc-154">status</span><span class="sxs-lookup"><span data-stu-id="49abc-154">status</span></span>|[<span data-ttu-id="49abc-155">windowsUpdateStatus</span><span class="sxs-lookup"><span data-stu-id="49abc-155">windowsUpdateStatus</span></span>](../resources/intune-shared-windowsupdatestatus.md)|<span data-ttu-id="49abc-156">Status do Windows UDPATE.</span><span class="sxs-lookup"><span data-stu-id="49abc-156">Windows udpate status.</span></span> <span data-ttu-id="49abc-157">Os valores possíveis são: `upToDate`, `pendingInstallation`, `pendingReboot`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="49abc-157">Possible values are: `upToDate`, `pendingInstallation`, `pendingReboot`, `failed`.</span></span>|
|<span data-ttu-id="49abc-158">qualityUpdateVersion</span><span class="sxs-lookup"><span data-stu-id="49abc-158">qualityUpdateVersion</span></span>|<span data-ttu-id="49abc-159">String</span><span class="sxs-lookup"><span data-stu-id="49abc-159">String</span></span>|<span data-ttu-id="49abc-160">A versão de atualização de qualidade do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="49abc-160">The Quality Update Version of the device.</span></span>|
|<span data-ttu-id="49abc-161">featureUpdateVersion</span><span class="sxs-lookup"><span data-stu-id="49abc-161">featureUpdateVersion</span></span>|<span data-ttu-id="49abc-162">String</span><span class="sxs-lookup"><span data-stu-id="49abc-162">String</span></span>|<span data-ttu-id="49abc-163">A versão atual de atualização de recursos do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="49abc-163">The current feature update version of the device.</span></span>|
|<span data-ttu-id="49abc-164">lastScanDateTime</span><span class="sxs-lookup"><span data-stu-id="49abc-164">lastScanDateTime</span></span>|<span data-ttu-id="49abc-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="49abc-165">DateTimeOffset</span></span>|<span data-ttu-id="49abc-166">A data e hora em que o agente do Windows Update realizou uma verificação bem-sucedida.</span><span class="sxs-lookup"><span data-stu-id="49abc-166">The date time that the Windows Update Agent did a successful scan.</span></span>|
|<span data-ttu-id="49abc-167">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="49abc-167">lastSyncDateTime</span></span>|<span data-ttu-id="49abc-168">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="49abc-168">DateTimeOffset</span></span>|<span data-ttu-id="49abc-169">Data e hora da última sincronização do dispositivo com o Microsoft Intune.</span><span class="sxs-lookup"><span data-stu-id="49abc-169">Last date time that the device sync with with Microsoft Intune.</span></span>|



## <a name="response"></a><span data-ttu-id="49abc-170">Resposta</span><span class="sxs-lookup"><span data-stu-id="49abc-170">Response</span></span>
<span data-ttu-id="49abc-171">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [windowsUpdateState](../resources/intune-shared-windowsupdatestate.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="49abc-171">If successful, this method returns a `200 OK` response code and an updated [windowsUpdateState](../resources/intune-shared-windowsupdatestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="49abc-172">Exemplo</span><span class="sxs-lookup"><span data-stu-id="49abc-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="49abc-173">Solicitação</span><span class="sxs-lookup"><span data-stu-id="49abc-173">Request</span></span>
<span data-ttu-id="49abc-174">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="49abc-174">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="49abc-175">Resposta</span><span class="sxs-lookup"><span data-stu-id="49abc-175">Response</span></span>
<span data-ttu-id="49abc-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="49abc-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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









