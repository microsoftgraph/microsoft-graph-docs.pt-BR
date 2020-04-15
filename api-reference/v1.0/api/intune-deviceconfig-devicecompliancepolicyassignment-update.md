---
title: Atualizar deviceCompliancePolicyAssignment
description: Atualizar as propriedades de um objeto deviceCompliancePolicyAssignment.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 2cd2895b83eca1ab8ce99c026ef8c02ce8e2ccde
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43399960"
---
# <a name="update-devicecompliancepolicyassignment"></a><span data-ttu-id="42638-103">Atualizar deviceCompliancePolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="42638-103">Update deviceCompliancePolicyAssignment</span></span>

<span data-ttu-id="42638-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="42638-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="42638-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="42638-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="42638-106">Atualizar as propriedades de um objeto [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md).</span><span class="sxs-lookup"><span data-stu-id="42638-106">Update the properties of a [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="42638-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="42638-107">Prerequisites</span></span>
<span data-ttu-id="42638-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="42638-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="42638-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="42638-110">Permission type</span></span>|<span data-ttu-id="42638-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="42638-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="42638-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="42638-112">Delegated (work or school account)</span></span>|<span data-ttu-id="42638-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="42638-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="42638-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="42638-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="42638-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="42638-115">Not supported.</span></span>|
|<span data-ttu-id="42638-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="42638-116">Application</span></span>|<span data-ttu-id="42638-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="42638-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="42638-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="42638-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/assignments/{deviceCompliancePolicyAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="42638-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="42638-119">Request headers</span></span>
|<span data-ttu-id="42638-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="42638-120">Header</span></span>|<span data-ttu-id="42638-121">Valor</span><span class="sxs-lookup"><span data-stu-id="42638-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="42638-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="42638-122">Authorization</span></span>|<span data-ttu-id="42638-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="42638-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="42638-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="42638-124">Accept</span></span>|<span data-ttu-id="42638-125">application/json</span><span class="sxs-lookup"><span data-stu-id="42638-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="42638-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="42638-126">Request body</span></span>
<span data-ttu-id="42638-127">No corpo da solicitação, forneça uma representação JSON do objeto [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md).</span><span class="sxs-lookup"><span data-stu-id="42638-127">In the request body, supply a JSON representation for the [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) object.</span></span>

<span data-ttu-id="42638-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md).</span><span class="sxs-lookup"><span data-stu-id="42638-128">The following table shows the properties that are required when you create the [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md).</span></span>

|<span data-ttu-id="42638-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="42638-129">Property</span></span>|<span data-ttu-id="42638-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="42638-130">Type</span></span>|<span data-ttu-id="42638-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="42638-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="42638-132">id</span><span class="sxs-lookup"><span data-stu-id="42638-132">id</span></span>|<span data-ttu-id="42638-133">String</span><span class="sxs-lookup"><span data-stu-id="42638-133">String</span></span>|<span data-ttu-id="42638-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="42638-134">Key of the entity.</span></span>|
|<span data-ttu-id="42638-135">destino</span><span class="sxs-lookup"><span data-stu-id="42638-135">target</span></span>|[<span data-ttu-id="42638-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="42638-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="42638-137">Destino da atribuição de políticas de conformidade.</span><span class="sxs-lookup"><span data-stu-id="42638-137">Target for the compliance policy assignment.</span></span>|



## <a name="response"></a><span data-ttu-id="42638-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="42638-138">Response</span></span>
<span data-ttu-id="42638-139">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="42638-139">If successful, this method returns a `200 OK` response code and an updated [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="42638-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="42638-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="42638-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="42638-141">Request</span></span>
<span data-ttu-id="42638-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="42638-142">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/assignments/{deviceCompliancePolicyAssignmentId}
Content-type: application/json
Content-length: 172

{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicyAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="42638-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="42638-143">Response</span></span>
<span data-ttu-id="42638-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="42638-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 221

{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicyAssignment",
  "id": "92dc3fef-3fef-92dc-ef3f-dc92ef3fdc92",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```






