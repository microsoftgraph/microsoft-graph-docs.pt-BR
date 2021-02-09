---
title: Criar assignmentFilterEvaluationStatusDetails
description: Criar um novo objeto assignmentFilterEvaluationStatusDetails.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 5a234b511821db87d92ee91416f6094379360cc6
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50160136"
---
# <a name="create-assignmentfilterevaluationstatusdetails"></a><span data-ttu-id="ad67d-103">Criar assignmentFilterEvaluationStatusDetails</span><span class="sxs-lookup"><span data-stu-id="ad67d-103">Create assignmentFilterEvaluationStatusDetails</span></span>

<span data-ttu-id="ad67d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ad67d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ad67d-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ad67d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ad67d-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ad67d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ad67d-107">Criar um novo [objeto assignmentFilterEvaluationStatusDetails.](../resources/intune-policyset-assignmentfilterevaluationstatusdetails.md)</span><span class="sxs-lookup"><span data-stu-id="ad67d-107">Create a new [assignmentFilterEvaluationStatusDetails](../resources/intune-policyset-assignmentfilterevaluationstatusdetails.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ad67d-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ad67d-108">Prerequisites</span></span>
<span data-ttu-id="ad67d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ad67d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ad67d-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ad67d-111">Permission type</span></span>|<span data-ttu-id="ad67d-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ad67d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ad67d-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ad67d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ad67d-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ad67d-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ad67d-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ad67d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ad67d-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ad67d-116">Not supported.</span></span>|
|<span data-ttu-id="ad67d-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ad67d-117">Application</span></span>|<span data-ttu-id="ad67d-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ad67d-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ad67d-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ad67d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managedDevices/{managedDeviceId}/assignmentFilterEvaluationStatusDetails
```

## <a name="request-headers"></a><span data-ttu-id="ad67d-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ad67d-120">Request headers</span></span>
|<span data-ttu-id="ad67d-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ad67d-121">Header</span></span>|<span data-ttu-id="ad67d-122">Valor</span><span class="sxs-lookup"><span data-stu-id="ad67d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ad67d-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="ad67d-123">Authorization</span></span>|<span data-ttu-id="ad67d-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ad67d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ad67d-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ad67d-125">Accept</span></span>|<span data-ttu-id="ad67d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ad67d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ad67d-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ad67d-127">Request body</span></span>
<span data-ttu-id="ad67d-128">No corpo da solicitação, fornece uma representação JSON do objeto assignmentFilterEvaluationStatusDetails.</span><span class="sxs-lookup"><span data-stu-id="ad67d-128">In the request body, supply a JSON representation for the assignmentFilterEvaluationStatusDetails object.</span></span>

<span data-ttu-id="ad67d-129">A tabela a seguir mostra as propriedades que são necessárias ao criar assignmentFilterEvaluationStatusDetails.</span><span class="sxs-lookup"><span data-stu-id="ad67d-129">The following table shows the properties that are required when you create the assignmentFilterEvaluationStatusDetails.</span></span>

|<span data-ttu-id="ad67d-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ad67d-130">Property</span></span>|<span data-ttu-id="ad67d-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="ad67d-131">Type</span></span>|<span data-ttu-id="ad67d-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="ad67d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ad67d-133">id</span><span class="sxs-lookup"><span data-stu-id="ad67d-133">id</span></span>|<span data-ttu-id="ad67d-134">String</span><span class="sxs-lookup"><span data-stu-id="ad67d-134">String</span></span>|<span data-ttu-id="ad67d-135">Chave da entidade AssignmentFilterEvaluationStatusDetails.</span><span class="sxs-lookup"><span data-stu-id="ad67d-135">Key of the AssignmentFilterEvaluationStatusDetails entity.</span></span>|
|<span data-ttu-id="ad67d-136">payloadId</span><span class="sxs-lookup"><span data-stu-id="ad67d-136">payloadId</span></span>|<span data-ttu-id="ad67d-137">String</span><span class="sxs-lookup"><span data-stu-id="ad67d-137">String</span></span>|<span data-ttu-id="ad67d-138">PayloadId no qual o filtro foi aplicado.</span><span class="sxs-lookup"><span data-stu-id="ad67d-138">PayloadId on which filter has been applied.</span></span>|



## <a name="response"></a><span data-ttu-id="ad67d-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="ad67d-139">Response</span></span>
<span data-ttu-id="ad67d-140">Se bem-sucedido, este método retorna um código de resposta e um objeto `201 Created` [assignmentFilterEvaluationStatusDetails](../resources/intune-policyset-assignmentfilterevaluationstatusdetails.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ad67d-140">If successful, this method returns a `201 Created` response code and a [assignmentFilterEvaluationStatusDetails](../resources/intune-policyset-assignmentfilterevaluationstatusdetails.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ad67d-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ad67d-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="ad67d-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ad67d-142">Request</span></span>
<span data-ttu-id="ad67d-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ad67d-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/managedDevices/{managedDeviceId}/assignmentFilterEvaluationStatusDetails
Content-type: application/json
Content-length: 117

{
  "@odata.type": "#microsoft.graph.assignmentFilterEvaluationStatusDetails",
  "payloadId": "Payload Id value"
}
```

### <a name="response"></a><span data-ttu-id="ad67d-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="ad67d-144">Response</span></span>
<span data-ttu-id="ad67d-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ad67d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 166

{
  "@odata.type": "#microsoft.graph.assignmentFilterEvaluationStatusDetails",
  "id": "820ef068-f068-820e-68f0-0e8268f00e82",
  "payloadId": "Payload Id value"
}
```




