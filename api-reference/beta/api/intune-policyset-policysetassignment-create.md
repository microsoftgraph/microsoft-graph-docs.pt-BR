---
title: Criar policySetAssignment
description: Criar um novo objeto policySetAssignment.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d95a41b843844edf43f430c19685a689d2d73917
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/16/2019
ms.locfileid: "37536312"
---
# <a name="create-policysetassignment"></a><span data-ttu-id="82094-103">Criar policySetAssignment</span><span class="sxs-lookup"><span data-stu-id="82094-103">Create policySetAssignment</span></span>

> <span data-ttu-id="82094-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="82094-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="82094-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="82094-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="82094-106">Criar um novo objeto [policySetAssignment](../resources/intune-policyset-policysetassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="82094-106">Create a new [policySetAssignment](../resources/intune-policyset-policysetassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="82094-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="82094-107">Prerequisites</span></span>
<span data-ttu-id="82094-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="82094-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="82094-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="82094-110">Permission type</span></span>|<span data-ttu-id="82094-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="82094-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="82094-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="82094-112">Delegated (work or school account)</span></span>|<span data-ttu-id="82094-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="82094-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="82094-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="82094-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="82094-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="82094-115">Not supported.</span></span>|
|<span data-ttu-id="82094-116">Application</span><span class="sxs-lookup"><span data-stu-id="82094-116">Application</span></span>|<span data-ttu-id="82094-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="82094-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="82094-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="82094-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/policySets/{policySetId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="82094-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="82094-119">Request headers</span></span>
|<span data-ttu-id="82094-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="82094-120">Header</span></span>|<span data-ttu-id="82094-121">Valor</span><span class="sxs-lookup"><span data-stu-id="82094-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="82094-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="82094-122">Authorization</span></span>|<span data-ttu-id="82094-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="82094-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="82094-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="82094-124">Accept</span></span>|<span data-ttu-id="82094-125">application/json</span><span class="sxs-lookup"><span data-stu-id="82094-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="82094-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="82094-126">Request body</span></span>
<span data-ttu-id="82094-127">No corpo da solicitação, forneça uma representação JSON do objeto policySetAssignment.</span><span class="sxs-lookup"><span data-stu-id="82094-127">In the request body, supply a JSON representation for the policySetAssignment object.</span></span>

<span data-ttu-id="82094-128">A tabela a seguir mostra as propriedades que são necessárias ao criar policySetAssignment.</span><span class="sxs-lookup"><span data-stu-id="82094-128">The following table shows the properties that are required when you create the policySetAssignment.</span></span>

|<span data-ttu-id="82094-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="82094-129">Property</span></span>|<span data-ttu-id="82094-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="82094-130">Type</span></span>|<span data-ttu-id="82094-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="82094-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="82094-132">id</span><span class="sxs-lookup"><span data-stu-id="82094-132">id</span></span>|<span data-ttu-id="82094-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="82094-133">String</span></span>|<span data-ttu-id="82094-134">Chave do PolicySetAssignment.</span><span class="sxs-lookup"><span data-stu-id="82094-134">Key of the PolicySetAssignment.</span></span>|
|<span data-ttu-id="82094-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="82094-135">lastModifiedDateTime</span></span>|<span data-ttu-id="82094-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="82094-136">DateTimeOffset</span></span>|<span data-ttu-id="82094-137">Hora da última modificação do PolicySetAssignment.</span><span class="sxs-lookup"><span data-stu-id="82094-137">Last modified time of the PolicySetAssignment.</span></span>|
|<span data-ttu-id="82094-138">destino</span><span class="sxs-lookup"><span data-stu-id="82094-138">target</span></span>|[<span data-ttu-id="82094-139">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="82094-139">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="82094-140">O grupo de destino de PolicySetAssignment</span><span class="sxs-lookup"><span data-stu-id="82094-140">The target group of PolicySetAssignment</span></span>|



## <a name="response"></a><span data-ttu-id="82094-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="82094-141">Response</span></span>
<span data-ttu-id="82094-142">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [policySetAssignment](../resources/intune-policyset-policysetassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="82094-142">If successful, this method returns a `201 Created` response code and a [policySetAssignment](../resources/intune-policyset-policysetassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="82094-143">Exemplo</span><span class="sxs-lookup"><span data-stu-id="82094-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="82094-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="82094-144">Request</span></span>
<span data-ttu-id="82094-145">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="82094-145">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="82094-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="82094-146">Response</span></span>
<span data-ttu-id="82094-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="82094-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






