---
title: atribuir ação
description: Ainda não documentado
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3708c956f447098a7aee694c52eb61372e9b1b14
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34968466"
---
# <a name="assign-action"></a><span data-ttu-id="69236-103">atribuir ação</span><span class="sxs-lookup"><span data-stu-id="69236-103">assign action</span></span>

> <span data-ttu-id="69236-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="69236-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="69236-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="69236-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="69236-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="69236-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="69236-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="69236-107">Prerequisites</span></span>
<span data-ttu-id="69236-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="69236-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="69236-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="69236-110">Permission type</span></span>|<span data-ttu-id="69236-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="69236-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="69236-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="69236-112">Delegated (work or school account)</span></span>|<span data-ttu-id="69236-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="69236-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="69236-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="69236-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="69236-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="69236-115">Not supported.</span></span>|
|<span data-ttu-id="69236-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="69236-116">Application</span></span>|<span data-ttu-id="69236-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="69236-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="69236-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="69236-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="69236-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="69236-119">Request headers</span></span>
|<span data-ttu-id="69236-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="69236-120">Header</span></span>|<span data-ttu-id="69236-121">Valor</span><span class="sxs-lookup"><span data-stu-id="69236-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="69236-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="69236-122">Authorization</span></span>|<span data-ttu-id="69236-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="69236-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="69236-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="69236-124">Accept</span></span>|<span data-ttu-id="69236-125">application/json</span><span class="sxs-lookup"><span data-stu-id="69236-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="69236-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="69236-126">Request body</span></span>
<span data-ttu-id="69236-127">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="69236-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="69236-128">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="69236-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="69236-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="69236-129">Property</span></span>|<span data-ttu-id="69236-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="69236-130">Type</span></span>|<span data-ttu-id="69236-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="69236-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="69236-132">assignments</span><span class="sxs-lookup"><span data-stu-id="69236-132">assignments</span></span>|<span data-ttu-id="69236-133">Coleção [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md)</span><span class="sxs-lookup"><span data-stu-id="69236-133">[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) collection</span></span>|<span data-ttu-id="69236-134">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="69236-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="69236-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="69236-135">Response</span></span>
<span data-ttu-id="69236-136">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="69236-136">If successful, this action returns a `200 OK` response code and a [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="69236-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="69236-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="69236-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="69236-138">Request</span></span>
<span data-ttu-id="69236-139">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="69236-139">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/assign

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

### <a name="response"></a><span data-ttu-id="69236-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="69236-140">Response</span></span>
<span data-ttu-id="69236-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="69236-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





