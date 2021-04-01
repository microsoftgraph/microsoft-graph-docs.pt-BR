---
title: Obter permissão
description: Recupere as propriedades e as relações de um objeto de permissão em um site.
author: BarrySh
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 65284bfb79121c49ed9323eef005f0276e8d0d20
ms.sourcegitcommit: 17f1c9cff2e59049b894db32435af02e4ae32a70
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/31/2021
ms.locfileid: "51473714"
---
# <a name="get-permission"></a><span data-ttu-id="6f7a5-103">Obter permissão</span><span class="sxs-lookup"><span data-stu-id="6f7a5-103">Get permission</span></span>
<span data-ttu-id="6f7a5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6f7a5-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="6f7a5-105">Recupere as propriedades e as relações de um [objeto de](../resources/permission.md) permissão em um site.</span><span class="sxs-lookup"><span data-stu-id="6f7a5-105">Retrieve the properties and relationships of a [permission](../resources/permission.md) object on a site.</span></span>

## <a name="permissions"></a><span data-ttu-id="6f7a5-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="6f7a5-106">Permissions</span></span>
<span data-ttu-id="6f7a5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6f7a5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6f7a5-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6f7a5-109">Permission type</span></span>                        | <span data-ttu-id="6f7a5-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6f7a5-110">Permissions (from least to most privileged)</span></span>
|:--------------------------------------|:-------------------------------------
|<span data-ttu-id="6f7a5-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6f7a5-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="6f7a5-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6f7a5-112">Not supported.</span></span>
|<span data-ttu-id="6f7a5-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6f7a5-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6f7a5-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6f7a5-114">Not supported.</span></span>
|<span data-ttu-id="6f7a5-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6f7a5-115">Application</span></span>                            | <span data-ttu-id="6f7a5-116">Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="6f7a5-116">Sites.FullControl.All</span></span>

## <a name="http-request"></a><span data-ttu-id="6f7a5-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6f7a5-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /sites/{sitesId}/permissions/{permissionId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6f7a5-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="6f7a5-118">Optional query parameters</span></span>
<span data-ttu-id="6f7a5-119">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="6f7a5-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="6f7a5-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="6f7a5-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="6f7a5-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6f7a5-121">Request headers</span></span>
|<span data-ttu-id="6f7a5-122">Nome</span><span class="sxs-lookup"><span data-stu-id="6f7a5-122">Name</span></span>|<span data-ttu-id="6f7a5-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="6f7a5-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="6f7a5-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="6f7a5-124">Authorization</span></span>|<span data-ttu-id="6f7a5-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6f7a5-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="6f7a5-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6f7a5-127">Request body</span></span>
<span data-ttu-id="6f7a5-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="6f7a5-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6f7a5-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="6f7a5-129">Response</span></span>

<span data-ttu-id="6f7a5-130">Se tiver êxito, este método retornará `200 OK` um código de resposta e o objeto [permission](../resources/permission.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6f7a5-130">If successful, this method returns a `200 OK` response code and the [permission](../resources/permission.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6f7a5-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="6f7a5-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="6f7a5-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6f7a5-132">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="6f7a5-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="6f7a5-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_permission"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/sites/{sitesId}/permissions/{permissionId}
```
# <a name="c"></a>[<span data-ttu-id="6f7a5-134">C#</span><span class="sxs-lookup"><span data-stu-id="6f7a5-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-permission-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6f7a5-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6f7a5-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-permission-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6f7a5-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6f7a5-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-permission-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6f7a5-137">Java</span><span class="sxs-lookup"><span data-stu-id="6f7a5-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-permission-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="6f7a5-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="6f7a5-138">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.permission"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "id": "1",
  "roles": ["read"],
  "grantedToIdentities": [{
    "application": {
      "id": "89ea5c94-7736-4e25-95ad-3fa95f62b66e",
      "displayName": "Contoso Time Manager App"
    }
  }]
}
```

<!-- {
  "type": "#page.annotation",
  "section": "documentation",
  "tocPath": "Sites/Permissions/Get site permission",
} -->
