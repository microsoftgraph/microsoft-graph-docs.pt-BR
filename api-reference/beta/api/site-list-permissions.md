---
title: Listar permissões
description: Obter os recursos de permissão da propriedade de navegação de permissões em um site.
author: BarrySh
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: b4c950aec7b58eb6583e8b7a0a209a64f022368e
ms.sourcegitcommit: 17f1c9cff2e59049b894db32435af02e4ae32a70
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/31/2021
ms.locfileid: "51473210"
---
# <a name="list-permissions"></a><span data-ttu-id="7ddc3-103">Listar permissões</span><span class="sxs-lookup"><span data-stu-id="7ddc3-103">List permissions</span></span>
<span data-ttu-id="7ddc3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7ddc3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7ddc3-105">Obter os [recursos de](../resources/permission.md) permissão da propriedade de navegação de permissões em um site.</span><span class="sxs-lookup"><span data-stu-id="7ddc3-105">Get the [permission](../resources/permission.md) resources from the permissions navigation property on a site.</span></span>

## <a name="permissions"></a><span data-ttu-id="7ddc3-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="7ddc3-106">Permissions</span></span>
<span data-ttu-id="7ddc3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7ddc3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7ddc3-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7ddc3-109">Permission type</span></span>                        | <span data-ttu-id="7ddc3-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7ddc3-110">Permissions (from least to most privileged)</span></span>
|:--------------------------------------|:-------------------------------------
|<span data-ttu-id="7ddc3-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7ddc3-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="7ddc3-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7ddc3-112">Not supported.</span></span>
|<span data-ttu-id="7ddc3-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7ddc3-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7ddc3-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7ddc3-114">Not supported.</span></span>
|<span data-ttu-id="7ddc3-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7ddc3-115">Application</span></span>                            | <span data-ttu-id="7ddc3-116">Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="7ddc3-116">Sites.FullControl.All</span></span>

## <a name="http-request"></a><span data-ttu-id="7ddc3-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7ddc3-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /sites/{sitesId}/permissions
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7ddc3-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="7ddc3-118">Optional query parameters</span></span>
<span data-ttu-id="7ddc3-119">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="7ddc3-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="7ddc3-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="7ddc3-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="7ddc3-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7ddc3-121">Request headers</span></span>
|<span data-ttu-id="7ddc3-122">Nome</span><span class="sxs-lookup"><span data-stu-id="7ddc3-122">Name</span></span>|<span data-ttu-id="7ddc3-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="7ddc3-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="7ddc3-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="7ddc3-124">Authorization</span></span>|<span data-ttu-id="7ddc3-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7ddc3-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="7ddc3-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7ddc3-127">Request body</span></span>
<span data-ttu-id="7ddc3-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7ddc3-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7ddc3-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="7ddc3-129">Response</span></span>

<span data-ttu-id="7ddc3-130">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de objetos [de](../resources/permission.md) permissão no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7ddc3-130">If successful, this method returns a `200 OK` response code and a collection of [permission](../resources/permission.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="7ddc3-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="7ddc3-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="7ddc3-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7ddc3-132">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="7ddc3-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="7ddc3-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_permission"
}
-->
``` http
GET https://graph.microsoft.com/beta/sites/{sitesId}/permissions
```
# <a name="c"></a>[<span data-ttu-id="7ddc3-134">C#</span><span class="sxs-lookup"><span data-stu-id="7ddc3-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-permission-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7ddc3-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7ddc3-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-permission-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7ddc3-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7ddc3-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-permission-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7ddc3-137">Java</span><span class="sxs-lookup"><span data-stu-id="7ddc3-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-permission-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="7ddc3-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="7ddc3-138">Response</span></span>
<span data-ttu-id="7ddc3-139">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="7ddc3-139">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.permission)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
   "value":[
      {
         "id":"1",
         "roles":[
            "read"
         ],
         "grantedToIdentities":[
            {
               "application":{
                  "id":"89ea5c94-7736-4e25-95ad-3fa95f62b66e",
                  "displayName":"Contoso Time Manager App"
               }
            }
         ]
      },
      {
         "id":"2",
         "roles":[
            "write"
         ],
         "grantedToIdentities":[
            {
               "application":{
                  "id":"22f09bb7-dd29-403e-bec2-ab5cde52c2b3",
                  "displayName":"Fabrikam Dashboard App"
               }
            }
         ]
      }
   ]
}
```

<!-- {
  "type": "#page.annotation",
  "section": "documentation",
  "tocPath": "Sites/Permissions/List site permissions"
} -->
