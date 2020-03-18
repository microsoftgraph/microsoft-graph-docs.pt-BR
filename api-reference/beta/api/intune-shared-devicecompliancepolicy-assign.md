---
title: atribuir ação
description: Ainda não documentado
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 1b864bb7d68132ee2ade2f5dc53e7005e07a3447
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42801212"
---
# <a name="assign-action"></a><span data-ttu-id="8c717-103">atribuir ação</span><span class="sxs-lookup"><span data-stu-id="8c717-103">assign action</span></span>

> <span data-ttu-id="8c717-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="8c717-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8c717-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="8c717-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8c717-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="8c717-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8c717-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="8c717-107">Prerequisites</span></span>
<span data-ttu-id="8c717-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8c717-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8c717-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8c717-110">Permission type</span></span>|<span data-ttu-id="8c717-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="8c717-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8c717-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8c717-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="8c717-113">&nbsp; &nbsp; **Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="8c717-113">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="8c717-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8c717-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8c717-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8c717-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8c717-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8c717-116">Not supported.</span></span>|
|<span data-ttu-id="8c717-117">Application</span><span class="sxs-lookup"><span data-stu-id="8c717-117">Application</span></span>||
| <span data-ttu-id="8c717-118">&nbsp; &nbsp; **Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="8c717-118">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="8c717-119">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8c717-119">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8c717-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8c717-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="8c717-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8c717-121">Request headers</span></span>
|<span data-ttu-id="8c717-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8c717-122">Header</span></span>|<span data-ttu-id="8c717-123">Valor</span><span class="sxs-lookup"><span data-stu-id="8c717-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8c717-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="8c717-124">Authorization</span></span>|<span data-ttu-id="8c717-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8c717-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8c717-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="8c717-126">Accept</span></span>|<span data-ttu-id="8c717-127">application/json</span><span class="sxs-lookup"><span data-stu-id="8c717-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8c717-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8c717-128">Request body</span></span>
<span data-ttu-id="8c717-129">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="8c717-129">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="8c717-130">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="8c717-130">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="8c717-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8c717-131">Property</span></span>|<span data-ttu-id="8c717-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="8c717-132">Type</span></span>|<span data-ttu-id="8c717-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="8c717-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8c717-134">assignments</span><span class="sxs-lookup"><span data-stu-id="8c717-134">assignments</span></span>|<span data-ttu-id="8c717-135">Coleção [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md)</span><span class="sxs-lookup"><span data-stu-id="8c717-135">[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) collection</span></span>|<span data-ttu-id="8c717-136">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="8c717-136">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="8c717-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="8c717-137">Response</span></span>
<span data-ttu-id="8c717-138">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8c717-138">If successful, this action returns a `200 OK` response code and a [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8c717-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8c717-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="8c717-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8c717-140">Request</span></span>
<span data-ttu-id="8c717-141">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8c717-141">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="8c717-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="8c717-142">Response</span></span>
<span data-ttu-id="8c717-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8c717-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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







