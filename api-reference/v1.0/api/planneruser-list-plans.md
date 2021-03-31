---
title: Listar planos
description: Recupere uma lista de objetos **plannerplan** compartilhados com um objeto user.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: apiPageType
ms.openlocfilehash: 6671f06e9ae50ae41aa4cf3c3fbba78d40c2578e
ms.sourcegitcommit: 17f1c9cff2e59049b894db32435af02e4ae32a70
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/31/2021
ms.locfileid: "51473364"
---
# <a name="list-plans"></a><span data-ttu-id="cb850-103">Listar planos</span><span class="sxs-lookup"><span data-stu-id="cb850-103">List plans</span></span>

<span data-ttu-id="cb850-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cb850-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="cb850-105">Recupere uma lista de objetos **plannerplan** compartilhados com um [objeto user.](../resources/user.md)</span><span class="sxs-lookup"><span data-stu-id="cb850-105">Retrieve a list of **plannerplan** objects shared with a [user](../resources/user.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="cb850-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="cb850-106">Permissions</span></span>
<span data-ttu-id="cb850-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cb850-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cb850-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cb850-109">Permission type</span></span>      | <span data-ttu-id="cb850-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="cb850-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cb850-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cb850-111">Delegated (work or school account)</span></span> | <span data-ttu-id="cb850-112">Tasks.Read, Tasks.ReadWrite, Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cb850-112">Tasks.Read, Tasks.ReadWrite, Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="cb850-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cb850-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cb850-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cb850-114">Not supported.</span></span>    |
|<span data-ttu-id="cb850-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cb850-115">Application</span></span> | <span data-ttu-id="cb850-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cb850-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="cb850-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cb850-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/planner/plans
GET /users/{id}/planner/plans
GET /drive/root/createdByUser/planner/plans
```

## <a name="request-headers"></a><span data-ttu-id="cb850-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cb850-118">Request headers</span></span>
| <span data-ttu-id="cb850-119">Nome</span><span class="sxs-lookup"><span data-stu-id="cb850-119">Name</span></span>      |<span data-ttu-id="cb850-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="cb850-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="cb850-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="cb850-121">Authorization</span></span>  | <span data-ttu-id="cb850-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cb850-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cb850-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cb850-124">Request body</span></span>
<span data-ttu-id="cb850-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="cb850-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cb850-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="cb850-126">Response</span></span>

<span data-ttu-id="cb850-127">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [plannerPlan](../resources/plannerplan.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cb850-127">If successful, this method returns a `200 OK` response code and collection of [plannerPlan](../resources/plannerplan.md) objects in the response body.</span></span>

<span data-ttu-id="cb850-128">Este método pode retornar qualquer um dos [códigos de status de HTTP](/graph/errors).</span><span class="sxs-lookup"><span data-stu-id="cb850-128">This method can return any of the [HTTP status codes](/graph/errors).</span></span> <span data-ttu-id="cb850-129">Os erros mais comuns que os aplicativos devem tratar para esse método são as respostas 403 e 404.</span><span class="sxs-lookup"><span data-stu-id="cb850-129">The most common errors that apps should handle for this method are the 403 and 404 responses.</span></span> <span data-ttu-id="cb850-130">Saiba mais sobre esses erros em [Condições de erro comuns do Planner](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="cb850-130">For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="cb850-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="cb850-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="cb850-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cb850-132">Request</span></span>
<span data-ttu-id="cb850-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="cb850-133">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="cb850-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="cb850-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_plans_3"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/planner/plans
```
# <a name="c"></a>[<span data-ttu-id="cb850-135">C#</span><span class="sxs-lookup"><span data-stu-id="cb850-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-plans-3-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="cb850-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cb850-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-plans-3-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cb850-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cb850-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-plans-3-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="cb850-138">Java</span><span class="sxs-lookup"><span data-stu-id="cb850-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-plans-3-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="cb850-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="cb850-139">Response</span></span>
<span data-ttu-id="cb850-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="cb850-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerPlan",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 438

{
  "value": [
    {
      "createdBy": {
        "application": {
          "id": "95e27074-6c4a-447a-aa24-9d718a0b86fa"
        },
        "user": {
          "id": "ebf3b108-5234-4e22-b93d-656d7dae5874"
        }
      },
      "createdDateTime": "2015-03-30T18:36:49.2407981Z",
      "owner": "ebf3b108-5234-4e22-b93d-656d7dae5874",
      "title": "title-value",
      "id": "xqQg5FS2LkCp935s-FIFm2QAFkHM"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List plans",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

