---
title: Criar policySetAssignment
description: Criar um novo objeto policySetAssignment.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 85a40859f986d07c36cc6e1d5950d3b1e23c00c7
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49257881"
---
# <a name="create-policysetassignment"></a><span data-ttu-id="15ad7-103">Criar policySetAssignment</span><span class="sxs-lookup"><span data-stu-id="15ad7-103">Create policySetAssignment</span></span>

<span data-ttu-id="15ad7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="15ad7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="15ad7-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="15ad7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="15ad7-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="15ad7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="15ad7-107">Criar um novo objeto [policySetAssignment](../resources/intune-policyset-policysetassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="15ad7-107">Create a new [policySetAssignment](../resources/intune-policyset-policysetassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="15ad7-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="15ad7-108">Prerequisites</span></span>
<span data-ttu-id="15ad7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="15ad7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="15ad7-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="15ad7-111">Permission type</span></span>|<span data-ttu-id="15ad7-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="15ad7-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="15ad7-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="15ad7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="15ad7-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="15ad7-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="15ad7-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="15ad7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="15ad7-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="15ad7-116">Not supported.</span></span>|
|<span data-ttu-id="15ad7-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="15ad7-117">Application</span></span>|<span data-ttu-id="15ad7-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="15ad7-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="15ad7-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="15ad7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/policySets/{policySetId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="15ad7-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="15ad7-120">Request headers</span></span>
|<span data-ttu-id="15ad7-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="15ad7-121">Header</span></span>|<span data-ttu-id="15ad7-122">Valor</span><span class="sxs-lookup"><span data-stu-id="15ad7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="15ad7-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="15ad7-123">Authorization</span></span>|<span data-ttu-id="15ad7-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="15ad7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="15ad7-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="15ad7-125">Accept</span></span>|<span data-ttu-id="15ad7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="15ad7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="15ad7-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="15ad7-127">Request body</span></span>
<span data-ttu-id="15ad7-128">No corpo da solicitação, forneça uma representação JSON do objeto policySetAssignment.</span><span class="sxs-lookup"><span data-stu-id="15ad7-128">In the request body, supply a JSON representation for the policySetAssignment object.</span></span>

<span data-ttu-id="15ad7-129">A tabela a seguir mostra as propriedades que são necessárias ao criar policySetAssignment.</span><span class="sxs-lookup"><span data-stu-id="15ad7-129">The following table shows the properties that are required when you create the policySetAssignment.</span></span>

|<span data-ttu-id="15ad7-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="15ad7-130">Property</span></span>|<span data-ttu-id="15ad7-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="15ad7-131">Type</span></span>|<span data-ttu-id="15ad7-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="15ad7-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="15ad7-133">id</span><span class="sxs-lookup"><span data-stu-id="15ad7-133">id</span></span>|<span data-ttu-id="15ad7-134">String</span><span class="sxs-lookup"><span data-stu-id="15ad7-134">String</span></span>|<span data-ttu-id="15ad7-135">Chave do PolicySetAssignment.</span><span class="sxs-lookup"><span data-stu-id="15ad7-135">Key of the PolicySetAssignment.</span></span>|
|<span data-ttu-id="15ad7-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="15ad7-136">lastModifiedDateTime</span></span>|<span data-ttu-id="15ad7-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="15ad7-137">DateTimeOffset</span></span>|<span data-ttu-id="15ad7-138">Hora da última modificação do PolicySetAssignment.</span><span class="sxs-lookup"><span data-stu-id="15ad7-138">Last modified time of the PolicySetAssignment.</span></span>|
|<span data-ttu-id="15ad7-139">destino</span><span class="sxs-lookup"><span data-stu-id="15ad7-139">target</span></span>|[<span data-ttu-id="15ad7-140">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="15ad7-140">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="15ad7-141">O grupo de destino de PolicySetAssignment</span><span class="sxs-lookup"><span data-stu-id="15ad7-141">The target group of PolicySetAssignment</span></span>|



## <a name="response"></a><span data-ttu-id="15ad7-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="15ad7-142">Response</span></span>
<span data-ttu-id="15ad7-143">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [policySetAssignment](../resources/intune-policyset-policysetassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="15ad7-143">If successful, this method returns a `201 Created` response code and a [policySetAssignment](../resources/intune-policyset-policysetassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="15ad7-144">Exemplo</span><span class="sxs-lookup"><span data-stu-id="15ad7-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="15ad7-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="15ad7-145">Request</span></span>
<span data-ttu-id="15ad7-146">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="15ad7-146">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/policySets/{policySetId}/assignments
Content-type: application/json
Content-length: 314

{
  "@odata.type": "#microsoft.graph.policySetAssignment",
  "target": {
    "@odata.type": "microsoft.graph.allDevicesAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
    "deviceAndAppManagementAssignmentFilterType": "include"
  }
}
```

### <a name="response"></a><span data-ttu-id="15ad7-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="15ad7-147">Response</span></span>
<span data-ttu-id="15ad7-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="15ad7-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 427

{
  "@odata.type": "#microsoft.graph.policySetAssignment",
  "id": "0a8e7d40-7d40-0a8e-407d-8e0a407d8e0a",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "target": {
    "@odata.type": "microsoft.graph.allDevicesAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
    "deviceAndAppManagementAssignmentFilterType": "include"
  }
}
```




