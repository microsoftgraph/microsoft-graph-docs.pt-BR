---
title: Obter implantação
description: Leia as propriedades e as relações de um objeto de implantação.
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: apiPageType
ms.openlocfilehash: 43081598030efc8ac4b3e30fe35d99931dde5d8f
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067778"
---
# <a name="get-deployment"></a><span data-ttu-id="6a2d7-103">Obter implantação</span><span class="sxs-lookup"><span data-stu-id="6a2d7-103">Get deployment</span></span>
<span data-ttu-id="6a2d7-104">Namespace: microsoft.graph.windowsUpdates</span><span class="sxs-lookup"><span data-stu-id="6a2d7-104">Namespace: microsoft.graph.windowsUpdates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6a2d7-105">Leia as propriedades e as relações de um [objeto de](../resources/windowsupdates-deployment.md) implantação.</span><span class="sxs-lookup"><span data-stu-id="6a2d7-105">Read the properties and relationships of a [deployment](../resources/windowsupdates-deployment.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="6a2d7-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="6a2d7-106">Permissions</span></span>
<span data-ttu-id="6a2d7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6a2d7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6a2d7-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6a2d7-109">Permission type</span></span>|<span data-ttu-id="6a2d7-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6a2d7-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6a2d7-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6a2d7-111">Delegated (work or school account)</span></span>|<span data-ttu-id="6a2d7-112">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6a2d7-112">WindowsUpdates.ReadWrite.All</span></span>|
|<span data-ttu-id="6a2d7-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6a2d7-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6a2d7-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6a2d7-114">Not supported.</span></span>|
|<span data-ttu-id="6a2d7-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6a2d7-115">Application</span></span>|<span data-ttu-id="6a2d7-116">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6a2d7-116">WindowsUpdates.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6a2d7-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6a2d7-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /admin/windows/updates/deployments/{deploymentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6a2d7-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="6a2d7-118">Optional query parameters</span></span>
<span data-ttu-id="6a2d7-119">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="6a2d7-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="6a2d7-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="6a2d7-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="6a2d7-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6a2d7-121">Request headers</span></span>
|<span data-ttu-id="6a2d7-122">Nome</span><span class="sxs-lookup"><span data-stu-id="6a2d7-122">Name</span></span>|<span data-ttu-id="6a2d7-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="6a2d7-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="6a2d7-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="6a2d7-124">Authorization</span></span>|<span data-ttu-id="6a2d7-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6a2d7-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="6a2d7-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6a2d7-127">Request body</span></span>
<span data-ttu-id="6a2d7-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="6a2d7-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6a2d7-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="6a2d7-129">Response</span></span>

<span data-ttu-id="6a2d7-130">Se tiver êxito, este método retornará um código de resposta e um `200 OK` objeto [de](../resources/windowsupdates-deployment.md) implantação no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6a2d7-130">If successful, this method returns a `200 OK` response code and a [deployment](../resources/windowsupdates-deployment.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6a2d7-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="6a2d7-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="6a2d7-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6a2d7-132">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_deployment"
}
-->
``` http
GET https://graph.microsoft.com/beta/admin/windows/updates/deployments/b5171742-1742-b517-4217-17b5421717b5
```


### <a name="response"></a><span data-ttu-id="6a2d7-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="6a2d7-133">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.windowsUpdates.deployment"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsUpdates.deployment",
    "id": "b5171742-1742-b517-4217-17b5421717b5",
    "state": {
      "@odata.type": "microsoft.graph.windowsUpdates.deploymentState"
    },
    "content": {
      "@odata.type": "microsoft.graph.windowsUpdates.deployableContent"
    },
    "settings": {
      "@odata.type": "microsoft.graph.windowsUpdates.deploymentSettings"
    },
    "createdDateTime": "String (timestamp)",
    "lastModifiedDateTime": "String (timestamp)"
  }
}
```

