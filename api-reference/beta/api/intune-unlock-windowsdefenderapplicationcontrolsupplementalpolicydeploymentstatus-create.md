---
title: Criar windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus
description: Criar um novo objeto windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 3528cc2da190464ddfd60a013440ae9cd21c9d6b
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39938730"
---
# <a name="create-windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus"></a><span data-ttu-id="55d42-103">Criar windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus</span><span class="sxs-lookup"><span data-stu-id="55d42-103">Create windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus</span></span>

> <span data-ttu-id="55d42-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="55d42-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="55d42-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="55d42-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="55d42-106">Criar um novo objeto [windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus.md) .</span><span class="sxs-lookup"><span data-stu-id="55d42-106">Create a new [windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="55d42-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="55d42-107">Prerequisites</span></span>
<span data-ttu-id="55d42-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="55d42-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="55d42-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="55d42-110">Permission type</span></span>|<span data-ttu-id="55d42-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="55d42-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="55d42-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="55d42-112">Delegated (work or school account)</span></span>|<span data-ttu-id="55d42-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="55d42-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="55d42-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="55d42-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="55d42-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="55d42-115">Not supported.</span></span>|
|<span data-ttu-id="55d42-116">Application</span><span class="sxs-lookup"><span data-stu-id="55d42-116">Application</span></span>|<span data-ttu-id="55d42-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="55d42-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="55d42-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="55d42-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/wdacSupplementalPolicies/{windowsDefenderApplicationControlSupplementalPolicyId}/deviceStatuses
```

## <a name="request-headers"></a><span data-ttu-id="55d42-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="55d42-119">Request headers</span></span>
|<span data-ttu-id="55d42-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="55d42-120">Header</span></span>|<span data-ttu-id="55d42-121">Valor</span><span class="sxs-lookup"><span data-stu-id="55d42-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="55d42-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="55d42-122">Authorization</span></span>|<span data-ttu-id="55d42-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="55d42-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="55d42-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="55d42-124">Accept</span></span>|<span data-ttu-id="55d42-125">application/json</span><span class="sxs-lookup"><span data-stu-id="55d42-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="55d42-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="55d42-126">Request body</span></span>
<span data-ttu-id="55d42-127">No corpo da solicitação, forneça uma representação JSON do objeto windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus.</span><span class="sxs-lookup"><span data-stu-id="55d42-127">In the request body, supply a JSON representation for the windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus object.</span></span>

<span data-ttu-id="55d42-128">A tabela a seguir mostra as propriedades que são necessárias ao criar windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus.</span><span class="sxs-lookup"><span data-stu-id="55d42-128">The following table shows the properties that are required when you create the windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus.</span></span>

|<span data-ttu-id="55d42-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="55d42-129">Property</span></span>|<span data-ttu-id="55d42-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="55d42-130">Type</span></span>|<span data-ttu-id="55d42-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="55d42-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="55d42-132">id</span><span class="sxs-lookup"><span data-stu-id="55d42-132">id</span></span>|<span data-ttu-id="55d42-133">String</span><span class="sxs-lookup"><span data-stu-id="55d42-133">String</span></span>|<span data-ttu-id="55d42-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="55d42-134">Key of the entity.</span></span>|
|<span data-ttu-id="55d42-135">deviceName</span><span class="sxs-lookup"><span data-stu-id="55d42-135">deviceName</span></span>|<span data-ttu-id="55d42-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="55d42-136">String</span></span>|<span data-ttu-id="55d42-137">Nome do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="55d42-137">Device name.</span></span>|
|<span data-ttu-id="55d42-138">deviceId</span><span class="sxs-lookup"><span data-stu-id="55d42-138">deviceId</span></span>|<span data-ttu-id="55d42-139">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="55d42-139">String</span></span>|<span data-ttu-id="55d42-140">ID de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="55d42-140">Device ID.</span></span>|
|<span data-ttu-id="55d42-141">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="55d42-141">lastSyncDateTime</span></span>|<span data-ttu-id="55d42-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="55d42-142">DateTimeOffset</span></span>|<span data-ttu-id="55d42-143">Hora da data da última sincronização.</span><span class="sxs-lookup"><span data-stu-id="55d42-143">Last sync date time.</span></span>|
|<span data-ttu-id="55d42-144">osVersion</span><span class="sxs-lookup"><span data-stu-id="55d42-144">osVersion</span></span>|<span data-ttu-id="55d42-145">String</span><span class="sxs-lookup"><span data-stu-id="55d42-145">String</span></span>|<span data-ttu-id="55d42-146">Versão do sistema operacional Windows.</span><span class="sxs-lookup"><span data-stu-id="55d42-146">Windows OS Version.</span></span>|
|<span data-ttu-id="55d42-147">osDescription</span><span class="sxs-lookup"><span data-stu-id="55d42-147">osDescription</span></span>|<span data-ttu-id="55d42-148">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="55d42-148">String</span></span>|<span data-ttu-id="55d42-149">Descrição da versão do sistema operacional Windows.</span><span class="sxs-lookup"><span data-stu-id="55d42-149">Windows OS Version Description.</span></span>|
|<span data-ttu-id="55d42-150">deploymentStatus</span><span class="sxs-lookup"><span data-stu-id="55d42-150">deploymentStatus</span></span>|[<span data-ttu-id="55d42-151">windowsDefenderApplicationControlSupplementalPolicyStatuses</span><span class="sxs-lookup"><span data-stu-id="55d42-151">windowsDefenderApplicationControlSupplementalPolicyStatuses</span></span>](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicystatuses.md)|<span data-ttu-id="55d42-152">O estado de implantação da política.</span><span class="sxs-lookup"><span data-stu-id="55d42-152">The deployment state of the policy.</span></span> <span data-ttu-id="55d42-153">Os valores possíveis são: `unknown`, `success`, `tokenError`, `notAuthorizedByToken`, `policyNotFound`.</span><span class="sxs-lookup"><span data-stu-id="55d42-153">Possible values are: `unknown`, `success`, `tokenError`, `notAuthorizedByToken`, `policyNotFound`.</span></span>|
|<span data-ttu-id="55d42-154">userName</span><span class="sxs-lookup"><span data-stu-id="55d42-154">userName</span></span>|<span data-ttu-id="55d42-155">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="55d42-155">String</span></span>|<span data-ttu-id="55d42-156">O nome do usuário deste dispositivo.</span><span class="sxs-lookup"><span data-stu-id="55d42-156">The name of the user of this device.</span></span>|
|<span data-ttu-id="55d42-157">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="55d42-157">userPrincipalName</span></span>|<span data-ttu-id="55d42-158">String</span><span class="sxs-lookup"><span data-stu-id="55d42-158">String</span></span>|<span data-ttu-id="55d42-159">Nome principal do usuário.</span><span class="sxs-lookup"><span data-stu-id="55d42-159">User Principal Name.</span></span>|
|<span data-ttu-id="55d42-160">policyVersion</span><span class="sxs-lookup"><span data-stu-id="55d42-160">policyVersion</span></span>|<span data-ttu-id="55d42-161">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="55d42-161">String</span></span>|<span data-ttu-id="55d42-162">Versão de leitura humana da política complementar do WindowsDefenderApplicationControl.</span><span class="sxs-lookup"><span data-stu-id="55d42-162">Human readable version of the WindowsDefenderApplicationControl supplemental policy.</span></span>|



## <a name="response"></a><span data-ttu-id="55d42-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="55d42-163">Response</span></span>
<span data-ttu-id="55d42-164">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="55d42-164">If successful, this method returns a `201 Created` response code and a [windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="55d42-165">Exemplo</span><span class="sxs-lookup"><span data-stu-id="55d42-165">Example</span></span>

### <a name="request"></a><span data-ttu-id="55d42-166">Solicitação</span><span class="sxs-lookup"><span data-stu-id="55d42-166">Request</span></span>
<span data-ttu-id="55d42-167">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="55d42-167">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="55d42-168">Resposta</span><span class="sxs-lookup"><span data-stu-id="55d42-168">Response</span></span>
<span data-ttu-id="55d42-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="55d42-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





