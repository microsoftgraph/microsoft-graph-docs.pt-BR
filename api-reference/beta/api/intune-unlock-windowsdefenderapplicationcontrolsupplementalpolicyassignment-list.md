---
title: Listar windowsDefenderApplicationControlSupplementalPolicyAssignments
description: Listar Propriedades e relações dos objetos windowsDefenderApplicationControlSupplementalPolicyAssignment.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 5e8d70be8ca56682813402105f88b21db46b7ed1
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39938744"
---
# <a name="list-windowsdefenderapplicationcontrolsupplementalpolicyassignments"></a><span data-ttu-id="c1ee0-103">Listar windowsDefenderApplicationControlSupplementalPolicyAssignments</span><span class="sxs-lookup"><span data-stu-id="c1ee0-103">List windowsDefenderApplicationControlSupplementalPolicyAssignments</span></span>

> <span data-ttu-id="c1ee0-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c1ee0-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c1ee0-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c1ee0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c1ee0-106">Listar Propriedades e relações dos objetos [windowsDefenderApplicationControlSupplementalPolicyAssignment](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicyassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="c1ee0-106">List properties and relationships of the [windowsDefenderApplicationControlSupplementalPolicyAssignment](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicyassignment.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c1ee0-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c1ee0-107">Prerequisites</span></span>
<span data-ttu-id="c1ee0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c1ee0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c1ee0-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c1ee0-110">Permission type</span></span>|<span data-ttu-id="c1ee0-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="c1ee0-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c1ee0-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c1ee0-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c1ee0-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="c1ee0-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="c1ee0-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c1ee0-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c1ee0-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c1ee0-115">Not supported.</span></span>|
|<span data-ttu-id="c1ee0-116">Application</span><span class="sxs-lookup"><span data-stu-id="c1ee0-116">Application</span></span>|<span data-ttu-id="c1ee0-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="c1ee0-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c1ee0-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c1ee0-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/wdacSupplementalPolicies/{windowsDefenderApplicationControlSupplementalPolicyId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="c1ee0-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c1ee0-119">Request headers</span></span>
|<span data-ttu-id="c1ee0-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c1ee0-120">Header</span></span>|<span data-ttu-id="c1ee0-121">Valor</span><span class="sxs-lookup"><span data-stu-id="c1ee0-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c1ee0-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="c1ee0-122">Authorization</span></span>|<span data-ttu-id="c1ee0-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c1ee0-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c1ee0-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="c1ee0-124">Accept</span></span>|<span data-ttu-id="c1ee0-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c1ee0-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c1ee0-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c1ee0-126">Request body</span></span>
<span data-ttu-id="c1ee0-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c1ee0-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c1ee0-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="c1ee0-128">Response</span></span>
<span data-ttu-id="c1ee0-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [windowsDefenderApplicationControlSupplementalPolicyAssignment](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicyassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c1ee0-129">If successful, this method returns a `200 OK` response code and a collection of [windowsDefenderApplicationControlSupplementalPolicyAssignment](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicyassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c1ee0-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c1ee0-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="c1ee0-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c1ee0-131">Request</span></span>
<span data-ttu-id="c1ee0-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c1ee0-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/wdacSupplementalPolicies/{windowsDefenderApplicationControlSupplementalPolicyId}/assignments
```

### <a name="response"></a><span data-ttu-id="c1ee0-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="c1ee0-133">Response</span></span>
<span data-ttu-id="c1ee0-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c1ee0-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 303

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsDefenderApplicationControlSupplementalPolicyAssignment",
      "id": "5e299ff3-9ff3-5e29-f39f-295ef39f295e",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      }
    }
  ]
}
```





