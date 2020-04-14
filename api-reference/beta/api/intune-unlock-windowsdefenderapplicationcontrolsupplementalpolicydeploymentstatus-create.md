---
title: Criar windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus
description: Criar um novo objeto windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 18af990c81696e235ca9e29879c6570773527d0f
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43472293"
---
# <a name="create-windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus"></a><span data-ttu-id="5add3-103">Criar windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus</span><span class="sxs-lookup"><span data-stu-id="5add3-103">Create windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus</span></span>

<span data-ttu-id="5add3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5add3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5add3-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="5add3-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5add3-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="5add3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5add3-107">Criar um novo objeto [windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus.md) .</span><span class="sxs-lookup"><span data-stu-id="5add3-107">Create a new [windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5add3-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="5add3-108">Prerequisites</span></span>
<span data-ttu-id="5add3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5add3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5add3-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5add3-111">Permission type</span></span>|<span data-ttu-id="5add3-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="5add3-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5add3-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5add3-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5add3-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5add3-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="5add3-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5add3-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5add3-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5add3-116">Not supported.</span></span>|
|<span data-ttu-id="5add3-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5add3-117">Application</span></span>|<span data-ttu-id="5add3-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5add3-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5add3-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5add3-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/wdacSupplementalPolicies/{windowsDefenderApplicationControlSupplementalPolicyId}/deviceStatuses
```

## <a name="request-headers"></a><span data-ttu-id="5add3-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5add3-120">Request headers</span></span>
|<span data-ttu-id="5add3-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5add3-121">Header</span></span>|<span data-ttu-id="5add3-122">Valor</span><span class="sxs-lookup"><span data-stu-id="5add3-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5add3-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="5add3-123">Authorization</span></span>|<span data-ttu-id="5add3-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5add3-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5add3-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="5add3-125">Accept</span></span>|<span data-ttu-id="5add3-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5add3-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5add3-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5add3-127">Request body</span></span>
<span data-ttu-id="5add3-128">No corpo da solicitação, forneça uma representação JSON do objeto windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus.</span><span class="sxs-lookup"><span data-stu-id="5add3-128">In the request body, supply a JSON representation for the windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus object.</span></span>

<span data-ttu-id="5add3-129">A tabela a seguir mostra as propriedades que são necessárias ao criar windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus.</span><span class="sxs-lookup"><span data-stu-id="5add3-129">The following table shows the properties that are required when you create the windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus.</span></span>

|<span data-ttu-id="5add3-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5add3-130">Property</span></span>|<span data-ttu-id="5add3-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="5add3-131">Type</span></span>|<span data-ttu-id="5add3-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="5add3-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5add3-133">id</span><span class="sxs-lookup"><span data-stu-id="5add3-133">id</span></span>|<span data-ttu-id="5add3-134">String</span><span class="sxs-lookup"><span data-stu-id="5add3-134">String</span></span>|<span data-ttu-id="5add3-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="5add3-135">Key of the entity.</span></span>|
|<span data-ttu-id="5add3-136">deviceName</span><span class="sxs-lookup"><span data-stu-id="5add3-136">deviceName</span></span>|<span data-ttu-id="5add3-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5add3-137">String</span></span>|<span data-ttu-id="5add3-138">Nome do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="5add3-138">Device name.</span></span>|
|<span data-ttu-id="5add3-139">deviceId</span><span class="sxs-lookup"><span data-stu-id="5add3-139">deviceId</span></span>|<span data-ttu-id="5add3-140">String</span><span class="sxs-lookup"><span data-stu-id="5add3-140">String</span></span>|<span data-ttu-id="5add3-141">ID de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="5add3-141">Device ID.</span></span>|
|<span data-ttu-id="5add3-142">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="5add3-142">lastSyncDateTime</span></span>|<span data-ttu-id="5add3-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5add3-143">DateTimeOffset</span></span>|<span data-ttu-id="5add3-144">Hora da data da última sincronização.</span><span class="sxs-lookup"><span data-stu-id="5add3-144">Last sync date time.</span></span>|
|<span data-ttu-id="5add3-145">osVersion</span><span class="sxs-lookup"><span data-stu-id="5add3-145">osVersion</span></span>|<span data-ttu-id="5add3-146">String</span><span class="sxs-lookup"><span data-stu-id="5add3-146">String</span></span>|<span data-ttu-id="5add3-147">Versão do sistema operacional Windows.</span><span class="sxs-lookup"><span data-stu-id="5add3-147">Windows OS Version.</span></span>|
|<span data-ttu-id="5add3-148">osDescription</span><span class="sxs-lookup"><span data-stu-id="5add3-148">osDescription</span></span>|<span data-ttu-id="5add3-149">String</span><span class="sxs-lookup"><span data-stu-id="5add3-149">String</span></span>|<span data-ttu-id="5add3-150">Descrição da versão do sistema operacional Windows.</span><span class="sxs-lookup"><span data-stu-id="5add3-150">Windows OS Version Description.</span></span>|
|<span data-ttu-id="5add3-151">deploymentStatus</span><span class="sxs-lookup"><span data-stu-id="5add3-151">deploymentStatus</span></span>|[<span data-ttu-id="5add3-152">windowsDefenderApplicationControlSupplementalPolicyStatuses</span><span class="sxs-lookup"><span data-stu-id="5add3-152">windowsDefenderApplicationControlSupplementalPolicyStatuses</span></span>](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicystatuses.md)|<span data-ttu-id="5add3-153">O estado de implantação da política.</span><span class="sxs-lookup"><span data-stu-id="5add3-153">The deployment state of the policy.</span></span> <span data-ttu-id="5add3-154">Os valores possíveis são: `unknown`, `success`, `tokenError`, `notAuthorizedByToken`, `policyNotFound`.</span><span class="sxs-lookup"><span data-stu-id="5add3-154">Possible values are: `unknown`, `success`, `tokenError`, `notAuthorizedByToken`, `policyNotFound`.</span></span>|
|<span data-ttu-id="5add3-155">userName</span><span class="sxs-lookup"><span data-stu-id="5add3-155">userName</span></span>|<span data-ttu-id="5add3-156">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5add3-156">String</span></span>|<span data-ttu-id="5add3-157">O nome do usuário deste dispositivo.</span><span class="sxs-lookup"><span data-stu-id="5add3-157">The name of the user of this device.</span></span>|
|<span data-ttu-id="5add3-158">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="5add3-158">userPrincipalName</span></span>|<span data-ttu-id="5add3-159">String</span><span class="sxs-lookup"><span data-stu-id="5add3-159">String</span></span>|<span data-ttu-id="5add3-160">Nome principal do usuário.</span><span class="sxs-lookup"><span data-stu-id="5add3-160">User Principal Name.</span></span>|
|<span data-ttu-id="5add3-161">policyVersion</span><span class="sxs-lookup"><span data-stu-id="5add3-161">policyVersion</span></span>|<span data-ttu-id="5add3-162">String</span><span class="sxs-lookup"><span data-stu-id="5add3-162">String</span></span>|<span data-ttu-id="5add3-163">Versão de leitura humana da política complementar do WindowsDefenderApplicationControl.</span><span class="sxs-lookup"><span data-stu-id="5add3-163">Human readable version of the WindowsDefenderApplicationControl supplemental policy.</span></span>|



## <a name="response"></a><span data-ttu-id="5add3-164">Resposta</span><span class="sxs-lookup"><span data-stu-id="5add3-164">Response</span></span>
<span data-ttu-id="5add3-165">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5add3-165">If successful, this method returns a `201 Created` response code and a [windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5add3-166">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5add3-166">Example</span></span>

### <a name="request"></a><span data-ttu-id="5add3-167">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5add3-167">Request</span></span>
<span data-ttu-id="5add3-168">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5add3-168">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="5add3-169">Resposta</span><span class="sxs-lookup"><span data-stu-id="5add3-169">Response</span></span>
<span data-ttu-id="5add3-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5add3-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



