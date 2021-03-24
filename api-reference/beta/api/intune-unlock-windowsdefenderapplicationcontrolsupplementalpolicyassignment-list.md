---
title: Listar windowsDefenderApplicationControlSupplementalPolicyAssignments
description: Listar propriedades e relações dos objetos windowsDefenderApplicationControlSupplementalPolicyAssignment.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 11606eefaeb6a7e33300612cdd8cf09b60808b5c
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51133973"
---
# <a name="list-windowsdefenderapplicationcontrolsupplementalpolicyassignments"></a><span data-ttu-id="99c19-103">Listar windowsDefenderApplicationControlSupplementalPolicyAssignments</span><span class="sxs-lookup"><span data-stu-id="99c19-103">List windowsDefenderApplicationControlSupplementalPolicyAssignments</span></span>

<span data-ttu-id="99c19-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="99c19-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="99c19-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="99c19-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="99c19-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="99c19-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="99c19-107">Listar propriedades e relações dos [objetos windowsDefenderApplicationControlSupplementalPolicyAssignment.](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicyassignment.md)</span><span class="sxs-lookup"><span data-stu-id="99c19-107">List properties and relationships of the [windowsDefenderApplicationControlSupplementalPolicyAssignment](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicyassignment.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="99c19-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="99c19-108">Prerequisites</span></span>
<span data-ttu-id="99c19-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="99c19-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="99c19-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="99c19-111">Permission type</span></span>|<span data-ttu-id="99c19-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="99c19-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="99c19-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="99c19-113">Delegated (work or school account)</span></span>|<span data-ttu-id="99c19-114">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="99c19-114">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="99c19-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="99c19-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="99c19-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="99c19-116">Not supported.</span></span>|
|<span data-ttu-id="99c19-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="99c19-117">Application</span></span>|<span data-ttu-id="99c19-118">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="99c19-118">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="99c19-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="99c19-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/wdacSupplementalPolicies/{windowsDefenderApplicationControlSupplementalPolicyId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="99c19-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="99c19-120">Request headers</span></span>
|<span data-ttu-id="99c19-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="99c19-121">Header</span></span>|<span data-ttu-id="99c19-122">Valor</span><span class="sxs-lookup"><span data-stu-id="99c19-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="99c19-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="99c19-123">Authorization</span></span>|<span data-ttu-id="99c19-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="99c19-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="99c19-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="99c19-125">Accept</span></span>|<span data-ttu-id="99c19-126">application/json</span><span class="sxs-lookup"><span data-stu-id="99c19-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="99c19-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="99c19-127">Request body</span></span>
<span data-ttu-id="99c19-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="99c19-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="99c19-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="99c19-129">Response</span></span>
<span data-ttu-id="99c19-130">Se tiver êxito, este método retornará um código de resposta e uma coleção de objetos `200 OK` [windowsDefenderApplicationControlSupplementalPolicyAssignment](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicyassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="99c19-130">If successful, this method returns a `200 OK` response code and a collection of [windowsDefenderApplicationControlSupplementalPolicyAssignment](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicyassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="99c19-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="99c19-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="99c19-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="99c19-132">Request</span></span>
<span data-ttu-id="99c19-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="99c19-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/wdacSupplementalPolicies/{windowsDefenderApplicationControlSupplementalPolicyId}/assignments
```

### <a name="response"></a><span data-ttu-id="99c19-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="99c19-134">Response</span></span>
<span data-ttu-id="99c19-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="99c19-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 478

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsDefenderApplicationControlSupplementalPolicyAssignment",
      "id": "5e299ff3-9ff3-5e29-f39f-295ef39f295e",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget",
        "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
        "deviceAndAppManagementAssignmentFilterType": "include"
      }
    }
  ]
}
```




