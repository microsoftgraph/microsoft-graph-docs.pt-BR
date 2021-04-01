---
title: Listar recentPlans
description: Recupere uma lista de plannerPlans recentemente exibida por um usuário. Você pode atualizar os planos exibidos recentemente atualizando o recurso plannerUser.
author: TarkanSevilmis
localization_priority: Normal
ms.prod: planner
doc_type: apiPageType
ms.openlocfilehash: abe618b63bdd15e3053c831352490255468bb0f2
ms.sourcegitcommit: 17f1c9cff2e59049b894db32435af02e4ae32a70
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/31/2021
ms.locfileid: "51473469"
---
# <a name="list-recentplans"></a><span data-ttu-id="314aa-104">Listar recentPlans</span><span class="sxs-lookup"><span data-stu-id="314aa-104">List recentPlans</span></span>

<span data-ttu-id="314aa-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="314aa-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="314aa-106">Recupere uma lista de [plannerPlans exibidos](../resources/plannerplan.md) recentemente por um usuário.</span><span class="sxs-lookup"><span data-stu-id="314aa-106">Retrieve a list of [plannerPlans](../resources/plannerplan.md) recently viewed by a user.</span></span> <span data-ttu-id="314aa-107">Você pode atualizar os planos exibidos recentemente [atualizando o recurso plannerUser](planneruser-update.md).</span><span class="sxs-lookup"><span data-stu-id="314aa-107">You can update recently viewed plans by [updating the plannerUser resource](planneruser-update.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="314aa-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="314aa-108">Permissions</span></span>
<span data-ttu-id="314aa-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="314aa-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="314aa-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="314aa-111">Permission type</span></span>      | <span data-ttu-id="314aa-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="314aa-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="314aa-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="314aa-113">Delegated (work or school account)</span></span> | <span data-ttu-id="314aa-114">Tasks.Read, Tasks.ReadWrite, Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="314aa-114">Tasks.Read, Tasks.ReadWrite, Group.Read.All</span></span>    |
|<span data-ttu-id="314aa-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="314aa-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="314aa-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="314aa-116">Not supported.</span></span>    |
|<span data-ttu-id="314aa-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="314aa-117">Application</span></span> | <span data-ttu-id="314aa-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="314aa-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="314aa-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="314aa-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/planner/recentPlans
GET /users/{id}/planner/recentPlans
```

## <a name="request-headers"></a><span data-ttu-id="314aa-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="314aa-120">Request headers</span></span>
| <span data-ttu-id="314aa-121">Nome</span><span class="sxs-lookup"><span data-stu-id="314aa-121">Name</span></span>      |<span data-ttu-id="314aa-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="314aa-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="314aa-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="314aa-123">Authorization</span></span>  | <span data-ttu-id="314aa-124">Portador {código}.</span><span class="sxs-lookup"><span data-stu-id="314aa-124">Bearer {code}.</span></span> <span data-ttu-id="314aa-125">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="314aa-125">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="314aa-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="314aa-126">Request body</span></span>
<span data-ttu-id="314aa-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="314aa-127">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="314aa-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="314aa-128">Response</span></span>
<span data-ttu-id="314aa-129">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de objetos [plannerPlan](../resources/plannerplan.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="314aa-129">If successful, this method returns a `200 OK` response code and a collection of [plannerPlan](../resources/plannerplan.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="314aa-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="314aa-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="314aa-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="314aa-131">Request</span></span>
<span data-ttu-id="314aa-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="314aa-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="314aa-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="314aa-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_recentplans"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/planner/recentPlans
```
# <a name="c"></a>[<span data-ttu-id="314aa-134">C#</span><span class="sxs-lookup"><span data-stu-id="314aa-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-recentplans-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="314aa-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="314aa-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-recentplans-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="314aa-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="314aa-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-recentplans-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="314aa-137">Java</span><span class="sxs-lookup"><span data-stu-id="314aa-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-recentplans-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="314aa-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="314aa-138">Response</span></span>
<span data-ttu-id="314aa-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="314aa-139">The following is an example of the response.</span></span> 

><span data-ttu-id="314aa-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="314aa-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


