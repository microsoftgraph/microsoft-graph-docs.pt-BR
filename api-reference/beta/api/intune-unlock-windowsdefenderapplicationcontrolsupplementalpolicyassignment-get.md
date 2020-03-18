---
title: Obter windowsDefenderApplicationControlSupplementalPolicyAssignment
description: Leia as propriedades e as relações do objeto windowsDefenderApplicationControlSupplementalPolicyAssignment.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 524c330c0d66d5535b93fa70e146907f38e0d41b
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42799812"
---
# <a name="get-windowsdefenderapplicationcontrolsupplementalpolicyassignment"></a><span data-ttu-id="ca249-103">Obter windowsDefenderApplicationControlSupplementalPolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="ca249-103">Get windowsDefenderApplicationControlSupplementalPolicyAssignment</span></span>

> <span data-ttu-id="ca249-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ca249-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ca249-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ca249-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ca249-106">Leia as propriedades e as relações do objeto [windowsDefenderApplicationControlSupplementalPolicyAssignment](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicyassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="ca249-106">Read properties and relationships of the [windowsDefenderApplicationControlSupplementalPolicyAssignment](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicyassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ca249-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ca249-107">Prerequisites</span></span>
<span data-ttu-id="ca249-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ca249-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ca249-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ca249-110">Permission type</span></span>|<span data-ttu-id="ca249-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ca249-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ca249-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ca249-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ca249-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="ca249-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="ca249-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ca249-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ca249-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ca249-115">Not supported.</span></span>|
|<span data-ttu-id="ca249-116">Application</span><span class="sxs-lookup"><span data-stu-id="ca249-116">Application</span></span>|<span data-ttu-id="ca249-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="ca249-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ca249-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ca249-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/wdacSupplementalPolicies/{windowsDefenderApplicationControlSupplementalPolicyId}/assignments/{windowsDefenderApplicationControlSupplementalPolicyAssignmentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ca249-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="ca249-119">Optional query parameters</span></span>
<span data-ttu-id="ca249-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="ca249-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ca249-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ca249-121">Request headers</span></span>
|<span data-ttu-id="ca249-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ca249-122">Header</span></span>|<span data-ttu-id="ca249-123">Valor</span><span class="sxs-lookup"><span data-stu-id="ca249-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ca249-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="ca249-124">Authorization</span></span>|<span data-ttu-id="ca249-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ca249-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ca249-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ca249-126">Accept</span></span>|<span data-ttu-id="ca249-127">application/json</span><span class="sxs-lookup"><span data-stu-id="ca249-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ca249-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ca249-128">Request body</span></span>
<span data-ttu-id="ca249-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ca249-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ca249-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="ca249-130">Response</span></span>
<span data-ttu-id="ca249-131">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [windowsDefenderApplicationControlSupplementalPolicyAssignment](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicyassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ca249-131">If successful, this method returns a `200 OK` response code and [windowsDefenderApplicationControlSupplementalPolicyAssignment](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicyassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ca249-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ca249-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="ca249-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ca249-133">Request</span></span>
<span data-ttu-id="ca249-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ca249-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/wdacSupplementalPolicies/{windowsDefenderApplicationControlSupplementalPolicyId}/assignments/{windowsDefenderApplicationControlSupplementalPolicyAssignmentId}
```

### <a name="response"></a><span data-ttu-id="ca249-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="ca249-135">Response</span></span>
<span data-ttu-id="ca249-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ca249-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 279

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsDefenderApplicationControlSupplementalPolicyAssignment",
    "id": "5e299ff3-9ff3-5e29-f39f-295ef39f295e",
    "target": {
      "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
    }
  }
}
```




