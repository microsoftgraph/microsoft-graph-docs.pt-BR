---
title: Atualizar deviceCompliancePolicyAssignment
description: Atualizar as propriedades de um objeto deviceCompliancePolicyAssignment.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9bc05524538cbb9fd1321d2fdb12da4c5a6b7412
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32459686"
---
# <a name="update-devicecompliancepolicyassignment"></a><span data-ttu-id="a9c88-103">Atualizar deviceCompliancePolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="a9c88-103">Update deviceCompliancePolicyAssignment</span></span>

> <span data-ttu-id="a9c88-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a9c88-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a9c88-105">Atualizar as propriedades de um objeto [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md).</span><span class="sxs-lookup"><span data-stu-id="a9c88-105">Update the properties of a [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a9c88-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a9c88-106">Prerequisites</span></span>
<span data-ttu-id="a9c88-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a9c88-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a9c88-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a9c88-109">Permission type</span></span>|<span data-ttu-id="a9c88-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a9c88-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a9c88-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a9c88-111">Delegated (work or school account)</span></span>|<span data-ttu-id="a9c88-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a9c88-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a9c88-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a9c88-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a9c88-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a9c88-114">Not supported.</span></span>|
|<span data-ttu-id="a9c88-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a9c88-115">Application</span></span>|<span data-ttu-id="a9c88-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a9c88-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a9c88-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a9c88-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/assignments/{deviceCompliancePolicyAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="a9c88-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a9c88-118">Request headers</span></span>
|<span data-ttu-id="a9c88-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a9c88-119">Header</span></span>|<span data-ttu-id="a9c88-120">Valor</span><span class="sxs-lookup"><span data-stu-id="a9c88-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a9c88-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="a9c88-121">Authorization</span></span>|<span data-ttu-id="a9c88-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a9c88-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a9c88-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a9c88-123">Accept</span></span>|<span data-ttu-id="a9c88-124">application/json</span><span class="sxs-lookup"><span data-stu-id="a9c88-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a9c88-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a9c88-125">Request body</span></span>
<span data-ttu-id="a9c88-126">No corpo da solicitação, forneça uma representação JSON do objeto [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md).</span><span class="sxs-lookup"><span data-stu-id="a9c88-126">In the request body, supply a JSON representation for the [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) object.</span></span>

<span data-ttu-id="a9c88-127">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md).</span><span class="sxs-lookup"><span data-stu-id="a9c88-127">The following table shows the properties that are required when you create the [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md).</span></span>

|<span data-ttu-id="a9c88-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a9c88-128">Property</span></span>|<span data-ttu-id="a9c88-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="a9c88-129">Type</span></span>|<span data-ttu-id="a9c88-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="a9c88-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a9c88-131">id</span><span class="sxs-lookup"><span data-stu-id="a9c88-131">id</span></span>|<span data-ttu-id="a9c88-132">String</span><span class="sxs-lookup"><span data-stu-id="a9c88-132">String</span></span>|<span data-ttu-id="a9c88-133">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="a9c88-133">Key of the entity.</span></span>|
|<span data-ttu-id="a9c88-134">destino</span><span class="sxs-lookup"><span data-stu-id="a9c88-134">target</span></span>|[<span data-ttu-id="a9c88-135">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="a9c88-135">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="a9c88-136">Destino da atribuição de políticas de conformidade.</span><span class="sxs-lookup"><span data-stu-id="a9c88-136">Target for the compliance policy assignment.</span></span>|



## <a name="response"></a><span data-ttu-id="a9c88-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="a9c88-137">Response</span></span>
<span data-ttu-id="a9c88-138">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a9c88-138">If successful, this method returns a `200 OK` response code and an updated [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a9c88-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a9c88-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="a9c88-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a9c88-140">Request</span></span>
<span data-ttu-id="a9c88-141">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a9c88-141">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="a9c88-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="a9c88-142">Response</span></span>
<span data-ttu-id="a9c88-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a9c88-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



