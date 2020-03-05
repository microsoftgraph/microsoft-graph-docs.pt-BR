---
title: Listar recentPlans
description: Recupere uma lista de plannerPlans recentemente exibida por um usuário. Você pode atualizar os planos exibidos recentemente atualizando o recurso plannerUser.
author: TarkanSevilmis
localization_priority: Normal
ms.prod: planner
doc_type: apiPageType
ms.openlocfilehash: af0492c5f99545bbe823dafc301826d6ba9a3234
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42455561"
---
# <a name="list-recentplans"></a><span data-ttu-id="83770-104">Listar recentPlans</span><span class="sxs-lookup"><span data-stu-id="83770-104">List recentPlans</span></span>

<span data-ttu-id="83770-105">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="83770-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="83770-106">Recupere uma lista de [plannerPlans](../resources/plannerplan.md) exibidos recentemente por um usuário.</span><span class="sxs-lookup"><span data-stu-id="83770-106">Retrieve a list of [plannerPlans](../resources/plannerplan.md) recently viewed by a user.</span></span> <span data-ttu-id="83770-107">Você pode atualizar os planos exibidos recentemente [atualizando o recurso plannerUser](planneruser-update.md).</span><span class="sxs-lookup"><span data-stu-id="83770-107">You can update recently viewed plans by [updating the plannerUser resource](planneruser-update.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="83770-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="83770-108">Permissions</span></span>
<span data-ttu-id="83770-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="83770-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="83770-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="83770-111">Permission type</span></span>      | <span data-ttu-id="83770-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="83770-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="83770-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="83770-113">Delegated (work or school account)</span></span> | <span data-ttu-id="83770-114">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="83770-114">Group.Read.All</span></span>    |
|<span data-ttu-id="83770-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="83770-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="83770-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="83770-116">Not supported.</span></span>    |
|<span data-ttu-id="83770-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="83770-117">Application</span></span> | <span data-ttu-id="83770-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="83770-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="83770-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="83770-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/planner/recentPlans
GET /users/{id}/planner/recentPlans
```

## <a name="request-headers"></a><span data-ttu-id="83770-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="83770-120">Request headers</span></span>
| <span data-ttu-id="83770-121">Nome</span><span class="sxs-lookup"><span data-stu-id="83770-121">Name</span></span>      |<span data-ttu-id="83770-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="83770-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="83770-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="83770-123">Authorization</span></span>  | <span data-ttu-id="83770-124">Portador {código}.</span><span class="sxs-lookup"><span data-stu-id="83770-124">Bearer {code}.</span></span> <span data-ttu-id="83770-125">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="83770-125">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="83770-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="83770-126">Request body</span></span>
<span data-ttu-id="83770-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="83770-127">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="83770-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="83770-128">Response</span></span>
<span data-ttu-id="83770-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [plannerPlan](../resources/plannerplan.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="83770-129">If successful, this method returns a `200 OK` response code and a collection of [plannerPlan](../resources/plannerplan.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="83770-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="83770-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="83770-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="83770-131">Request</span></span>
<span data-ttu-id="83770-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="83770-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="83770-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="83770-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_recentplans"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/planner/recentPlans
```
# <a name="c"></a>[<span data-ttu-id="83770-134">C#</span><span class="sxs-lookup"><span data-stu-id="83770-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-recentplans-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="83770-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="83770-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-recentplans-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="83770-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="83770-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-recentplans-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="83770-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="83770-137">Response</span></span>
<span data-ttu-id="83770-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="83770-138">The following is an example of the response.</span></span> 

><span data-ttu-id="83770-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="83770-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerPlan",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 979

{
  "value": [
    {
      "@odata.etag": "W/\"JzEtUGxhbiAgQEBAQEBAQEBAQEBAQEBDXCc=\"",
      "createdBy": {
        "user": {
          "id": "dd8a8379-1ac1-4eee-861d-ec15f6fa3611"
        },
        "application": {
          "id": "09abbdfd-ed23-44ee-a2d9-a627aa1c90f3"
        }
      },
      "createdDateTime": "2015-10-14T00:57:28.4698344Z",
      "owner": "eacd01dd-84cc-4c12-bd8a-9a33e5aeed11",
      "title": "Budget Planning (2016)",
      "id": "uZWtCtli30CGoWLIWSat1mQAC0ai"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List recentPlans",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
