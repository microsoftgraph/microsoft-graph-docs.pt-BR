---
title: Obter windowsDefenderApplicationControlSupplementalPolicyDeploymentSummary
description: Leia propriedades e relações do objeto windowsDefenderApplicationControlSupplementalPolicyDeploymentSummary.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 26d4b1944a55e44b6148a90e1c1612b37af8c045
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51133896"
---
# <a name="get-windowsdefenderapplicationcontrolsupplementalpolicydeploymentsummary"></a><span data-ttu-id="2a3dd-103">Obter windowsDefenderApplicationControlSupplementalPolicyDeploymentSummary</span><span class="sxs-lookup"><span data-stu-id="2a3dd-103">Get windowsDefenderApplicationControlSupplementalPolicyDeploymentSummary</span></span>

<span data-ttu-id="2a3dd-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2a3dd-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2a3dd-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="2a3dd-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2a3dd-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2a3dd-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2a3dd-107">Leia propriedades e relações do [objeto windowsDefenderApplicationControlSupplementalPolicyDeploymentSummary.](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentsummary.md)</span><span class="sxs-lookup"><span data-stu-id="2a3dd-107">Read properties and relationships of the [windowsDefenderApplicationControlSupplementalPolicyDeploymentSummary](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2a3dd-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="2a3dd-108">Prerequisites</span></span>
<span data-ttu-id="2a3dd-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2a3dd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2a3dd-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2a3dd-111">Permission type</span></span>|<span data-ttu-id="2a3dd-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2a3dd-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2a3dd-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2a3dd-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2a3dd-114">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2a3dd-114">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="2a3dd-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2a3dd-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2a3dd-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2a3dd-116">Not supported.</span></span>|
|<span data-ttu-id="2a3dd-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2a3dd-117">Application</span></span>|<span data-ttu-id="2a3dd-118">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2a3dd-118">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2a3dd-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2a3dd-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/wdacSupplementalPolicies/{windowsDefenderApplicationControlSupplementalPolicyId}/deploySummary
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2a3dd-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="2a3dd-120">Optional query parameters</span></span>
<span data-ttu-id="2a3dd-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="2a3dd-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2a3dd-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2a3dd-122">Request headers</span></span>
|<span data-ttu-id="2a3dd-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2a3dd-123">Header</span></span>|<span data-ttu-id="2a3dd-124">Valor</span><span class="sxs-lookup"><span data-stu-id="2a3dd-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2a3dd-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="2a3dd-125">Authorization</span></span>|<span data-ttu-id="2a3dd-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2a3dd-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2a3dd-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="2a3dd-127">Accept</span></span>|<span data-ttu-id="2a3dd-128">application/json</span><span class="sxs-lookup"><span data-stu-id="2a3dd-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2a3dd-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2a3dd-129">Request body</span></span>
<span data-ttu-id="2a3dd-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="2a3dd-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2a3dd-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="2a3dd-131">Response</span></span>
<span data-ttu-id="2a3dd-132">Se tiver êxito, este método retornará um código de resposta e um objeto `200 OK` [windowsDefenderApplicationControlSupplementalPolicyDeploymentSummary](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentsummary.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2a3dd-132">If successful, this method returns a `200 OK` response code and [windowsDefenderApplicationControlSupplementalPolicyDeploymentSummary](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2a3dd-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2a3dd-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="2a3dd-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2a3dd-134">Request</span></span>
<span data-ttu-id="2a3dd-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2a3dd-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/wdacSupplementalPolicies/{windowsDefenderApplicationControlSupplementalPolicyId}/deploySummary
```

### <a name="response"></a><span data-ttu-id="2a3dd-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="2a3dd-136">Response</span></span>
<span data-ttu-id="2a3dd-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2a3dd-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 242

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsDefenderApplicationControlSupplementalPolicyDeploymentSummary",
    "id": "2f8656ed-56ed-2f86-ed56-862fed56862f",
    "deployedDeviceCount": 3,
    "failedDeviceCount": 1
  }
}
```




