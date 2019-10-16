---
title: Criar windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus
description: Criar um novo objeto windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 295b0b60b7910ef1dbb10fd5733de8f89369808e
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/16/2019
ms.locfileid: "37536655"
---
# <a name="create-windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus"></a><span data-ttu-id="543bf-103">Criar windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus</span><span class="sxs-lookup"><span data-stu-id="543bf-103">Create windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus</span></span>

> <span data-ttu-id="543bf-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="543bf-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="543bf-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="543bf-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="543bf-106">Criar um novo objeto [windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus.md) .</span><span class="sxs-lookup"><span data-stu-id="543bf-106">Create a new [windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="543bf-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="543bf-107">Prerequisites</span></span>
<span data-ttu-id="543bf-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="543bf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="543bf-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="543bf-110">Permission type</span></span>|<span data-ttu-id="543bf-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="543bf-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="543bf-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="543bf-112">Delegated (work or school account)</span></span>|<span data-ttu-id="543bf-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="543bf-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="543bf-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="543bf-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="543bf-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="543bf-115">Not supported.</span></span>|
|<span data-ttu-id="543bf-116">Application</span><span class="sxs-lookup"><span data-stu-id="543bf-116">Application</span></span>|<span data-ttu-id="543bf-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="543bf-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="543bf-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="543bf-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/wdacSupplementalPolicies/{windowsDefenderApplicationControlSupplementalPolicyId}/deviceStatuses
```

## <a name="request-headers"></a><span data-ttu-id="543bf-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="543bf-119">Request headers</span></span>
|<span data-ttu-id="543bf-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="543bf-120">Header</span></span>|<span data-ttu-id="543bf-121">Valor</span><span class="sxs-lookup"><span data-stu-id="543bf-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="543bf-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="543bf-122">Authorization</span></span>|<span data-ttu-id="543bf-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="543bf-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="543bf-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="543bf-124">Accept</span></span>|<span data-ttu-id="543bf-125">application/json</span><span class="sxs-lookup"><span data-stu-id="543bf-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="543bf-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="543bf-126">Request body</span></span>
<span data-ttu-id="543bf-127">No corpo da solicitação, forneça uma representação JSON do objeto windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus.</span><span class="sxs-lookup"><span data-stu-id="543bf-127">In the request body, supply a JSON representation for the windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus object.</span></span>

<span data-ttu-id="543bf-128">A tabela a seguir mostra as propriedades que são necessárias ao criar windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus.</span><span class="sxs-lookup"><span data-stu-id="543bf-128">The following table shows the properties that are required when you create the windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus.</span></span>

|<span data-ttu-id="543bf-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="543bf-129">Property</span></span>|<span data-ttu-id="543bf-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="543bf-130">Type</span></span>|<span data-ttu-id="543bf-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="543bf-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="543bf-132">id</span><span class="sxs-lookup"><span data-stu-id="543bf-132">id</span></span>|<span data-ttu-id="543bf-133">String</span><span class="sxs-lookup"><span data-stu-id="543bf-133">String</span></span>|<span data-ttu-id="543bf-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="543bf-134">Key of the entity.</span></span>|
|<span data-ttu-id="543bf-135">deviceName</span><span class="sxs-lookup"><span data-stu-id="543bf-135">deviceName</span></span>|<span data-ttu-id="543bf-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="543bf-136">String</span></span>|<span data-ttu-id="543bf-137">Nome do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="543bf-137">Device name.</span></span>|
|<span data-ttu-id="543bf-138">deviceId</span><span class="sxs-lookup"><span data-stu-id="543bf-138">deviceId</span></span>|<span data-ttu-id="543bf-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="543bf-139">String</span></span>|<span data-ttu-id="543bf-140">ID de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="543bf-140">Device ID.</span></span>|
|<span data-ttu-id="543bf-141">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="543bf-141">lastSyncDateTime</span></span>|<span data-ttu-id="543bf-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="543bf-142">DateTimeOffset</span></span>|<span data-ttu-id="543bf-143">Hora da data da última sincronização.</span><span class="sxs-lookup"><span data-stu-id="543bf-143">Last sync date time.</span></span>|
|<span data-ttu-id="543bf-144">osVersion</span><span class="sxs-lookup"><span data-stu-id="543bf-144">osVersion</span></span>|<span data-ttu-id="543bf-145">String</span><span class="sxs-lookup"><span data-stu-id="543bf-145">String</span></span>|<span data-ttu-id="543bf-146">Versão do sistema operacional Windows.</span><span class="sxs-lookup"><span data-stu-id="543bf-146">Windows OS Version.</span></span>|
|<span data-ttu-id="543bf-147">osDescription</span><span class="sxs-lookup"><span data-stu-id="543bf-147">osDescription</span></span>|<span data-ttu-id="543bf-148">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="543bf-148">String</span></span>|<span data-ttu-id="543bf-149">Descrição da versão do sistema operacional Windows.</span><span class="sxs-lookup"><span data-stu-id="543bf-149">Windows OS Version Description.</span></span>|
|<span data-ttu-id="543bf-150">deploymentStatus</span><span class="sxs-lookup"><span data-stu-id="543bf-150">deploymentStatus</span></span>|[<span data-ttu-id="543bf-151">windowsDefenderApplicationControlSupplementalPolicyStatuses</span><span class="sxs-lookup"><span data-stu-id="543bf-151">windowsDefenderApplicationControlSupplementalPolicyStatuses</span></span>](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicystatuses.md)|<span data-ttu-id="543bf-152">O estado de implantação da política.</span><span class="sxs-lookup"><span data-stu-id="543bf-152">The deployment state of the policy.</span></span> <span data-ttu-id="543bf-153">Os valores possíveis são: `unknown`, `success`, `tokenError`, `notAuthorizedByToken`, `policyNotFound`.</span><span class="sxs-lookup"><span data-stu-id="543bf-153">Possible values are: `unknown`, `success`, `tokenError`, `notAuthorizedByToken`, `policyNotFound`.</span></span>|
|<span data-ttu-id="543bf-154">userName</span><span class="sxs-lookup"><span data-stu-id="543bf-154">userName</span></span>|<span data-ttu-id="543bf-155">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="543bf-155">String</span></span>|<span data-ttu-id="543bf-156">O nome do usuário deste dispositivo.</span><span class="sxs-lookup"><span data-stu-id="543bf-156">The name of the user of this device.</span></span>|
|<span data-ttu-id="543bf-157">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="543bf-157">userPrincipalName</span></span>|<span data-ttu-id="543bf-158">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="543bf-158">String</span></span>|<span data-ttu-id="543bf-159">Nome principal do usuário.</span><span class="sxs-lookup"><span data-stu-id="543bf-159">User Principal Name.</span></span>|
|<span data-ttu-id="543bf-160">policyVersion</span><span class="sxs-lookup"><span data-stu-id="543bf-160">policyVersion</span></span>|<span data-ttu-id="543bf-161">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="543bf-161">String</span></span>|<span data-ttu-id="543bf-162">Versão de leitura humana da política complementar do WindowsDefenderApplicationControl.</span><span class="sxs-lookup"><span data-stu-id="543bf-162">Human readable version of the WindowsDefenderApplicationControl supplemental policy.</span></span>|



## <a name="response"></a><span data-ttu-id="543bf-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="543bf-163">Response</span></span>
<span data-ttu-id="543bf-164">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="543bf-164">If successful, this method returns a `201 Created` response code and a [windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="543bf-165">Exemplo</span><span class="sxs-lookup"><span data-stu-id="543bf-165">Example</span></span>

### <a name="request"></a><span data-ttu-id="543bf-166">Solicitação</span><span class="sxs-lookup"><span data-stu-id="543bf-166">Request</span></span>
<span data-ttu-id="543bf-167">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="543bf-167">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/wdacSupplementalPolicies/{windowsDefenderApplicationControlSupplementalPolicyId}/deviceStatuses
Content-type: application/json
Content-length: 486

{
  "@odata.type": "#microsoft.graph.windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus",
  "deviceName": "Device Name value",
  "deviceId": "Device Id value",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "osVersion": "Os Version value",
  "osDescription": "Os Description value",
  "deploymentStatus": "success",
  "userName": "User Name value",
  "userPrincipalName": "User Principal Name value",
  "policyVersion": "Policy Version value"
}
```

### <a name="response"></a><span data-ttu-id="543bf-168">Resposta</span><span class="sxs-lookup"><span data-stu-id="543bf-168">Response</span></span>
<span data-ttu-id="543bf-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="543bf-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 535

{
  "@odata.type": "#microsoft.graph.windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus",
  "id": "e3c01841-1841-e3c0-4118-c0e34118c0e3",
  "deviceName": "Device Name value",
  "deviceId": "Device Id value",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "osVersion": "Os Version value",
  "osDescription": "Os Description value",
  "deploymentStatus": "success",
  "userName": "User Name value",
  "userPrincipalName": "User Principal Name value",
  "policyVersion": "Policy Version value"
}
```






