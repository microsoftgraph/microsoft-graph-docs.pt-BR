---
title: Atualizar policySetAssignment
description: Atualiza as propriedades de um objeto policySetAssignment.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d1b8681e5d5ea665adf50e86c36317a47c617b1d
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43383638"
---
# <a name="update-policysetassignment"></a><span data-ttu-id="97000-103">Atualizar policySetAssignment</span><span class="sxs-lookup"><span data-stu-id="97000-103">Update policySetAssignment</span></span>

<span data-ttu-id="97000-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="97000-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="97000-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="97000-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="97000-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="97000-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="97000-107">Atualiza as propriedades de um objeto [policySetAssignment](../resources/intune-policyset-policysetassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="97000-107">Update the properties of a [policySetAssignment](../resources/intune-policyset-policysetassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="97000-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="97000-108">Prerequisites</span></span>
<span data-ttu-id="97000-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="97000-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="97000-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="97000-111">Permission type</span></span>|<span data-ttu-id="97000-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="97000-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="97000-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="97000-113">Delegated (work or school account)</span></span>|<span data-ttu-id="97000-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="97000-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="97000-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="97000-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="97000-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="97000-116">Not supported.</span></span>|
|<span data-ttu-id="97000-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="97000-117">Application</span></span>|<span data-ttu-id="97000-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="97000-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="97000-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="97000-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/policySets/{policySetId}/assignments/{policySetAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="97000-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="97000-120">Request headers</span></span>
|<span data-ttu-id="97000-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="97000-121">Header</span></span>|<span data-ttu-id="97000-122">Valor</span><span class="sxs-lookup"><span data-stu-id="97000-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="97000-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="97000-123">Authorization</span></span>|<span data-ttu-id="97000-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="97000-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="97000-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="97000-125">Accept</span></span>|<span data-ttu-id="97000-126">application/json</span><span class="sxs-lookup"><span data-stu-id="97000-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="97000-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="97000-127">Request body</span></span>
<span data-ttu-id="97000-128">No corpo da solicitação, forneça uma representação JSON do objeto [policySetAssignment](../resources/intune-policyset-policysetassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="97000-128">In the request body, supply a JSON representation for the [policySetAssignment](../resources/intune-policyset-policysetassignment.md) object.</span></span>

<span data-ttu-id="97000-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [policySetAssignment](../resources/intune-policyset-policysetassignment.md).</span><span class="sxs-lookup"><span data-stu-id="97000-129">The following table shows the properties that are required when you create the [policySetAssignment](../resources/intune-policyset-policysetassignment.md).</span></span>

|<span data-ttu-id="97000-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="97000-130">Property</span></span>|<span data-ttu-id="97000-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="97000-131">Type</span></span>|<span data-ttu-id="97000-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="97000-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="97000-133">id</span><span class="sxs-lookup"><span data-stu-id="97000-133">id</span></span>|<span data-ttu-id="97000-134">String</span><span class="sxs-lookup"><span data-stu-id="97000-134">String</span></span>|<span data-ttu-id="97000-135">Chave do PolicySetAssignment.</span><span class="sxs-lookup"><span data-stu-id="97000-135">Key of the PolicySetAssignment.</span></span>|
|<span data-ttu-id="97000-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="97000-136">lastModifiedDateTime</span></span>|<span data-ttu-id="97000-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="97000-137">DateTimeOffset</span></span>|<span data-ttu-id="97000-138">Hora da última modificação do PolicySetAssignment.</span><span class="sxs-lookup"><span data-stu-id="97000-138">Last modified time of the PolicySetAssignment.</span></span>|
|<span data-ttu-id="97000-139">destino</span><span class="sxs-lookup"><span data-stu-id="97000-139">target</span></span>|[<span data-ttu-id="97000-140">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="97000-140">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="97000-141">O grupo de destino de PolicySetAssignment</span><span class="sxs-lookup"><span data-stu-id="97000-141">The target group of PolicySetAssignment</span></span>|



## <a name="response"></a><span data-ttu-id="97000-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="97000-142">Response</span></span>
<span data-ttu-id="97000-143">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [policySetAssignment](../resources/intune-policyset-policysetassignment.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="97000-143">If successful, this method returns a `200 OK` response code and an updated [policySetAssignment](../resources/intune-policyset-policysetassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="97000-144">Exemplo</span><span class="sxs-lookup"><span data-stu-id="97000-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="97000-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="97000-145">Request</span></span>
<span data-ttu-id="97000-146">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="97000-146">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="97000-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="97000-147">Response</span></span>
<span data-ttu-id="97000-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="97000-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



