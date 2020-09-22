---
title: Atualizar policySetAssignment
description: Atualiza as propriedades de um objeto policySetAssignment.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 995334df6d502d65a2982b568bbfa6773850d076
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48032009"
---
# <a name="update-policysetassignment"></a><span data-ttu-id="aebab-103">Atualizar policySetAssignment</span><span class="sxs-lookup"><span data-stu-id="aebab-103">Update policySetAssignment</span></span>

<span data-ttu-id="aebab-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="aebab-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="aebab-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="aebab-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="aebab-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="aebab-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="aebab-107">Atualiza as propriedades de um objeto [policySetAssignment](../resources/intune-policyset-policysetassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="aebab-107">Update the properties of a [policySetAssignment](../resources/intune-policyset-policysetassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="aebab-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="aebab-108">Prerequisites</span></span>
<span data-ttu-id="aebab-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="aebab-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="aebab-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="aebab-111">Permission type</span></span>|<span data-ttu-id="aebab-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="aebab-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="aebab-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="aebab-113">Delegated (work or school account)</span></span>|<span data-ttu-id="aebab-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aebab-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="aebab-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="aebab-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="aebab-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="aebab-116">Not supported.</span></span>|
|<span data-ttu-id="aebab-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="aebab-117">Application</span></span>|<span data-ttu-id="aebab-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aebab-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="aebab-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="aebab-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/policySets/{policySetId}/assignments/{policySetAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="aebab-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="aebab-120">Request headers</span></span>
|<span data-ttu-id="aebab-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="aebab-121">Header</span></span>|<span data-ttu-id="aebab-122">Valor</span><span class="sxs-lookup"><span data-stu-id="aebab-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="aebab-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="aebab-123">Authorization</span></span>|<span data-ttu-id="aebab-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="aebab-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="aebab-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="aebab-125">Accept</span></span>|<span data-ttu-id="aebab-126">application/json</span><span class="sxs-lookup"><span data-stu-id="aebab-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="aebab-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="aebab-127">Request body</span></span>
<span data-ttu-id="aebab-128">No corpo da solicitação, forneça uma representação JSON do objeto [policySetAssignment](../resources/intune-policyset-policysetassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="aebab-128">In the request body, supply a JSON representation for the [policySetAssignment](../resources/intune-policyset-policysetassignment.md) object.</span></span>

<span data-ttu-id="aebab-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [policySetAssignment](../resources/intune-policyset-policysetassignment.md).</span><span class="sxs-lookup"><span data-stu-id="aebab-129">The following table shows the properties that are required when you create the [policySetAssignment](../resources/intune-policyset-policysetassignment.md).</span></span>

|<span data-ttu-id="aebab-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="aebab-130">Property</span></span>|<span data-ttu-id="aebab-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="aebab-131">Type</span></span>|<span data-ttu-id="aebab-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="aebab-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aebab-133">id</span><span class="sxs-lookup"><span data-stu-id="aebab-133">id</span></span>|<span data-ttu-id="aebab-134">String</span><span class="sxs-lookup"><span data-stu-id="aebab-134">String</span></span>|<span data-ttu-id="aebab-135">Chave do PolicySetAssignment.</span><span class="sxs-lookup"><span data-stu-id="aebab-135">Key of the PolicySetAssignment.</span></span>|
|<span data-ttu-id="aebab-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="aebab-136">lastModifiedDateTime</span></span>|<span data-ttu-id="aebab-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="aebab-137">DateTimeOffset</span></span>|<span data-ttu-id="aebab-138">Hora da última modificação do PolicySetAssignment.</span><span class="sxs-lookup"><span data-stu-id="aebab-138">Last modified time of the PolicySetAssignment.</span></span>|
|<span data-ttu-id="aebab-139">destino</span><span class="sxs-lookup"><span data-stu-id="aebab-139">target</span></span>|[<span data-ttu-id="aebab-140">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="aebab-140">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="aebab-141">O grupo de destino de PolicySetAssignment</span><span class="sxs-lookup"><span data-stu-id="aebab-141">The target group of PolicySetAssignment</span></span>|



## <a name="response"></a><span data-ttu-id="aebab-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="aebab-142">Response</span></span>
<span data-ttu-id="aebab-143">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [policySetAssignment](../resources/intune-policyset-policysetassignment.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="aebab-143">If successful, this method returns a `200 OK` response code and an updated [policySetAssignment](../resources/intune-policyset-policysetassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="aebab-144">Exemplo</span><span class="sxs-lookup"><span data-stu-id="aebab-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="aebab-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="aebab-145">Request</span></span>
<span data-ttu-id="aebab-146">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="aebab-146">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/policySets/{policySetId}/assignments/{policySetAssignmentId}
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

### <a name="response"></a><span data-ttu-id="aebab-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="aebab-147">Response</span></span>
<span data-ttu-id="aebab-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="aebab-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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






