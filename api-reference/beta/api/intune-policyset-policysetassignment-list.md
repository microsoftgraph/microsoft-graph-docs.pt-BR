---
title: Listar policySetAssignments
description: Listar propriedades e relações dos objetos policySetAssignment.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b4e7eda14f5dadab6be9d00950dd8ce044ab9240
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50153730"
---
# <a name="list-policysetassignments"></a><span data-ttu-id="d2089-103">Listar policySetAssignments</span><span class="sxs-lookup"><span data-stu-id="d2089-103">List policySetAssignments</span></span>

<span data-ttu-id="d2089-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d2089-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d2089-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d2089-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d2089-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d2089-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d2089-107">Listar propriedades e relações dos [objetos policySetAssignment.](../resources/intune-policyset-policysetassignment.md)</span><span class="sxs-lookup"><span data-stu-id="d2089-107">List properties and relationships of the [policySetAssignment](../resources/intune-policyset-policysetassignment.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d2089-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d2089-108">Prerequisites</span></span>
<span data-ttu-id="d2089-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d2089-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d2089-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d2089-111">Permission type</span></span>|<span data-ttu-id="d2089-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d2089-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d2089-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d2089-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d2089-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="d2089-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="d2089-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d2089-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d2089-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d2089-116">Not supported.</span></span>|
|<span data-ttu-id="d2089-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d2089-117">Application</span></span>|<span data-ttu-id="d2089-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="d2089-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d2089-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d2089-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/policySets/{policySetId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="d2089-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d2089-120">Request headers</span></span>
|<span data-ttu-id="d2089-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d2089-121">Header</span></span>|<span data-ttu-id="d2089-122">Valor</span><span class="sxs-lookup"><span data-stu-id="d2089-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d2089-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="d2089-123">Authorization</span></span>|<span data-ttu-id="d2089-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d2089-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d2089-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d2089-125">Accept</span></span>|<span data-ttu-id="d2089-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d2089-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d2089-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d2089-127">Request body</span></span>
<span data-ttu-id="d2089-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d2089-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d2089-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="d2089-129">Response</span></span>
<span data-ttu-id="d2089-130">Se bem-sucedido, este método retorna um código de resposta e uma coleção de `200 OK` [objetos policySetAssignment](../resources/intune-policyset-policysetassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d2089-130">If successful, this method returns a `200 OK` response code and a collection of [policySetAssignment](../resources/intune-policyset-policysetassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d2089-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d2089-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="d2089-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d2089-132">Request</span></span>
<span data-ttu-id="d2089-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d2089-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/policySets/{policySetId}/assignments
```

### <a name="response"></a><span data-ttu-id="d2089-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="d2089-134">Response</span></span>
<span data-ttu-id="d2089-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d2089-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 560

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.policySetAssignment",
      "id": "0a8e7d40-7d40-0a8e-407d-8e0a407d8e0a",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "target": {
        "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
        "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
        "deviceAndAppManagementAssignmentFilterType": "include",
        "collectionId": "Collection Id value"
      }
    }
  ]
}
```




