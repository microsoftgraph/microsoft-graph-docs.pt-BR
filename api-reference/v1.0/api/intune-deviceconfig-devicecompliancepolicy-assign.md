---
title: atribuir ação
description: Ainda não documentado
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b25039710d8f9382c5946bcb24c7c0a7a7c80af1
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/02/2019
ms.locfileid: "37354270"
---
# <a name="assign-action"></a><span data-ttu-id="7b88f-103">atribuir ação</span><span class="sxs-lookup"><span data-stu-id="7b88f-103">assign action</span></span>

> <span data-ttu-id="7b88f-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="7b88f-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7b88f-105">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="7b88f-105">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7b88f-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="7b88f-106">Prerequisites</span></span>
<span data-ttu-id="7b88f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7b88f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7b88f-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7b88f-109">Permission type</span></span>|<span data-ttu-id="7b88f-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="7b88f-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7b88f-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7b88f-111">Delegated (work or school account)</span></span>|<span data-ttu-id="7b88f-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7b88f-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="7b88f-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7b88f-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7b88f-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7b88f-114">Not supported.</span></span>|
|<span data-ttu-id="7b88f-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7b88f-115">Application</span></span>|<span data-ttu-id="7b88f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7b88f-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7b88f-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7b88f-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="7b88f-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7b88f-118">Request headers</span></span>
|<span data-ttu-id="7b88f-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="7b88f-119">Header</span></span>|<span data-ttu-id="7b88f-120">Valor</span><span class="sxs-lookup"><span data-stu-id="7b88f-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7b88f-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="7b88f-121">Authorization</span></span>|<span data-ttu-id="7b88f-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7b88f-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7b88f-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="7b88f-123">Accept</span></span>|<span data-ttu-id="7b88f-124">application/json</span><span class="sxs-lookup"><span data-stu-id="7b88f-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7b88f-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7b88f-125">Request body</span></span>
<span data-ttu-id="7b88f-126">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="7b88f-126">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="7b88f-127">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="7b88f-127">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="7b88f-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7b88f-128">Property</span></span>|<span data-ttu-id="7b88f-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="7b88f-129">Type</span></span>|<span data-ttu-id="7b88f-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="7b88f-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7b88f-131">assignments</span><span class="sxs-lookup"><span data-stu-id="7b88f-131">assignments</span></span>|<span data-ttu-id="7b88f-132">Coleção [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md)</span><span class="sxs-lookup"><span data-stu-id="7b88f-132">[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) collection</span></span>|<span data-ttu-id="7b88f-133">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="7b88f-133">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="7b88f-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="7b88f-134">Response</span></span>
<span data-ttu-id="7b88f-135">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7b88f-135">If successful, this action returns a `200 OK` response code and a [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7b88f-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7b88f-136">Example</span></span>

### <a name="request"></a><span data-ttu-id="7b88f-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7b88f-137">Request</span></span>
<span data-ttu-id="7b88f-138">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7b88f-138">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/assign

Content-type: application/json
Content-length: 280

{
  "assignments": [
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

### <a name="response"></a><span data-ttu-id="7b88f-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="7b88f-139">Response</span></span>
<span data-ttu-id="7b88f-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7b88f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




