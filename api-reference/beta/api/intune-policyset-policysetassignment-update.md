---
title: Atualizar policySetAssignment
description: Atualiza as propriedades de um objeto policySetAssignment.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 0f9cffe1673b56e44a36edbddd557d7c1ab53bf3
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37191727"
---
# <a name="update-policysetassignment"></a><span data-ttu-id="e888b-103">Atualizar policySetAssignment</span><span class="sxs-lookup"><span data-stu-id="e888b-103">Update policySetAssignment</span></span>

> <span data-ttu-id="e888b-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e888b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e888b-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e888b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e888b-106">Atualiza as propriedades de um objeto [policySetAssignment](../resources/intune-policyset-policysetassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="e888b-106">Update the properties of a [policySetAssignment](../resources/intune-policyset-policysetassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e888b-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e888b-107">Prerequisites</span></span>
<span data-ttu-id="e888b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e888b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e888b-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e888b-110">Permission type</span></span>|<span data-ttu-id="e888b-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e888b-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e888b-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e888b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e888b-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e888b-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e888b-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e888b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e888b-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e888b-115">Not supported.</span></span>|
|<span data-ttu-id="e888b-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e888b-116">Application</span></span>|<span data-ttu-id="e888b-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e888b-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e888b-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e888b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/policySets/{policySetId}/assignments/{policySetAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="e888b-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e888b-119">Request headers</span></span>
|<span data-ttu-id="e888b-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e888b-120">Header</span></span>|<span data-ttu-id="e888b-121">Valor</span><span class="sxs-lookup"><span data-stu-id="e888b-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e888b-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="e888b-122">Authorization</span></span>|<span data-ttu-id="e888b-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e888b-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e888b-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e888b-124">Accept</span></span>|<span data-ttu-id="e888b-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e888b-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e888b-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e888b-126">Request body</span></span>
<span data-ttu-id="e888b-127">No corpo da solicitação, forneça uma representação JSON do objeto [policySetAssignment](../resources/intune-policyset-policysetassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="e888b-127">In the request body, supply a JSON representation for the [policySetAssignment](../resources/intune-policyset-policysetassignment.md) object.</span></span>

<span data-ttu-id="e888b-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [policySetAssignment](../resources/intune-policyset-policysetassignment.md).</span><span class="sxs-lookup"><span data-stu-id="e888b-128">The following table shows the properties that are required when you create the [policySetAssignment](../resources/intune-policyset-policysetassignment.md).</span></span>

|<span data-ttu-id="e888b-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e888b-129">Property</span></span>|<span data-ttu-id="e888b-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="e888b-130">Type</span></span>|<span data-ttu-id="e888b-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="e888b-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e888b-132">id</span><span class="sxs-lookup"><span data-stu-id="e888b-132">id</span></span>|<span data-ttu-id="e888b-133">String</span><span class="sxs-lookup"><span data-stu-id="e888b-133">String</span></span>|<span data-ttu-id="e888b-134">Chave do PolicySetAssignment.</span><span class="sxs-lookup"><span data-stu-id="e888b-134">Key of the PolicySetAssignment.</span></span>|
|<span data-ttu-id="e888b-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e888b-135">lastModifiedDateTime</span></span>|<span data-ttu-id="e888b-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e888b-136">DateTimeOffset</span></span>|<span data-ttu-id="e888b-137">Hora da última modificação do PolicySetAssignment.</span><span class="sxs-lookup"><span data-stu-id="e888b-137">Last modified time of the PolicySetAssignment.</span></span>|
|<span data-ttu-id="e888b-138">destino</span><span class="sxs-lookup"><span data-stu-id="e888b-138">target</span></span>|[<span data-ttu-id="e888b-139">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="e888b-139">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="e888b-140">O grupo de destino de PolicySetAssignment</span><span class="sxs-lookup"><span data-stu-id="e888b-140">The target group of PolicySetAssignment</span></span>|



## <a name="response"></a><span data-ttu-id="e888b-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="e888b-141">Response</span></span>
<span data-ttu-id="e888b-142">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [policySetAssignment](../resources/intune-policyset-policysetassignment.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e888b-142">If successful, this method returns a `200 OK` response code and an updated [policySetAssignment](../resources/intune-policyset-policysetassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e888b-143">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e888b-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="e888b-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e888b-144">Request</span></span>
<span data-ttu-id="e888b-145">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e888b-145">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/policySets/{policySetId}/assignments/{policySetAssignmentId}
Content-type: application/json
Content-length: 159

{
  "@odata.type": "#microsoft.graph.policySetAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="e888b-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="e888b-146">Response</span></span>
<span data-ttu-id="e888b-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e888b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 272

{
  "@odata.type": "#microsoft.graph.policySetAssignment",
  "id": "0a8e7d40-7d40-0a8e-407d-8e0a407d8e0a",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```




