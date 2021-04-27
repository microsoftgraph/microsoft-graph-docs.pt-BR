---
title: Obter plannerTaskDetails
description: Recupere as propriedades e as relações do **objeto plannertaskdetails.**
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: apiPageType
ms.openlocfilehash: eb1318bbb28884c5d9e95b97274c4cae836ef322
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52049972"
---
# <a name="get-plannertaskdetails"></a><span data-ttu-id="47b0a-103">Obter plannerTaskDetails</span><span class="sxs-lookup"><span data-stu-id="47b0a-103">Get plannerTaskDetails</span></span>

<span data-ttu-id="47b0a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="47b0a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="47b0a-105">Recupere as propriedades e as relações do **objeto plannertaskdetails.**</span><span class="sxs-lookup"><span data-stu-id="47b0a-105">Retrieve the properties and relationships of **plannertaskdetails** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="47b0a-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="47b0a-106">Permissions</span></span>
<span data-ttu-id="47b0a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="47b0a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="47b0a-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="47b0a-109">Permission type</span></span>      | <span data-ttu-id="47b0a-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="47b0a-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="47b0a-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="47b0a-111">Delegated (work or school account)</span></span> | <span data-ttu-id="47b0a-112">Tasks.Read, Tasks.ReadWrite, Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="47b0a-112">Tasks.Read, Tasks.ReadWrite, Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="47b0a-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="47b0a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="47b0a-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="47b0a-114">Not supported.</span></span>    |
|<span data-ttu-id="47b0a-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="47b0a-115">Application</span></span> | <span data-ttu-id="47b0a-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="47b0a-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="47b0a-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="47b0a-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /planner/tasks/{id}/details
```

## <a name="request-headers"></a><span data-ttu-id="47b0a-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="47b0a-118">Request headers</span></span>
| <span data-ttu-id="47b0a-119">Nome</span><span class="sxs-lookup"><span data-stu-id="47b0a-119">Name</span></span>      |<span data-ttu-id="47b0a-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="47b0a-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="47b0a-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="47b0a-121">Authorization</span></span>  | <span data-ttu-id="47b0a-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="47b0a-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="47b0a-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="47b0a-124">Request body</span></span>
<span data-ttu-id="47b0a-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="47b0a-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="47b0a-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="47b0a-126">Response</span></span>

<span data-ttu-id="47b0a-127">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto plannerTaskDetails](../resources/plannertaskdetails.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="47b0a-127">If successful, this method returns a `200 OK` response code and [plannerTaskDetails](../resources/plannertaskdetails.md) object in the response body.</span></span>

<span data-ttu-id="47b0a-128">Este método pode retornar qualquer um dos [códigos de status de HTTP](/graph/errors).</span><span class="sxs-lookup"><span data-stu-id="47b0a-128">This method can return any of the [HTTP status codes](/graph/errors).</span></span> <span data-ttu-id="47b0a-129">Os erros mais comuns que os aplicativos devem tratar para esse método são as respostas 403 e 404.</span><span class="sxs-lookup"><span data-stu-id="47b0a-129">The most common errors that apps should handle for this method are the 403 and 404 responses.</span></span> <span data-ttu-id="47b0a-130">Saiba mais sobre esses erros em [Condições de erro comuns do Planner](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="47b0a-130">For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="47b0a-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="47b0a-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="47b0a-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="47b0a-132">Request</span></span>
<span data-ttu-id="47b0a-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="47b0a-133">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="47b0a-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="47b0a-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_plannertaskdetails"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/planner/tasks/gcrYAaAkgU2EQUvpkNNXLGQAGTtu/details
```
# <a name="c"></a>[<span data-ttu-id="47b0a-135">C#</span><span class="sxs-lookup"><span data-stu-id="47b0a-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-plannertaskdetails-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="47b0a-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="47b0a-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-plannertaskdetails-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="47b0a-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="47b0a-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-plannertaskdetails-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="47b0a-138">Java</span><span class="sxs-lookup"><span data-stu-id="47b0a-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-plannertaskdetails-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="47b0a-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="47b0a-139">Response</span></span>
<span data-ttu-id="47b0a-140">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="47b0a-140">Here is an example of the response.</span></span> <span data-ttu-id="47b0a-141">Observação: o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="47b0a-141">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerTaskDetails"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1036

{
  "description": "Task details properties:\nchecklist:Sub items\nreferences:Related links",
  "previewType": "automatic",
  "references": {
    "https%3A//developer%2Emicrosoft%2Ecom/en-us/graph/graph-explorer": {
      "@odata.type": "#microsoft.graph.plannerExternalReference",
      "alias": "Graph Explorer",
      "type": "Other",
      "previewPriority": "0009005706180391122",
      "lastModifiedBy": {
        "user": {
          "id": "fbab97d0-4932-4511-b675-204639209557"
        }
      },
      "lastModifiedDateTime": "2017-04-24T22:52:29.814Z"
    }
  },
  "checklist": {
    "d280ed1a-9f6b-4f9c-a962-fb4d00dc50ff": {
      "@odata.type": "#microsoft.graph.plannerChecklistItem",
      "isChecked": false,
      "title": "Try reading task details",
      "orderHint": "8587094707721254251P]",
      "lastModifiedBy": {
        "user": {
          "id": "e396de0e-4812-4fcb-9f9e-0358744df343"
        }
      },
      "lastModifiedDateTime": "2017-04-14T02:16:14.866Z"
    }
  },
  "id": "gcrYAaAkgU2EQUvpkNNXLGQAGTtu"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get plannerTaskDetails",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


