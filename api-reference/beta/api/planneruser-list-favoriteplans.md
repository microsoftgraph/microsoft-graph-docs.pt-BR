---
title: Listar favoritePlans
description: Recupere uma lista de plannerPlans marcados como favoritos por um usuário. Você pode marcar um plano como favorito, atualizando o recurso plannerUser.
author: TarkanSevilmis
localization_priority: Normal
ms.prod: planner
doc_type: apiPageType
ms.openlocfilehash: 16e9a023c53776204b719fef8b681425ccde1de2
ms.sourcegitcommit: a9f0fde9924ad184d315bb2de43c2610002409f3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/30/2020
ms.locfileid: "48314563"
---
# <a name="list-favoriteplans"></a><span data-ttu-id="91b7b-104">Listar favoritePlans</span><span class="sxs-lookup"><span data-stu-id="91b7b-104">List favoritePlans</span></span>

<span data-ttu-id="91b7b-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="91b7b-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="91b7b-106">Recupere uma lista de [plannerPlans](../resources/plannerplan.md) marcados como favoritos por um usuário.</span><span class="sxs-lookup"><span data-stu-id="91b7b-106">Retrieve a list of [plannerPlans](../resources/plannerplan.md) that are marked as favorite by a user.</span></span> <span data-ttu-id="91b7b-107">Você pode marcar um plano como favorito, [atualizando o recurso plannerUser](planneruser-update.md).</span><span class="sxs-lookup"><span data-stu-id="91b7b-107">You can mark a plan as favorite by [updating the plannerUser resource](planneruser-update.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="91b7b-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="91b7b-108">Permissions</span></span>
<span data-ttu-id="91b7b-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="91b7b-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="91b7b-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="91b7b-111">Permission type</span></span>      | <span data-ttu-id="91b7b-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="91b7b-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="91b7b-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="91b7b-113">Delegated (work or school account)</span></span> | <span data-ttu-id="91b7b-114">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="91b7b-114">Group.Read.All</span></span>    |
|<span data-ttu-id="91b7b-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="91b7b-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="91b7b-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="91b7b-116">Not supported.</span></span>    |
|<span data-ttu-id="91b7b-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="91b7b-117">Application</span></span> | <span data-ttu-id="91b7b-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="91b7b-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="91b7b-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="91b7b-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/planner/favoritePlans
GET /users/{id}/planner/favoritePlans
```
## <a name="optional-query-parameters"></a><span data-ttu-id="91b7b-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="91b7b-120">Optional query parameters</span></span>
<span data-ttu-id="91b7b-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="91b7b-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="91b7b-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="91b7b-122">Request headers</span></span>
| <span data-ttu-id="91b7b-123">Nome</span><span class="sxs-lookup"><span data-stu-id="91b7b-123">Name</span></span>      |<span data-ttu-id="91b7b-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="91b7b-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="91b7b-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="91b7b-125">Authorization</span></span>  | <span data-ttu-id="91b7b-126">Portador {código}.</span><span class="sxs-lookup"><span data-stu-id="91b7b-126">Bearer {code}.</span></span> <span data-ttu-id="91b7b-127">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="91b7b-127">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="91b7b-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="91b7b-128">Request body</span></span>
<span data-ttu-id="91b7b-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="91b7b-129">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="91b7b-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="91b7b-130">Response</span></span>
<span data-ttu-id="91b7b-131">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [plannerPlan](../resources/plannerplan.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="91b7b-131">If successful, this method returns a `200 OK` response code and a collection of [plannerPlan](../resources/plannerplan.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="91b7b-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="91b7b-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="91b7b-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="91b7b-133">Request</span></span>
<span data-ttu-id="91b7b-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="91b7b-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="91b7b-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="91b7b-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_favoriteplans"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/planner/favoritePlans
```
# <a name="c"></a>[<span data-ttu-id="91b7b-136">C#</span><span class="sxs-lookup"><span data-stu-id="91b7b-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-favoriteplans-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="91b7b-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="91b7b-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-favoriteplans-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="91b7b-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="91b7b-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-favoriteplans-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="91b7b-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="91b7b-139">Response</span></span>
<span data-ttu-id="91b7b-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="91b7b-140">The following is an example of the response.</span></span> 

><span data-ttu-id="91b7b-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="91b7b-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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