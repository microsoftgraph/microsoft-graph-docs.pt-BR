---
title: Criar deviceCompliancePolicyAssignment
description: Criar um novo objeto deviceCompliancePolicyAssignment.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 59357e9270e72ef7a77fac8dbe2e0bf3330c640c
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50155171"
---
# <a name="create-devicecompliancepolicyassignment"></a><span data-ttu-id="6b391-103">Criar deviceCompliancePolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="6b391-103">Create deviceCompliancePolicyAssignment</span></span>

<span data-ttu-id="6b391-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6b391-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6b391-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="6b391-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6b391-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6b391-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6b391-107">Criar um novo objeto [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md).</span><span class="sxs-lookup"><span data-stu-id="6b391-107">Create a new [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6b391-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="6b391-108">Prerequisites</span></span>
<span data-ttu-id="6b391-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6b391-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6b391-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6b391-111">Permission type</span></span>|<span data-ttu-id="6b391-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="6b391-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6b391-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6b391-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6b391-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6b391-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6b391-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6b391-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6b391-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6b391-116">Not supported.</span></span>|
|<span data-ttu-id="6b391-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6b391-117">Application</span></span>|<span data-ttu-id="6b391-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6b391-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6b391-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6b391-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="6b391-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6b391-120">Request headers</span></span>
|<span data-ttu-id="6b391-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6b391-121">Header</span></span>|<span data-ttu-id="6b391-122">Valor</span><span class="sxs-lookup"><span data-stu-id="6b391-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6b391-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="6b391-123">Authorization</span></span>|<span data-ttu-id="6b391-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6b391-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6b391-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="6b391-125">Accept</span></span>|<span data-ttu-id="6b391-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6b391-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6b391-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6b391-127">Request body</span></span>
<span data-ttu-id="6b391-128">No corpo da solicitação, forneça uma representação JSON do objeto deviceCompliancePolicyAssignment.</span><span class="sxs-lookup"><span data-stu-id="6b391-128">In the request body, supply a JSON representation for the deviceCompliancePolicyAssignment object.</span></span>

<span data-ttu-id="6b391-129">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceCompliancePolicyAssignment.</span><span class="sxs-lookup"><span data-stu-id="6b391-129">The following table shows the properties that are required when you create the deviceCompliancePolicyAssignment.</span></span>

|<span data-ttu-id="6b391-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6b391-130">Property</span></span>|<span data-ttu-id="6b391-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="6b391-131">Type</span></span>|<span data-ttu-id="6b391-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="6b391-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6b391-133">id</span><span class="sxs-lookup"><span data-stu-id="6b391-133">id</span></span>|<span data-ttu-id="6b391-134">String</span><span class="sxs-lookup"><span data-stu-id="6b391-134">String</span></span>|<span data-ttu-id="6b391-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="6b391-135">Key of the entity.</span></span>|
|<span data-ttu-id="6b391-136">destino</span><span class="sxs-lookup"><span data-stu-id="6b391-136">target</span></span>|[<span data-ttu-id="6b391-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="6b391-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="6b391-138">Destino da atribuição de políticas de conformidade.</span><span class="sxs-lookup"><span data-stu-id="6b391-138">Target for the compliance policy assignment.</span></span>|
|<span data-ttu-id="6b391-139">source</span><span class="sxs-lookup"><span data-stu-id="6b391-139">source</span></span>|[<span data-ttu-id="6b391-140">deviceAndAppManagementAssignmentSource</span><span class="sxs-lookup"><span data-stu-id="6b391-140">deviceAndAppManagementAssignmentSource</span></span>](../resources/intune-shared-deviceandappmanagementassignmentsource.md)|<span data-ttu-id="6b391-141">A fonte de atribuição para a política de conformidade do dispositivo, direta ou direta/policySet.</span><span class="sxs-lookup"><span data-stu-id="6b391-141">The assignment source for the device compliance policy, direct or parcel/policySet.</span></span> <span data-ttu-id="6b391-142">Os valores possíveis são: `direct` e `policySets`.</span><span class="sxs-lookup"><span data-stu-id="6b391-142">Possible values are: `direct`, `policySets`.</span></span>|
|<span data-ttu-id="6b391-143">sourceId</span><span class="sxs-lookup"><span data-stu-id="6b391-143">sourceId</span></span>|<span data-ttu-id="6b391-144">String</span><span class="sxs-lookup"><span data-stu-id="6b391-144">String</span></span>|<span data-ttu-id="6b391-145">O identificador da origem da atribuição.</span><span class="sxs-lookup"><span data-stu-id="6b391-145">The identifier of the source of the assignment.</span></span>|



## <a name="response"></a><span data-ttu-id="6b391-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="6b391-146">Response</span></span>
<span data-ttu-id="6b391-147">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6b391-147">If successful, this method returns a `201 Created` response code and a [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6b391-148">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6b391-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="6b391-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6b391-149">Request</span></span>
<span data-ttu-id="6b391-150">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6b391-150">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/assignments
Content-type: application/json
Content-length: 452

{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicyAssignment",
  "target": {
    "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
    "deviceAndAppManagementAssignmentFilterType": "include",
    "collectionId": "Collection Id value"
  },
  "source": "policySets",
  "sourceId": "Source Id value"
}
```

### <a name="response"></a><span data-ttu-id="6b391-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="6b391-151">Response</span></span>
<span data-ttu-id="6b391-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6b391-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 501

{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicyAssignment",
  "id": "92dc3fef-3fef-92dc-ef3f-dc92ef3fdc92",
  "target": {
    "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
    "deviceAndAppManagementAssignmentFilterType": "include",
    "collectionId": "Collection Id value"
  },
  "source": "policySets",
  "sourceId": "Source Id value"
}
```




