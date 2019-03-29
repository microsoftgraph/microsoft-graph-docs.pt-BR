---
title: Listar deviceCompliancePolicyAssignments
description: Listar propriedades e relações dos objetosdeviceCompliancePolicyAssignment.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 854fd1d53ff2bbc4263fb866994b680847e9b9b4
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/29/2019
ms.locfileid: "30982249"
---
# <a name="list-devicecompliancepolicyassignments"></a><span data-ttu-id="80913-103">Listar deviceCompliancePolicyAssignments</span><span class="sxs-lookup"><span data-stu-id="80913-103">List deviceCompliancePolicyAssignments</span></span>

> <span data-ttu-id="80913-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="80913-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="80913-105">Listar propriedades e relações dos objetos[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md).</span><span class="sxs-lookup"><span data-stu-id="80913-105">List properties and relationships of the [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="80913-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="80913-106">Prerequisites</span></span>
<span data-ttu-id="80913-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="80913-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="80913-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="80913-109">Permission type</span></span>|<span data-ttu-id="80913-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="80913-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="80913-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="80913-111">Delegated (work or school account)</span></span>|<span data-ttu-id="80913-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="80913-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="80913-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="80913-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="80913-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="80913-114">Not supported.</span></span>|
|<span data-ttu-id="80913-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="80913-115">Application</span></span>|<span data-ttu-id="80913-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="80913-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="80913-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="80913-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="80913-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="80913-118">Request headers</span></span>
|<span data-ttu-id="80913-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="80913-119">Header</span></span>|<span data-ttu-id="80913-120">Valor</span><span class="sxs-lookup"><span data-stu-id="80913-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="80913-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="80913-121">Authorization</span></span>|<span data-ttu-id="80913-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="80913-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="80913-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="80913-123">Accept</span></span>|<span data-ttu-id="80913-124">application/json</span><span class="sxs-lookup"><span data-stu-id="80913-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="80913-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="80913-125">Request body</span></span>
<span data-ttu-id="80913-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="80913-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="80913-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="80913-127">Response</span></span>
<span data-ttu-id="80913-128">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="80913-128">If successful, this method returns a `200 OK` response code and a collection of [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="80913-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="80913-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="80913-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="80913-130">Request</span></span>
<span data-ttu-id="80913-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="80913-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/assignments
```

### <a name="response"></a><span data-ttu-id="80913-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="80913-132">Response</span></span>
<span data-ttu-id="80913-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="80913-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 274

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceCompliancePolicyAssignment",
      "id": "92dc3fef-3fef-92dc-ef3f-dc92ef3fdc92",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      }
    }
  ]
}
```



