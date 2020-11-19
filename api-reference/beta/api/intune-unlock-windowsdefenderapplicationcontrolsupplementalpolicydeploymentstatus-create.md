---
title: Criar windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus
description: Criar um novo objeto windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: fef6d21122855587f2b107b861c63381ba0d4dd5
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49223098"
---
# <a name="create-windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus"></a><span data-ttu-id="99df1-103">Criar windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus</span><span class="sxs-lookup"><span data-stu-id="99df1-103">Create windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus</span></span>

<span data-ttu-id="99df1-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="99df1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="99df1-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="99df1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="99df1-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="99df1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="99df1-107">Criar um novo objeto [windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus.md) .</span><span class="sxs-lookup"><span data-stu-id="99df1-107">Create a new [windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="99df1-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="99df1-108">Prerequisites</span></span>
<span data-ttu-id="99df1-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="99df1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="99df1-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="99df1-111">Permission type</span></span>|<span data-ttu-id="99df1-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="99df1-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="99df1-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="99df1-113">Delegated (work or school account)</span></span>|<span data-ttu-id="99df1-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="99df1-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="99df1-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="99df1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="99df1-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="99df1-116">Not supported.</span></span>|
|<span data-ttu-id="99df1-117">Application</span><span class="sxs-lookup"><span data-stu-id="99df1-117">Application</span></span>|<span data-ttu-id="99df1-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="99df1-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="99df1-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="99df1-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/wdacSupplementalPolicies/{windowsDefenderApplicationControlSupplementalPolicyId}/deviceStatuses
```

## <a name="request-headers"></a><span data-ttu-id="99df1-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="99df1-120">Request headers</span></span>
|<span data-ttu-id="99df1-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="99df1-121">Header</span></span>|<span data-ttu-id="99df1-122">Valor</span><span class="sxs-lookup"><span data-stu-id="99df1-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="99df1-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="99df1-123">Authorization</span></span>|<span data-ttu-id="99df1-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="99df1-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="99df1-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="99df1-125">Accept</span></span>|<span data-ttu-id="99df1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="99df1-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="99df1-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="99df1-127">Request body</span></span>
<span data-ttu-id="99df1-128">No corpo da solicitação, forneça uma representação JSON do objeto windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus.</span><span class="sxs-lookup"><span data-stu-id="99df1-128">In the request body, supply a JSON representation for the windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus object.</span></span>

<span data-ttu-id="99df1-129">A tabela a seguir mostra as propriedades que são necessárias ao criar windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus.</span><span class="sxs-lookup"><span data-stu-id="99df1-129">The following table shows the properties that are required when you create the windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus.</span></span>

|<span data-ttu-id="99df1-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="99df1-130">Property</span></span>|<span data-ttu-id="99df1-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="99df1-131">Type</span></span>|<span data-ttu-id="99df1-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="99df1-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="99df1-133">id</span><span class="sxs-lookup"><span data-stu-id="99df1-133">id</span></span>|<span data-ttu-id="99df1-134">String</span><span class="sxs-lookup"><span data-stu-id="99df1-134">String</span></span>|<span data-ttu-id="99df1-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="99df1-135">Key of the entity.</span></span>|
|<span data-ttu-id="99df1-136">deviceName</span><span class="sxs-lookup"><span data-stu-id="99df1-136">deviceName</span></span>|<span data-ttu-id="99df1-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="99df1-137">String</span></span>|<span data-ttu-id="99df1-138">Nome do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="99df1-138">Device name.</span></span>|
|<span data-ttu-id="99df1-139">deviceId</span><span class="sxs-lookup"><span data-stu-id="99df1-139">deviceId</span></span>|<span data-ttu-id="99df1-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="99df1-140">String</span></span>|<span data-ttu-id="99df1-141">ID de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="99df1-141">Device ID.</span></span>|
|<span data-ttu-id="99df1-142">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="99df1-142">lastSyncDateTime</span></span>|<span data-ttu-id="99df1-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="99df1-143">DateTimeOffset</span></span>|<span data-ttu-id="99df1-144">Hora da data da última sincronização.</span><span class="sxs-lookup"><span data-stu-id="99df1-144">Last sync date time.</span></span>|
|<span data-ttu-id="99df1-145">osVersion</span><span class="sxs-lookup"><span data-stu-id="99df1-145">osVersion</span></span>|<span data-ttu-id="99df1-146">String</span><span class="sxs-lookup"><span data-stu-id="99df1-146">String</span></span>|<span data-ttu-id="99df1-147">Versão do sistema operacional Windows.</span><span class="sxs-lookup"><span data-stu-id="99df1-147">Windows OS Version.</span></span>|
|<span data-ttu-id="99df1-148">osDescription</span><span class="sxs-lookup"><span data-stu-id="99df1-148">osDescription</span></span>|<span data-ttu-id="99df1-149">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="99df1-149">String</span></span>|<span data-ttu-id="99df1-150">Descrição da versão do sistema operacional Windows.</span><span class="sxs-lookup"><span data-stu-id="99df1-150">Windows OS Version Description.</span></span>|
|<span data-ttu-id="99df1-151">deploymentStatus</span><span class="sxs-lookup"><span data-stu-id="99df1-151">deploymentStatus</span></span>|[<span data-ttu-id="99df1-152">windowsDefenderApplicationControlSupplementalPolicyStatuses</span><span class="sxs-lookup"><span data-stu-id="99df1-152">windowsDefenderApplicationControlSupplementalPolicyStatuses</span></span>](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicystatuses.md)|<span data-ttu-id="99df1-153">O estado de implantação da política.</span><span class="sxs-lookup"><span data-stu-id="99df1-153">The deployment state of the policy.</span></span> <span data-ttu-id="99df1-154">Os valores possíveis são: `unknown`, `success`, `tokenError`, `notAuthorizedByToken`, `policyNotFound`.</span><span class="sxs-lookup"><span data-stu-id="99df1-154">Possible values are: `unknown`, `success`, `tokenError`, `notAuthorizedByToken`, `policyNotFound`.</span></span>|
|<span data-ttu-id="99df1-155">userName</span><span class="sxs-lookup"><span data-stu-id="99df1-155">userName</span></span>|<span data-ttu-id="99df1-156">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="99df1-156">String</span></span>|<span data-ttu-id="99df1-157">O nome do usuário deste dispositivo.</span><span class="sxs-lookup"><span data-stu-id="99df1-157">The name of the user of this device.</span></span>|
|<span data-ttu-id="99df1-158">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="99df1-158">userPrincipalName</span></span>|<span data-ttu-id="99df1-159">String</span><span class="sxs-lookup"><span data-stu-id="99df1-159">String</span></span>|<span data-ttu-id="99df1-160">Nome principal do usuário.</span><span class="sxs-lookup"><span data-stu-id="99df1-160">User Principal Name.</span></span>|
|<span data-ttu-id="99df1-161">policyVersion</span><span class="sxs-lookup"><span data-stu-id="99df1-161">policyVersion</span></span>|<span data-ttu-id="99df1-162">String</span><span class="sxs-lookup"><span data-stu-id="99df1-162">String</span></span>|<span data-ttu-id="99df1-163">Versão de leitura humana da política complementar do WindowsDefenderApplicationControl.</span><span class="sxs-lookup"><span data-stu-id="99df1-163">Human readable version of the WindowsDefenderApplicationControl supplemental policy.</span></span>|



## <a name="response"></a><span data-ttu-id="99df1-164">Resposta</span><span class="sxs-lookup"><span data-stu-id="99df1-164">Response</span></span>
<span data-ttu-id="99df1-165">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="99df1-165">If successful, this method returns a `201 Created` response code and a [windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="99df1-166">Exemplo</span><span class="sxs-lookup"><span data-stu-id="99df1-166">Example</span></span>

### <a name="request"></a><span data-ttu-id="99df1-167">Solicitação</span><span class="sxs-lookup"><span data-stu-id="99df1-167">Request</span></span>
<span data-ttu-id="99df1-168">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="99df1-168">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="99df1-169">Resposta</span><span class="sxs-lookup"><span data-stu-id="99df1-169">Response</span></span>
<span data-ttu-id="99df1-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="99df1-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




