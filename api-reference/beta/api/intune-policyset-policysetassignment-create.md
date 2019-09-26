---
title: Criar policySetAssignment
description: Criar um novo objeto policySetAssignment.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e9827b9222ba4b02457cc40486f8fad3357baca6
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37191735"
---
# <a name="create-policysetassignment"></a><span data-ttu-id="1e4a1-103">Criar policySetAssignment</span><span class="sxs-lookup"><span data-stu-id="1e4a1-103">Create policySetAssignment</span></span>

> <span data-ttu-id="1e4a1-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="1e4a1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1e4a1-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1e4a1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1e4a1-106">Criar um novo objeto [policySetAssignment](../resources/intune-policyset-policysetassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="1e4a1-106">Create a new [policySetAssignment](../resources/intune-policyset-policysetassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1e4a1-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="1e4a1-107">Prerequisites</span></span>
<span data-ttu-id="1e4a1-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1e4a1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1e4a1-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1e4a1-110">Permission type</span></span>|<span data-ttu-id="1e4a1-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="1e4a1-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1e4a1-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1e4a1-112">Delegated (work or school account)</span></span>|<span data-ttu-id="1e4a1-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1e4a1-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="1e4a1-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1e4a1-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1e4a1-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1e4a1-115">Not supported.</span></span>|
|<span data-ttu-id="1e4a1-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1e4a1-116">Application</span></span>|<span data-ttu-id="1e4a1-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1e4a1-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1e4a1-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1e4a1-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/policySets/{policySetId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="1e4a1-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1e4a1-119">Request headers</span></span>
|<span data-ttu-id="1e4a1-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1e4a1-120">Header</span></span>|<span data-ttu-id="1e4a1-121">Valor</span><span class="sxs-lookup"><span data-stu-id="1e4a1-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1e4a1-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="1e4a1-122">Authorization</span></span>|<span data-ttu-id="1e4a1-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1e4a1-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1e4a1-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="1e4a1-124">Accept</span></span>|<span data-ttu-id="1e4a1-125">application/json</span><span class="sxs-lookup"><span data-stu-id="1e4a1-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1e4a1-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1e4a1-126">Request body</span></span>
<span data-ttu-id="1e4a1-127">No corpo da solicitação, forneça uma representação JSON do objeto policySetAssignment.</span><span class="sxs-lookup"><span data-stu-id="1e4a1-127">In the request body, supply a JSON representation for the policySetAssignment object.</span></span>

<span data-ttu-id="1e4a1-128">A tabela a seguir mostra as propriedades que são necessárias ao criar policySetAssignment.</span><span class="sxs-lookup"><span data-stu-id="1e4a1-128">The following table shows the properties that are required when you create the policySetAssignment.</span></span>

|<span data-ttu-id="1e4a1-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1e4a1-129">Property</span></span>|<span data-ttu-id="1e4a1-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="1e4a1-130">Type</span></span>|<span data-ttu-id="1e4a1-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="1e4a1-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1e4a1-132">id</span><span class="sxs-lookup"><span data-stu-id="1e4a1-132">id</span></span>|<span data-ttu-id="1e4a1-133">String</span><span class="sxs-lookup"><span data-stu-id="1e4a1-133">String</span></span>|<span data-ttu-id="1e4a1-134">Chave do PolicySetAssignment.</span><span class="sxs-lookup"><span data-stu-id="1e4a1-134">Key of the PolicySetAssignment.</span></span>|
|<span data-ttu-id="1e4a1-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1e4a1-135">lastModifiedDateTime</span></span>|<span data-ttu-id="1e4a1-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1e4a1-136">DateTimeOffset</span></span>|<span data-ttu-id="1e4a1-137">Hora da última modificação do PolicySetAssignment.</span><span class="sxs-lookup"><span data-stu-id="1e4a1-137">Last modified time of the PolicySetAssignment.</span></span>|
|<span data-ttu-id="1e4a1-138">destino</span><span class="sxs-lookup"><span data-stu-id="1e4a1-138">target</span></span>|[<span data-ttu-id="1e4a1-139">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="1e4a1-139">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="1e4a1-140">O grupo de destino de PolicySetAssignment</span><span class="sxs-lookup"><span data-stu-id="1e4a1-140">The target group of PolicySetAssignment</span></span>|



## <a name="response"></a><span data-ttu-id="1e4a1-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="1e4a1-141">Response</span></span>
<span data-ttu-id="1e4a1-142">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [policySetAssignment](../resources/intune-policyset-policysetassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1e4a1-142">If successful, this method returns a `201 Created` response code and a [policySetAssignment](../resources/intune-policyset-policysetassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1e4a1-143">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1e4a1-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="1e4a1-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1e4a1-144">Request</span></span>
<span data-ttu-id="1e4a1-145">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1e4a1-145">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/policySets/{policySetId}/assignments
Content-type: application/json
Content-length: 159

{
  "@odata.type": "#microsoft.graph.policySetAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="1e4a1-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="1e4a1-146">Response</span></span>
<span data-ttu-id="1e4a1-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1e4a1-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




