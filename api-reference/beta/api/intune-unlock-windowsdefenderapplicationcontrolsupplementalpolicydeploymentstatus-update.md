---
title: Atualizar windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus
description: Atualiza as propriedades de um objeto windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: ab3520c70898d893eaa3c836f8663fd0ed5ce813
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42457479"
---
# <a name="update-windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus"></a><span data-ttu-id="02d84-103">Atualizar windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus</span><span class="sxs-lookup"><span data-stu-id="02d84-103">Update windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus</span></span>

<span data-ttu-id="02d84-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="02d84-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="02d84-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="02d84-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="02d84-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="02d84-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="02d84-107">Atualiza as propriedades de um objeto [windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus.md) .</span><span class="sxs-lookup"><span data-stu-id="02d84-107">Update the properties of a [windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="02d84-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="02d84-108">Prerequisites</span></span>
<span data-ttu-id="02d84-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="02d84-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="02d84-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="02d84-111">Permission type</span></span>|<span data-ttu-id="02d84-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="02d84-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="02d84-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="02d84-113">Delegated (work or school account)</span></span>|<span data-ttu-id="02d84-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="02d84-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="02d84-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="02d84-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="02d84-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="02d84-116">Not supported.</span></span>|
|<span data-ttu-id="02d84-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="02d84-117">Application</span></span>|<span data-ttu-id="02d84-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="02d84-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="02d84-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="02d84-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/wdacSupplementalPolicies/{windowsDefenderApplicationControlSupplementalPolicyId}/deviceStatuses/{windowsDefenderApplicationControlSupplementalPolicyDeploymentStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="02d84-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="02d84-120">Request headers</span></span>
|<span data-ttu-id="02d84-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="02d84-121">Header</span></span>|<span data-ttu-id="02d84-122">Valor</span><span class="sxs-lookup"><span data-stu-id="02d84-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="02d84-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="02d84-123">Authorization</span></span>|<span data-ttu-id="02d84-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="02d84-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="02d84-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="02d84-125">Accept</span></span>|<span data-ttu-id="02d84-126">application/json</span><span class="sxs-lookup"><span data-stu-id="02d84-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="02d84-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="02d84-127">Request body</span></span>
<span data-ttu-id="02d84-128">No corpo da solicitação, forneça uma representação JSON do objeto [windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus.md) .</span><span class="sxs-lookup"><span data-stu-id="02d84-128">In the request body, supply a JSON representation for the [windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus.md) object.</span></span>

<span data-ttu-id="02d84-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus.md).</span><span class="sxs-lookup"><span data-stu-id="02d84-129">The following table shows the properties that are required when you create the [windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus.md).</span></span>

|<span data-ttu-id="02d84-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="02d84-130">Property</span></span>|<span data-ttu-id="02d84-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="02d84-131">Type</span></span>|<span data-ttu-id="02d84-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="02d84-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="02d84-133">id</span><span class="sxs-lookup"><span data-stu-id="02d84-133">id</span></span>|<span data-ttu-id="02d84-134">String</span><span class="sxs-lookup"><span data-stu-id="02d84-134">String</span></span>|<span data-ttu-id="02d84-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="02d84-135">Key of the entity.</span></span>|
|<span data-ttu-id="02d84-136">deviceName</span><span class="sxs-lookup"><span data-stu-id="02d84-136">deviceName</span></span>|<span data-ttu-id="02d84-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="02d84-137">String</span></span>|<span data-ttu-id="02d84-138">Nome do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="02d84-138">Device name.</span></span>|
|<span data-ttu-id="02d84-139">deviceId</span><span class="sxs-lookup"><span data-stu-id="02d84-139">deviceId</span></span>|<span data-ttu-id="02d84-140">String</span><span class="sxs-lookup"><span data-stu-id="02d84-140">String</span></span>|<span data-ttu-id="02d84-141">ID de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="02d84-141">Device ID.</span></span>|
|<span data-ttu-id="02d84-142">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="02d84-142">lastSyncDateTime</span></span>|<span data-ttu-id="02d84-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="02d84-143">DateTimeOffset</span></span>|<span data-ttu-id="02d84-144">Hora da data da última sincronização.</span><span class="sxs-lookup"><span data-stu-id="02d84-144">Last sync date time.</span></span>|
|<span data-ttu-id="02d84-145">osVersion</span><span class="sxs-lookup"><span data-stu-id="02d84-145">osVersion</span></span>|<span data-ttu-id="02d84-146">String</span><span class="sxs-lookup"><span data-stu-id="02d84-146">String</span></span>|<span data-ttu-id="02d84-147">Versão do sistema operacional Windows.</span><span class="sxs-lookup"><span data-stu-id="02d84-147">Windows OS Version.</span></span>|
|<span data-ttu-id="02d84-148">osDescription</span><span class="sxs-lookup"><span data-stu-id="02d84-148">osDescription</span></span>|<span data-ttu-id="02d84-149">String</span><span class="sxs-lookup"><span data-stu-id="02d84-149">String</span></span>|<span data-ttu-id="02d84-150">Descrição da versão do sistema operacional Windows.</span><span class="sxs-lookup"><span data-stu-id="02d84-150">Windows OS Version Description.</span></span>|
|<span data-ttu-id="02d84-151">deploymentStatus</span><span class="sxs-lookup"><span data-stu-id="02d84-151">deploymentStatus</span></span>|[<span data-ttu-id="02d84-152">windowsDefenderApplicationControlSupplementalPolicyStatuses</span><span class="sxs-lookup"><span data-stu-id="02d84-152">windowsDefenderApplicationControlSupplementalPolicyStatuses</span></span>](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicystatuses.md)|<span data-ttu-id="02d84-153">O estado de implantação da política.</span><span class="sxs-lookup"><span data-stu-id="02d84-153">The deployment state of the policy.</span></span> <span data-ttu-id="02d84-154">Os valores possíveis são: `unknown`, `success`, `tokenError`, `notAuthorizedByToken`, `policyNotFound`.</span><span class="sxs-lookup"><span data-stu-id="02d84-154">Possible values are: `unknown`, `success`, `tokenError`, `notAuthorizedByToken`, `policyNotFound`.</span></span>|
|<span data-ttu-id="02d84-155">userName</span><span class="sxs-lookup"><span data-stu-id="02d84-155">userName</span></span>|<span data-ttu-id="02d84-156">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="02d84-156">String</span></span>|<span data-ttu-id="02d84-157">O nome do usuário deste dispositivo.</span><span class="sxs-lookup"><span data-stu-id="02d84-157">The name of the user of this device.</span></span>|
|<span data-ttu-id="02d84-158">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="02d84-158">userPrincipalName</span></span>|<span data-ttu-id="02d84-159">String</span><span class="sxs-lookup"><span data-stu-id="02d84-159">String</span></span>|<span data-ttu-id="02d84-160">Nome principal do usuário.</span><span class="sxs-lookup"><span data-stu-id="02d84-160">User Principal Name.</span></span>|
|<span data-ttu-id="02d84-161">policyVersion</span><span class="sxs-lookup"><span data-stu-id="02d84-161">policyVersion</span></span>|<span data-ttu-id="02d84-162">String</span><span class="sxs-lookup"><span data-stu-id="02d84-162">String</span></span>|<span data-ttu-id="02d84-163">Versão de leitura humana da política complementar do WindowsDefenderApplicationControl.</span><span class="sxs-lookup"><span data-stu-id="02d84-163">Human readable version of the WindowsDefenderApplicationControl supplemental policy.</span></span>|



## <a name="response"></a><span data-ttu-id="02d84-164">Resposta</span><span class="sxs-lookup"><span data-stu-id="02d84-164">Response</span></span>
<span data-ttu-id="02d84-165">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="02d84-165">If successful, this method returns a `200 OK` response code and an updated [windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="02d84-166">Exemplo</span><span class="sxs-lookup"><span data-stu-id="02d84-166">Example</span></span>

### <a name="request"></a><span data-ttu-id="02d84-167">Solicitação</span><span class="sxs-lookup"><span data-stu-id="02d84-167">Request</span></span>
<span data-ttu-id="02d84-168">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="02d84-168">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/wdacSupplementalPolicies/{windowsDefenderApplicationControlSupplementalPolicyId}/deviceStatuses/{windowsDefenderApplicationControlSupplementalPolicyDeploymentStatusId}
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

### <a name="response"></a><span data-ttu-id="02d84-169">Resposta</span><span class="sxs-lookup"><span data-stu-id="02d84-169">Response</span></span>
<span data-ttu-id="02d84-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="02d84-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





