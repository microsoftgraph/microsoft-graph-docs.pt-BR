---
title: Criar deviceCompliancePolicyAssignment
description: Criar um novo objeto deviceCompliancePolicyAssignment.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 0051d67f7f33d2e48bb5d423950e9a4470439a4d
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37168562"
---
# <a name="create-devicecompliancepolicyassignment"></a><span data-ttu-id="a1646-103">Criar deviceCompliancePolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="a1646-103">Create deviceCompliancePolicyAssignment</span></span>

> <span data-ttu-id="a1646-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a1646-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a1646-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a1646-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a1646-106">Criar um novo objeto [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md).</span><span class="sxs-lookup"><span data-stu-id="a1646-106">Create a new [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a1646-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a1646-107">Prerequisites</span></span>
<span data-ttu-id="a1646-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a1646-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a1646-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a1646-110">Permission type</span></span>|<span data-ttu-id="a1646-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a1646-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a1646-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a1646-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a1646-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a1646-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a1646-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a1646-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a1646-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a1646-115">Not supported.</span></span>|
|<span data-ttu-id="a1646-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a1646-116">Application</span></span>|<span data-ttu-id="a1646-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a1646-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a1646-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a1646-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="a1646-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a1646-119">Request headers</span></span>
|<span data-ttu-id="a1646-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a1646-120">Header</span></span>|<span data-ttu-id="a1646-121">Valor</span><span class="sxs-lookup"><span data-stu-id="a1646-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a1646-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="a1646-122">Authorization</span></span>|<span data-ttu-id="a1646-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a1646-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a1646-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a1646-124">Accept</span></span>|<span data-ttu-id="a1646-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a1646-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a1646-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a1646-126">Request body</span></span>
<span data-ttu-id="a1646-127">No corpo da solicitação, forneça uma representação JSON do objeto deviceCompliancePolicyAssignment.</span><span class="sxs-lookup"><span data-stu-id="a1646-127">In the request body, supply a JSON representation for the deviceCompliancePolicyAssignment object.</span></span>

<span data-ttu-id="a1646-128">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceCompliancePolicyAssignment.</span><span class="sxs-lookup"><span data-stu-id="a1646-128">The following table shows the properties that are required when you create the deviceCompliancePolicyAssignment.</span></span>

|<span data-ttu-id="a1646-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a1646-129">Property</span></span>|<span data-ttu-id="a1646-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="a1646-130">Type</span></span>|<span data-ttu-id="a1646-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="a1646-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a1646-132">id</span><span class="sxs-lookup"><span data-stu-id="a1646-132">id</span></span>|<span data-ttu-id="a1646-133">String</span><span class="sxs-lookup"><span data-stu-id="a1646-133">String</span></span>|<span data-ttu-id="a1646-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="a1646-134">Key of the entity.</span></span>|
|<span data-ttu-id="a1646-135">destino</span><span class="sxs-lookup"><span data-stu-id="a1646-135">target</span></span>|[<span data-ttu-id="a1646-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="a1646-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="a1646-137">Destino da atribuição de políticas de conformidade.</span><span class="sxs-lookup"><span data-stu-id="a1646-137">Target for the compliance policy assignment.</span></span>|



## <a name="response"></a><span data-ttu-id="a1646-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="a1646-138">Response</span></span>
<span data-ttu-id="a1646-139">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a1646-139">If successful, this method returns a `201 Created` response code and a [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a1646-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a1646-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="a1646-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a1646-141">Request</span></span>
<span data-ttu-id="a1646-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a1646-142">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/assignments
Content-type: application/json
Content-length: 172

{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicyAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="a1646-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="a1646-143">Response</span></span>
<span data-ttu-id="a1646-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a1646-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




