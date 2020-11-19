---
title: atribuir ação
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: a4d0529997eeca13a6b809423499b050116a5207
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49257483"
---
# <a name="assign-action"></a><span data-ttu-id="9faf4-103">atribuir ação</span><span class="sxs-lookup"><span data-stu-id="9faf4-103">assign action</span></span>

<span data-ttu-id="9faf4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9faf4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9faf4-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="9faf4-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9faf4-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="9faf4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9faf4-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="9faf4-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9faf4-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="9faf4-108">Prerequisites</span></span>
<span data-ttu-id="9faf4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9faf4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9faf4-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9faf4-111">Permission type</span></span>|<span data-ttu-id="9faf4-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="9faf4-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9faf4-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9faf4-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="9faf4-114">&nbsp; &nbsp; **Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="9faf4-114">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="9faf4-115">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9faf4-115">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="9faf4-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9faf4-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9faf4-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9faf4-117">Not supported.</span></span>|
|<span data-ttu-id="9faf4-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9faf4-118">Application</span></span>||
| <span data-ttu-id="9faf4-119">&nbsp; &nbsp; **Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="9faf4-119">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="9faf4-120">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9faf4-120">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9faf4-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9faf4-121">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="9faf4-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9faf4-122">Request headers</span></span>
|<span data-ttu-id="9faf4-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9faf4-123">Header</span></span>|<span data-ttu-id="9faf4-124">Valor</span><span class="sxs-lookup"><span data-stu-id="9faf4-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9faf4-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="9faf4-125">Authorization</span></span>|<span data-ttu-id="9faf4-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9faf4-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9faf4-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="9faf4-127">Accept</span></span>|<span data-ttu-id="9faf4-128">application/json</span><span class="sxs-lookup"><span data-stu-id="9faf4-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9faf4-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9faf4-129">Request body</span></span>
<span data-ttu-id="9faf4-130">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="9faf4-130">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="9faf4-131">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="9faf4-131">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="9faf4-132">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9faf4-132">Property</span></span>|<span data-ttu-id="9faf4-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="9faf4-133">Type</span></span>|<span data-ttu-id="9faf4-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="9faf4-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9faf4-135">assignments</span><span class="sxs-lookup"><span data-stu-id="9faf4-135">assignments</span></span>|<span data-ttu-id="9faf4-136">Coleção [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md)</span><span class="sxs-lookup"><span data-stu-id="9faf4-136">[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) collection</span></span>|<span data-ttu-id="9faf4-137">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="9faf4-137">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="9faf4-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="9faf4-138">Response</span></span>
<span data-ttu-id="9faf4-139">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9faf4-139">If successful, this action returns a `200 OK` response code and a [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9faf4-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9faf4-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="9faf4-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9faf4-141">Request</span></span>
<span data-ttu-id="9faf4-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9faf4-142">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="9faf4-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="9faf4-143">Response</span></span>
<span data-ttu-id="9faf4-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9faf4-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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







