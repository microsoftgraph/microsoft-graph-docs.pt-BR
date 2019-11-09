---
title: Obter windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus
description: Leia as propriedades e as relações do objeto windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 379abe8be1e96cbc2a3e4333b4b742a24e3f077c
ms.sourcegitcommit: 5b1fad41067629d0e9f87746328664bb248f754f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/09/2019
ms.locfileid: "38087976"
---
# <a name="get-windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus"></a><span data-ttu-id="7e484-103">Obter windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus</span><span class="sxs-lookup"><span data-stu-id="7e484-103">Get windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus</span></span>

> <span data-ttu-id="7e484-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="7e484-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7e484-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="7e484-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7e484-106">Leia as propriedades e as relações do objeto [windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus.md) .</span><span class="sxs-lookup"><span data-stu-id="7e484-106">Read properties and relationships of the [windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7e484-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="7e484-107">Prerequisites</span></span>
<span data-ttu-id="7e484-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7e484-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7e484-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7e484-110">Permission type</span></span>|<span data-ttu-id="7e484-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="7e484-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7e484-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7e484-112">Delegated (work or school account)</span></span>|<span data-ttu-id="7e484-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="7e484-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="7e484-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7e484-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7e484-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7e484-115">Not supported.</span></span>|
|<span data-ttu-id="7e484-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7e484-116">Application</span></span>|<span data-ttu-id="7e484-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="7e484-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7e484-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7e484-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/wdacSupplementalPolicies/{windowsDefenderApplicationControlSupplementalPolicyId}/deviceStatuses/{windowsDefenderApplicationControlSupplementalPolicyDeploymentStatusId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7e484-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="7e484-119">Optional query parameters</span></span>
<span data-ttu-id="7e484-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="7e484-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7e484-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7e484-121">Request headers</span></span>
|<span data-ttu-id="7e484-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="7e484-122">Header</span></span>|<span data-ttu-id="7e484-123">Valor</span><span class="sxs-lookup"><span data-stu-id="7e484-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7e484-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="7e484-124">Authorization</span></span>|<span data-ttu-id="7e484-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7e484-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7e484-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="7e484-126">Accept</span></span>|<span data-ttu-id="7e484-127">application/json</span><span class="sxs-lookup"><span data-stu-id="7e484-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7e484-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7e484-128">Request body</span></span>
<span data-ttu-id="7e484-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7e484-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7e484-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="7e484-130">Response</span></span>
<span data-ttu-id="7e484-131">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7e484-131">If successful, this method returns a `200 OK` response code and [windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7e484-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7e484-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="7e484-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7e484-133">Request</span></span>
<span data-ttu-id="7e484-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7e484-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/wdacSupplementalPolicies/{windowsDefenderApplicationControlSupplementalPolicyId}/deviceStatuses/{windowsDefenderApplicationControlSupplementalPolicyDeploymentStatusId}
```

### <a name="response"></a><span data-ttu-id="7e484-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="7e484-135">Response</span></span>
<span data-ttu-id="7e484-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7e484-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 576

{
  "value": {
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
}
```






