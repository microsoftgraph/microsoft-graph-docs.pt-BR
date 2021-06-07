---
title: Atualizar deviceCompliancePolicyAssignment
description: Atualizar as propriedades de um objeto deviceCompliancePolicyAssignment.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 8b0dce7e104b3aa472471f515854745fb888c53e
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52753948"
---
# <a name="update-devicecompliancepolicyassignment"></a><span data-ttu-id="4f24b-103">Atualizar deviceCompliancePolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="4f24b-103">Update deviceCompliancePolicyAssignment</span></span>

<span data-ttu-id="4f24b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4f24b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4f24b-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="4f24b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4f24b-106">Atualizar as propriedades de um objeto [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md).</span><span class="sxs-lookup"><span data-stu-id="4f24b-106">Update the properties of a [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4f24b-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="4f24b-107">Prerequisites</span></span>
<span data-ttu-id="4f24b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4f24b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4f24b-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4f24b-110">Permission type</span></span>|<span data-ttu-id="4f24b-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4f24b-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4f24b-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4f24b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4f24b-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4f24b-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4f24b-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4f24b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4f24b-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4f24b-115">Not supported.</span></span>|
|<span data-ttu-id="4f24b-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4f24b-116">Application</span></span>|<span data-ttu-id="4f24b-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4f24b-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4f24b-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4f24b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/assignments/{deviceCompliancePolicyAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="4f24b-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4f24b-119">Request headers</span></span>
|<span data-ttu-id="4f24b-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4f24b-120">Header</span></span>|<span data-ttu-id="4f24b-121">Valor</span><span class="sxs-lookup"><span data-stu-id="4f24b-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4f24b-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="4f24b-122">Authorization</span></span>|<span data-ttu-id="4f24b-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4f24b-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4f24b-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="4f24b-124">Accept</span></span>|<span data-ttu-id="4f24b-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4f24b-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4f24b-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4f24b-126">Request body</span></span>
<span data-ttu-id="4f24b-127">No corpo da solicitação, forneça uma representação JSON do objeto [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md).</span><span class="sxs-lookup"><span data-stu-id="4f24b-127">In the request body, supply a JSON representation for the [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) object.</span></span>

<span data-ttu-id="4f24b-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md).</span><span class="sxs-lookup"><span data-stu-id="4f24b-128">The following table shows the properties that are required when you create the [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md).</span></span>

|<span data-ttu-id="4f24b-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4f24b-129">Property</span></span>|<span data-ttu-id="4f24b-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="4f24b-130">Type</span></span>|<span data-ttu-id="4f24b-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="4f24b-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4f24b-132">id</span><span class="sxs-lookup"><span data-stu-id="4f24b-132">id</span></span>|<span data-ttu-id="4f24b-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4f24b-133">String</span></span>|<span data-ttu-id="4f24b-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="4f24b-134">Key of the entity.</span></span>|
|<span data-ttu-id="4f24b-135">destino</span><span class="sxs-lookup"><span data-stu-id="4f24b-135">target</span></span>|[<span data-ttu-id="4f24b-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="4f24b-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="4f24b-137">Destino da atribuição de políticas de conformidade.</span><span class="sxs-lookup"><span data-stu-id="4f24b-137">Target for the compliance policy assignment.</span></span>|



## <a name="response"></a><span data-ttu-id="4f24b-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="4f24b-138">Response</span></span>
<span data-ttu-id="4f24b-139">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4f24b-139">If successful, this method returns a `200 OK` response code and an updated [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4f24b-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4f24b-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="4f24b-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4f24b-141">Request</span></span>
<span data-ttu-id="4f24b-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4f24b-142">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/assignments/{deviceCompliancePolicyAssignmentId}
Content-type: application/json
Content-length: 224

{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicyAssignment",
  "target": {
    "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
    "collectionId": "Collection Id value"
  }
}
```

### <a name="response"></a><span data-ttu-id="4f24b-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="4f24b-143">Response</span></span>
<span data-ttu-id="4f24b-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4f24b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 273

{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicyAssignment",
  "id": "92dc3fef-3fef-92dc-ef3f-dc92ef3fdc92",
  "target": {
    "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
    "collectionId": "Collection Id value"
  }
}
```




