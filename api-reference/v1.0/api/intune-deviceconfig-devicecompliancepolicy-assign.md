---
title: atribuir ação
description: Ainda não documentado
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 432ae60b3b4172a6b0f2fdf5322a1ef9dc2b6f15
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42515088"
---
# <a name="assign-action"></a><span data-ttu-id="1c7ca-103">atribuir ação</span><span class="sxs-lookup"><span data-stu-id="1c7ca-103">assign action</span></span>

<span data-ttu-id="1c7ca-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1c7ca-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1c7ca-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1c7ca-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1c7ca-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="1c7ca-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1c7ca-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="1c7ca-107">Prerequisites</span></span>
<span data-ttu-id="1c7ca-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1c7ca-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1c7ca-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1c7ca-110">Permission type</span></span>|<span data-ttu-id="1c7ca-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="1c7ca-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1c7ca-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1c7ca-112">Delegated (work or school account)</span></span>|<span data-ttu-id="1c7ca-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1c7ca-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="1c7ca-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1c7ca-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1c7ca-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1c7ca-115">Not supported.</span></span>|
|<span data-ttu-id="1c7ca-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1c7ca-116">Application</span></span>|<span data-ttu-id="1c7ca-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1c7ca-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1c7ca-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1c7ca-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="1c7ca-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1c7ca-119">Request headers</span></span>
|<span data-ttu-id="1c7ca-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1c7ca-120">Header</span></span>|<span data-ttu-id="1c7ca-121">Valor</span><span class="sxs-lookup"><span data-stu-id="1c7ca-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1c7ca-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="1c7ca-122">Authorization</span></span>|<span data-ttu-id="1c7ca-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1c7ca-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1c7ca-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="1c7ca-124">Accept</span></span>|<span data-ttu-id="1c7ca-125">application/json</span><span class="sxs-lookup"><span data-stu-id="1c7ca-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1c7ca-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1c7ca-126">Request body</span></span>
<span data-ttu-id="1c7ca-127">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="1c7ca-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="1c7ca-128">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="1c7ca-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="1c7ca-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1c7ca-129">Property</span></span>|<span data-ttu-id="1c7ca-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="1c7ca-130">Type</span></span>|<span data-ttu-id="1c7ca-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="1c7ca-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1c7ca-132">assignments</span><span class="sxs-lookup"><span data-stu-id="1c7ca-132">assignments</span></span>|<span data-ttu-id="1c7ca-133">Coleção [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md)</span><span class="sxs-lookup"><span data-stu-id="1c7ca-133">[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) collection</span></span>|<span data-ttu-id="1c7ca-134">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="1c7ca-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="1c7ca-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="1c7ca-135">Response</span></span>
<span data-ttu-id="1c7ca-136">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1c7ca-136">If successful, this action returns a `200 OK` response code and a [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1c7ca-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1c7ca-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="1c7ca-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1c7ca-138">Request</span></span>
<span data-ttu-id="1c7ca-139">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1c7ca-139">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="1c7ca-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="1c7ca-140">Response</span></span>
<span data-ttu-id="1c7ca-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1c7ca-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




