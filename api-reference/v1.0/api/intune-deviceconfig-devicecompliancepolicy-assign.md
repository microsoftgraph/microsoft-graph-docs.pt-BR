---
title: atribuir ação
description: Ainda não documentado
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: fa354796f555e0b2255bded84bf411a7d64a868a
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/26/2019
ms.locfileid: "30250135"
---
# <a name="assign-action"></a><span data-ttu-id="307e3-103">atribuir ação</span><span class="sxs-lookup"><span data-stu-id="307e3-103">assign action</span></span>

> <span data-ttu-id="307e3-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="307e3-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="307e3-105">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="307e3-105">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="307e3-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="307e3-106">Prerequisites</span></span>
<span data-ttu-id="307e3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="307e3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="307e3-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="307e3-109">Permission type</span></span>|<span data-ttu-id="307e3-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="307e3-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="307e3-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="307e3-111">Delegated (work or school account)</span></span>|<span data-ttu-id="307e3-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="307e3-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="307e3-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="307e3-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="307e3-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="307e3-114">Not supported.</span></span>|
|<span data-ttu-id="307e3-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="307e3-115">Application</span></span>|<span data-ttu-id="307e3-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="307e3-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="307e3-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="307e3-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="307e3-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="307e3-118">Request headers</span></span>
|<span data-ttu-id="307e3-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="307e3-119">Header</span></span>|<span data-ttu-id="307e3-120">Valor</span><span class="sxs-lookup"><span data-stu-id="307e3-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="307e3-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="307e3-121">Authorization</span></span>|<span data-ttu-id="307e3-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="307e3-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="307e3-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="307e3-123">Accept</span></span>|<span data-ttu-id="307e3-124">application/json</span><span class="sxs-lookup"><span data-stu-id="307e3-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="307e3-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="307e3-125">Request body</span></span>
<span data-ttu-id="307e3-126">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="307e3-126">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="307e3-127">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="307e3-127">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="307e3-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="307e3-128">Property</span></span>|<span data-ttu-id="307e3-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="307e3-129">Type</span></span>|<span data-ttu-id="307e3-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="307e3-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="307e3-131">assignments</span><span class="sxs-lookup"><span data-stu-id="307e3-131">assignments</span></span>|<span data-ttu-id="307e3-132">Coleção [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md)</span><span class="sxs-lookup"><span data-stu-id="307e3-132">[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) collection</span></span>|<span data-ttu-id="307e3-133">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="307e3-133">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="307e3-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="307e3-134">Response</span></span>
<span data-ttu-id="307e3-135">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="307e3-135">If successful, this action returns a `200 OK` response code and a [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="307e3-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="307e3-136">Example</span></span>

### <a name="request"></a><span data-ttu-id="307e3-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="307e3-137">Request</span></span>
<span data-ttu-id="307e3-138">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="307e3-138">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="307e3-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="307e3-139">Response</span></span>
<span data-ttu-id="307e3-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="307e3-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



