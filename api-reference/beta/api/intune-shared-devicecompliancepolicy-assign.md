---
title: atribuir ação
description: Ainda não documentado
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: dbb4e60a65ddfde71bca07134a3ed7acb93e63c9
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39940128"
---
# <a name="assign-action"></a><span data-ttu-id="1c444-103">atribuir ação</span><span class="sxs-lookup"><span data-stu-id="1c444-103">assign action</span></span>

> <span data-ttu-id="1c444-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="1c444-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1c444-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1c444-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1c444-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="1c444-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1c444-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="1c444-107">Prerequisites</span></span>
<span data-ttu-id="1c444-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1c444-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1c444-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1c444-110">Permission type</span></span>|<span data-ttu-id="1c444-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="1c444-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1c444-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1c444-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="1c444-113">&nbsp; &nbsp; **Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="1c444-113">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="1c444-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1c444-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="1c444-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1c444-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1c444-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1c444-116">Not supported.</span></span>|
|<span data-ttu-id="1c444-117">Application</span><span class="sxs-lookup"><span data-stu-id="1c444-117">Application</span></span>||
| <span data-ttu-id="1c444-118">&nbsp; &nbsp; **Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="1c444-118">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="1c444-119">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1c444-119">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1c444-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1c444-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="1c444-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1c444-121">Request headers</span></span>
|<span data-ttu-id="1c444-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1c444-122">Header</span></span>|<span data-ttu-id="1c444-123">Valor</span><span class="sxs-lookup"><span data-stu-id="1c444-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1c444-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="1c444-124">Authorization</span></span>|<span data-ttu-id="1c444-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1c444-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1c444-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="1c444-126">Accept</span></span>|<span data-ttu-id="1c444-127">application/json</span><span class="sxs-lookup"><span data-stu-id="1c444-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1c444-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1c444-128">Request body</span></span>
<span data-ttu-id="1c444-129">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="1c444-129">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="1c444-130">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="1c444-130">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="1c444-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1c444-131">Property</span></span>|<span data-ttu-id="1c444-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="1c444-132">Type</span></span>|<span data-ttu-id="1c444-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="1c444-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1c444-134">assignments</span><span class="sxs-lookup"><span data-stu-id="1c444-134">assignments</span></span>|<span data-ttu-id="1c444-135">Coleção [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md)</span><span class="sxs-lookup"><span data-stu-id="1c444-135">[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) collection</span></span>|<span data-ttu-id="1c444-136">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="1c444-136">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="1c444-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="1c444-137">Response</span></span>
<span data-ttu-id="1c444-138">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1c444-138">If successful, this action returns a `200 OK` response code and a [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1c444-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1c444-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="1c444-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1c444-140">Request</span></span>
<span data-ttu-id="1c444-141">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1c444-141">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="1c444-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="1c444-142">Response</span></span>
<span data-ttu-id="1c444-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1c444-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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








