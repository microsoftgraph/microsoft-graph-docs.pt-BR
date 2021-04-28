---
title: Listar implantações
description: Obter uma lista de objetos de implantação e suas propriedades.
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: apiPageType
ms.openlocfilehash: f0e1028be3e9f8c5c49ebae42022ae71eda0c583
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067773"
---
# <a name="list-deployments"></a><span data-ttu-id="04d0b-103">Listar implantações</span><span class="sxs-lookup"><span data-stu-id="04d0b-103">List deployments</span></span>
<span data-ttu-id="04d0b-104">Namespace: microsoft.graph.windowsUpdates</span><span class="sxs-lookup"><span data-stu-id="04d0b-104">Namespace: microsoft.graph.windowsUpdates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="04d0b-105">Obter uma lista de [objetos de implantação](../resources/windowsupdates-deployment.md) e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="04d0b-105">Get a list of [deployment](../resources/windowsupdates-deployment.md) objects and their properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="04d0b-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="04d0b-106">Permissions</span></span>
<span data-ttu-id="04d0b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="04d0b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="04d0b-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="04d0b-109">Permission type</span></span>|<span data-ttu-id="04d0b-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="04d0b-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="04d0b-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="04d0b-111">Delegated (work or school account)</span></span>|<span data-ttu-id="04d0b-112">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="04d0b-112">WindowsUpdates.ReadWrite.All</span></span>|
|<span data-ttu-id="04d0b-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="04d0b-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="04d0b-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="04d0b-114">Not supported.</span></span>|
|<span data-ttu-id="04d0b-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="04d0b-115">Application</span></span>|<span data-ttu-id="04d0b-116">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="04d0b-116">WindowsUpdates.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="04d0b-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="04d0b-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /admin/windows/updates/deployments
```

## <a name="optional-query-parameters"></a><span data-ttu-id="04d0b-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="04d0b-118">Optional query parameters</span></span>
<span data-ttu-id="04d0b-119">Este método dá suporte a alguns dos [parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta, incluindo `$count` , , , , , e `$filter` `$orderBy` `$select` `$skip` `$top` .</span><span class="sxs-lookup"><span data-stu-id="04d0b-119">This method supports some of the [OData query parameters](/graph/query-parameters) to help customize the response, including `$count`, `$filter`, `$orderBy`, `$select`, `$skip`, and `$top`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="04d0b-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="04d0b-120">Request headers</span></span>
|<span data-ttu-id="04d0b-121">Nome</span><span class="sxs-lookup"><span data-stu-id="04d0b-121">Name</span></span>|<span data-ttu-id="04d0b-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="04d0b-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="04d0b-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="04d0b-123">Authorization</span></span>|<span data-ttu-id="04d0b-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="04d0b-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="04d0b-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="04d0b-126">Request body</span></span>
<span data-ttu-id="04d0b-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="04d0b-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="04d0b-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="04d0b-128">Response</span></span>

<span data-ttu-id="04d0b-129">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de objetos de [implantação](../resources/windowsupdates-deployment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="04d0b-129">If successful, this method returns a `200 OK` response code and a collection of [deployment](../resources/windowsupdates-deployment.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="04d0b-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="04d0b-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="04d0b-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="04d0b-131">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "list_deployment"
}
-->
``` http
GET https://graph.microsoft.com/beta/admin/windows/updates/deployments
```


### <a name="response"></a><span data-ttu-id="04d0b-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="04d0b-132">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.windowsUpdates.deployment)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
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
  ]
}
```

