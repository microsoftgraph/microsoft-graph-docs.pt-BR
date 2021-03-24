---
title: Atualizar assignmentFilterEvaluationStatusDetails
description: Atualize as propriedades de um objeto assignmentFilterEvaluationStatusDetails.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 3b80c5a40c930633e54e590a117fc7bcd9ead4e1
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51125328"
---
# <a name="update-assignmentfilterevaluationstatusdetails"></a><span data-ttu-id="ae610-103">Atualizar assignmentFilterEvaluationStatusDetails</span><span class="sxs-lookup"><span data-stu-id="ae610-103">Update assignmentFilterEvaluationStatusDetails</span></span>

<span data-ttu-id="ae610-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ae610-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ae610-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ae610-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ae610-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ae610-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ae610-107">Atualize as propriedades de um [objeto assignmentFilterEvaluationStatusDetails.](../resources/intune-policyset-assignmentfilterevaluationstatusdetails.md)</span><span class="sxs-lookup"><span data-stu-id="ae610-107">Update the properties of a [assignmentFilterEvaluationStatusDetails](../resources/intune-policyset-assignmentfilterevaluationstatusdetails.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ae610-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ae610-108">Prerequisites</span></span>
<span data-ttu-id="ae610-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ae610-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ae610-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ae610-111">Permission type</span></span>|<span data-ttu-id="ae610-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ae610-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ae610-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ae610-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ae610-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ae610-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ae610-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ae610-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ae610-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ae610-116">Not supported.</span></span>|
|<span data-ttu-id="ae610-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ae610-117">Application</span></span>|<span data-ttu-id="ae610-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ae610-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ae610-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ae610-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/managedDevices/{managedDeviceId}/assignmentFilterEvaluationStatusDetails/{assignmentFilterEvaluationStatusDetailsId}
```

## <a name="request-headers"></a><span data-ttu-id="ae610-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ae610-120">Request headers</span></span>
|<span data-ttu-id="ae610-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ae610-121">Header</span></span>|<span data-ttu-id="ae610-122">Valor</span><span class="sxs-lookup"><span data-stu-id="ae610-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ae610-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="ae610-123">Authorization</span></span>|<span data-ttu-id="ae610-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ae610-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ae610-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ae610-125">Accept</span></span>|<span data-ttu-id="ae610-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ae610-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ae610-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ae610-127">Request body</span></span>
<span data-ttu-id="ae610-128">No corpo da solicitação, fornece uma representação JSON para o [objeto assignmentFilterEvaluationStatusDetails.](../resources/intune-policyset-assignmentfilterevaluationstatusdetails.md)</span><span class="sxs-lookup"><span data-stu-id="ae610-128">In the request body, supply a JSON representation for the [assignmentFilterEvaluationStatusDetails](../resources/intune-policyset-assignmentfilterevaluationstatusdetails.md) object.</span></span>

<span data-ttu-id="ae610-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [assignmentFilterEvaluationStatusDetails](../resources/intune-policyset-assignmentfilterevaluationstatusdetails.md).</span><span class="sxs-lookup"><span data-stu-id="ae610-129">The following table shows the properties that are required when you create the [assignmentFilterEvaluationStatusDetails](../resources/intune-policyset-assignmentfilterevaluationstatusdetails.md).</span></span>

|<span data-ttu-id="ae610-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ae610-130">Property</span></span>|<span data-ttu-id="ae610-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="ae610-131">Type</span></span>|<span data-ttu-id="ae610-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="ae610-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ae610-133">id</span><span class="sxs-lookup"><span data-stu-id="ae610-133">id</span></span>|<span data-ttu-id="ae610-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ae610-134">String</span></span>|<span data-ttu-id="ae610-135">Chave da entidade AssignmentFilterEvaluationStatusDetails.</span><span class="sxs-lookup"><span data-stu-id="ae610-135">Key of the AssignmentFilterEvaluationStatusDetails entity.</span></span>|
|<span data-ttu-id="ae610-136">payloadId</span><span class="sxs-lookup"><span data-stu-id="ae610-136">payloadId</span></span>|<span data-ttu-id="ae610-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ae610-137">String</span></span>|<span data-ttu-id="ae610-138">PayloadId no qual o filtro foi aplicado.</span><span class="sxs-lookup"><span data-stu-id="ae610-138">PayloadId on which filter has been applied.</span></span>|



## <a name="response"></a><span data-ttu-id="ae610-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="ae610-139">Response</span></span>
<span data-ttu-id="ae610-140">Se tiver êxito, este método retornará um código de resposta e um objeto `200 OK` [assignmentFilterEvaluationStatusDetails](../resources/intune-policyset-assignmentfilterevaluationstatusdetails.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ae610-140">If successful, this method returns a `200 OK` response code and an updated [assignmentFilterEvaluationStatusDetails](../resources/intune-policyset-assignmentfilterevaluationstatusdetails.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ae610-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ae610-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="ae610-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ae610-142">Request</span></span>
<span data-ttu-id="ae610-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ae610-143">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/managedDevices/{managedDeviceId}/assignmentFilterEvaluationStatusDetails/{assignmentFilterEvaluationStatusDetailsId}
Content-type: application/json
Content-length: 117

{
  "@odata.type": "#microsoft.graph.assignmentFilterEvaluationStatusDetails",
  "payloadId": "Payload Id value"
}
```

### <a name="response"></a><span data-ttu-id="ae610-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="ae610-144">Response</span></span>
<span data-ttu-id="ae610-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ae610-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 166

{
  "@odata.type": "#microsoft.graph.assignmentFilterEvaluationStatusDetails",
  "id": "820ef068-f068-820e-68f0-0e8268f00e82",
  "payloadId": "Payload Id value"
}
```




