---
title: Atualizar deviceCompliancePolicyAssignment
description: Atualizar as propriedades de um objeto deviceCompliancePolicyAssignment.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 19004fb0d283d27e48c9cb9f3de438c7444fc6a8
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32470486"
---
# <a name="update-devicecompliancepolicyassignment"></a><span data-ttu-id="02a51-103">Atualizar deviceCompliancePolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="02a51-103">Update deviceCompliancePolicyAssignment</span></span>

> <span data-ttu-id="02a51-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="02a51-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="02a51-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="02a51-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="02a51-106">Atualizar as propriedades de um objeto [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md).</span><span class="sxs-lookup"><span data-stu-id="02a51-106">Update the properties of a [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="02a51-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="02a51-107">Prerequisites</span></span>
<span data-ttu-id="02a51-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="02a51-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="02a51-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="02a51-110">Permission type</span></span>|<span data-ttu-id="02a51-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="02a51-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="02a51-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="02a51-112">Delegated (work or school account)</span></span>|<span data-ttu-id="02a51-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="02a51-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="02a51-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="02a51-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="02a51-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="02a51-115">Not supported.</span></span>|
|<span data-ttu-id="02a51-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="02a51-116">Application</span></span>|<span data-ttu-id="02a51-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="02a51-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="02a51-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="02a51-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/assignments/{deviceCompliancePolicyAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="02a51-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="02a51-119">Request headers</span></span>
|<span data-ttu-id="02a51-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="02a51-120">Header</span></span>|<span data-ttu-id="02a51-121">Valor</span><span class="sxs-lookup"><span data-stu-id="02a51-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="02a51-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="02a51-122">Authorization</span></span>|<span data-ttu-id="02a51-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="02a51-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="02a51-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="02a51-124">Accept</span></span>|<span data-ttu-id="02a51-125">application/json</span><span class="sxs-lookup"><span data-stu-id="02a51-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="02a51-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="02a51-126">Request body</span></span>
<span data-ttu-id="02a51-127">No corpo da solicitação, forneça uma representação JSON do objeto [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md).</span><span class="sxs-lookup"><span data-stu-id="02a51-127">In the request body, supply a JSON representation for the [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) object.</span></span>

<span data-ttu-id="02a51-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md).</span><span class="sxs-lookup"><span data-stu-id="02a51-128">The following table shows the properties that are required when you create the [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md).</span></span>

|<span data-ttu-id="02a51-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="02a51-129">Property</span></span>|<span data-ttu-id="02a51-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="02a51-130">Type</span></span>|<span data-ttu-id="02a51-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="02a51-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="02a51-132">id</span><span class="sxs-lookup"><span data-stu-id="02a51-132">id</span></span>|<span data-ttu-id="02a51-133">String</span><span class="sxs-lookup"><span data-stu-id="02a51-133">String</span></span>|<span data-ttu-id="02a51-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="02a51-134">Key of the entity.</span></span>|
|<span data-ttu-id="02a51-135">destino</span><span class="sxs-lookup"><span data-stu-id="02a51-135">target</span></span>|[<span data-ttu-id="02a51-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="02a51-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="02a51-137">Destino da atribuição de políticas de conformidade.</span><span class="sxs-lookup"><span data-stu-id="02a51-137">Target for the compliance policy assignment.</span></span>|



## <a name="response"></a><span data-ttu-id="02a51-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="02a51-138">Response</span></span>
<span data-ttu-id="02a51-139">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="02a51-139">If successful, this method returns a `200 OK` response code and an updated [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="02a51-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="02a51-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="02a51-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="02a51-141">Request</span></span>
<span data-ttu-id="02a51-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="02a51-142">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/assignments/{deviceCompliancePolicyAssignmentId}
Content-type: application/json
Content-length: 172

{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicyAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="02a51-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="02a51-143">Response</span></span>
<span data-ttu-id="02a51-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="02a51-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





