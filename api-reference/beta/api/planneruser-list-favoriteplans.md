---
title: Listar favoritePlans
description: Recupere uma lista de plannerPlans marcados como favoritos por um usuário. Você pode marcar um plano como favorito, atualizando o recurso plannerUser.
author: TarkanSevilmis
localization_priority: Normal
ms.prod: planner
ms.openlocfilehash: 56773902d911b9baed23a73eb536b99315cca02e
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35455109"
---
# <a name="list-favoriteplans"></a><span data-ttu-id="fa60e-104">Listar favoritePlans</span><span class="sxs-lookup"><span data-stu-id="fa60e-104">List favoritePlans</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fa60e-105">Recupere uma lista de [plannerPlans](../resources/plannerplan.md) marcados como favoritos por um usuário.</span><span class="sxs-lookup"><span data-stu-id="fa60e-105">Retrieve a list of [plannerPlans](../resources/plannerplan.md) that are marked as favorite by a user.</span></span> <span data-ttu-id="fa60e-106">Você pode marcar um plano como favorito, [atualizando o recurso plannerUser](planneruser-update.md).</span><span class="sxs-lookup"><span data-stu-id="fa60e-106">You can mark a plan as favorite by [updating the plannerUser resource](planneruser-update.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="fa60e-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="fa60e-107">Permissions</span></span>
<span data-ttu-id="fa60e-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fa60e-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fa60e-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fa60e-110">Permission type</span></span>      | <span data-ttu-id="fa60e-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="fa60e-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fa60e-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fa60e-112">Delegated (work or school account)</span></span> | <span data-ttu-id="fa60e-113">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="fa60e-113">Group.Read.All</span></span>    |
|<span data-ttu-id="fa60e-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fa60e-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fa60e-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fa60e-115">Not supported.</span></span>    |
|<span data-ttu-id="fa60e-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fa60e-116">Application</span></span> | <span data-ttu-id="fa60e-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fa60e-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="fa60e-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fa60e-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/planner/favoritePlans
GET /users/<id>/planner/favoritePlans
```
## <a name="optional-query-parameters"></a><span data-ttu-id="fa60e-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="fa60e-119">Optional query parameters</span></span>
<span data-ttu-id="fa60e-120">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="fa60e-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="fa60e-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fa60e-121">Request headers</span></span>
| <span data-ttu-id="fa60e-122">Nome</span><span class="sxs-lookup"><span data-stu-id="fa60e-122">Name</span></span>      |<span data-ttu-id="fa60e-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="fa60e-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="fa60e-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="fa60e-124">Authorization</span></span>  | <span data-ttu-id="fa60e-125">Portador {código}.</span><span class="sxs-lookup"><span data-stu-id="fa60e-125">Bearer {code}.</span></span> <span data-ttu-id="fa60e-126">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fa60e-126">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="fa60e-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fa60e-127">Request body</span></span>
<span data-ttu-id="fa60e-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="fa60e-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="fa60e-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="fa60e-129">Response</span></span>
<span data-ttu-id="fa60e-130">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [plannerPlan](../resources/plannerplan.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fa60e-130">If successful, this method returns a `200 OK` response code and a collection of [plannerPlan](../resources/plannerplan.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="fa60e-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fa60e-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="fa60e-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fa60e-132">Request</span></span>
<span data-ttu-id="fa60e-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="fa60e-133">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="fa60e-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="fa60e-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_favoriteplans"
}-->
```http
GET https://graph.microsoft.com/beta/me/planner/favoritePlans
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="fa60e-135">C#</span><span class="sxs-lookup"><span data-stu-id="fa60e-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-favoriteplans-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="fa60e-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="fa60e-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-favoriteplans-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="fa60e-137">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="fa60e-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-favoriteplans-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="fa60e-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="fa60e-138">Response</span></span>
<span data-ttu-id="fa60e-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="fa60e-139">The following is an example of the response.</span></span> 

><span data-ttu-id="fa60e-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fa60e-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "description": "List favoritePlans",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
