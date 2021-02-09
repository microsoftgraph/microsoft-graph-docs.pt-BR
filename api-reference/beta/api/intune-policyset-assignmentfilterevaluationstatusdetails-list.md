---
title: Listar assignmentFilterEvaluationStatusDetailses
description: Listar propriedades e relações dos objetos assignmentFilterEvaluationStatusDetails.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 3d2906add66455384bed8ca910b10dc0995e67cc
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50160132"
---
# <a name="list-assignmentfilterevaluationstatusdetailses"></a><span data-ttu-id="74e86-103">Listar assignmentFilterEvaluationStatusDetailses</span><span class="sxs-lookup"><span data-stu-id="74e86-103">List assignmentFilterEvaluationStatusDetailses</span></span>

<span data-ttu-id="74e86-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="74e86-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="74e86-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="74e86-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="74e86-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="74e86-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="74e86-107">Listar propriedades e relações dos objetos [assignmentFilterEvaluationStatusDetails.](../resources/intune-policyset-assignmentfilterevaluationstatusdetails.md)</span><span class="sxs-lookup"><span data-stu-id="74e86-107">List properties and relationships of the [assignmentFilterEvaluationStatusDetails](../resources/intune-policyset-assignmentfilterevaluationstatusdetails.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="74e86-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="74e86-108">Prerequisites</span></span>
<span data-ttu-id="74e86-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="74e86-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="74e86-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="74e86-111">Permission type</span></span>|<span data-ttu-id="74e86-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="74e86-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="74e86-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="74e86-113">Delegated (work or school account)</span></span>|<span data-ttu-id="74e86-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="74e86-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="74e86-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="74e86-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="74e86-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="74e86-116">Not supported.</span></span>|
|<span data-ttu-id="74e86-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="74e86-117">Application</span></span>|<span data-ttu-id="74e86-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="74e86-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="74e86-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="74e86-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/managedDevices/{managedDeviceId}/assignmentFilterEvaluationStatusDetails
```

## <a name="request-headers"></a><span data-ttu-id="74e86-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="74e86-120">Request headers</span></span>
|<span data-ttu-id="74e86-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="74e86-121">Header</span></span>|<span data-ttu-id="74e86-122">Valor</span><span class="sxs-lookup"><span data-stu-id="74e86-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="74e86-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="74e86-123">Authorization</span></span>|<span data-ttu-id="74e86-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="74e86-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="74e86-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="74e86-125">Accept</span></span>|<span data-ttu-id="74e86-126">application/json</span><span class="sxs-lookup"><span data-stu-id="74e86-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="74e86-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="74e86-127">Request body</span></span>
<span data-ttu-id="74e86-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="74e86-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="74e86-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="74e86-129">Response</span></span>
<span data-ttu-id="74e86-130">Se tiver êxito, este método retornará um código de resposta e uma coleção de objetos `200 OK` [assignmentFilterEvaluationStatusDetails](../resources/intune-policyset-assignmentfilterevaluationstatusdetails.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="74e86-130">If successful, this method returns a `200 OK` response code and a collection of [assignmentFilterEvaluationStatusDetails](../resources/intune-policyset-assignmentfilterevaluationstatusdetails.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="74e86-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="74e86-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="74e86-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="74e86-132">Request</span></span>
<span data-ttu-id="74e86-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="74e86-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/managedDevices/{managedDeviceId}/assignmentFilterEvaluationStatusDetails
```

### <a name="response"></a><span data-ttu-id="74e86-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="74e86-134">Response</span></span>
<span data-ttu-id="74e86-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="74e86-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 211

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.assignmentFilterEvaluationStatusDetails",
      "id": "820ef068-f068-820e-68f0-0e8268f00e82",
      "payloadId": "Payload Id value"
    }
  ]
}
```




