---
title: Listar windowsDefenderApplicationControlSupplementalPolicyDeploymentStatuses
description: Listar propriedades e relações dos objetos windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 122c90d2be1e105d40d308f3a0457771d6c2e9d4
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51133916"
---
# <a name="list-windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatuses"></a><span data-ttu-id="a9b81-103">Listar windowsDefenderApplicationControlSupplementalPolicyDeploymentStatuses</span><span class="sxs-lookup"><span data-stu-id="a9b81-103">List windowsDefenderApplicationControlSupplementalPolicyDeploymentStatuses</span></span>

<span data-ttu-id="a9b81-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a9b81-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a9b81-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a9b81-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a9b81-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a9b81-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a9b81-107">Listar propriedades e relações dos [objetos windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus.](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus.md)</span><span class="sxs-lookup"><span data-stu-id="a9b81-107">List properties and relationships of the [windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a9b81-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a9b81-108">Prerequisites</span></span>
<span data-ttu-id="a9b81-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a9b81-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a9b81-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a9b81-111">Permission type</span></span>|<span data-ttu-id="a9b81-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a9b81-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a9b81-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a9b81-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a9b81-114">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a9b81-114">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="a9b81-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a9b81-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a9b81-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a9b81-116">Not supported.</span></span>|
|<span data-ttu-id="a9b81-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a9b81-117">Application</span></span>|<span data-ttu-id="a9b81-118">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a9b81-118">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a9b81-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a9b81-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/wdacSupplementalPolicies/{windowsDefenderApplicationControlSupplementalPolicyId}/deviceStatuses
```

## <a name="request-headers"></a><span data-ttu-id="a9b81-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a9b81-120">Request headers</span></span>
|<span data-ttu-id="a9b81-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a9b81-121">Header</span></span>|<span data-ttu-id="a9b81-122">Valor</span><span class="sxs-lookup"><span data-stu-id="a9b81-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a9b81-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="a9b81-123">Authorization</span></span>|<span data-ttu-id="a9b81-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a9b81-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a9b81-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a9b81-125">Accept</span></span>|<span data-ttu-id="a9b81-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a9b81-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a9b81-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a9b81-127">Request body</span></span>
<span data-ttu-id="a9b81-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a9b81-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a9b81-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="a9b81-129">Response</span></span>
<span data-ttu-id="a9b81-130">Se tiver êxito, este método retornará um código de resposta e uma coleção de objetos `200 OK` [windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a9b81-130">If successful, this method returns a `200 OK` response code and a collection of [windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a9b81-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a9b81-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="a9b81-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a9b81-132">Request</span></span>
<span data-ttu-id="a9b81-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a9b81-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/wdacSupplementalPolicies/{windowsDefenderApplicationControlSupplementalPolicyId}/deviceStatuses
```

### <a name="response"></a><span data-ttu-id="a9b81-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="a9b81-134">Response</span></span>
<span data-ttu-id="a9b81-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a9b81-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 612

{
  "value": [
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
  ]
}
```




