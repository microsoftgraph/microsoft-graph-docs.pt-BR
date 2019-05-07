---
title: Listar planos
description: Recupere uma lista de objetos **plannerplan** compartilhados com um objeto user.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 730eb1e491372a8ee342e0b6a840f556eee55ef3
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33608465"
---
# <a name="list-plans"></a><span data-ttu-id="045c5-103">Listar planos</span><span class="sxs-lookup"><span data-stu-id="045c5-103">List plans</span></span>

<span data-ttu-id="045c5-104">Recupere uma lista de objetos **plannerplan** compartilhados com um objeto [User](../resources/user.md) .</span><span class="sxs-lookup"><span data-stu-id="045c5-104">Retrieve a list of **plannerplan** objects shared with a [user](../resources/user.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="045c5-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="045c5-105">Permissions</span></span>
<span data-ttu-id="045c5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="045c5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="045c5-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="045c5-108">Permission type</span></span>      | <span data-ttu-id="045c5-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="045c5-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="045c5-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="045c5-110">Delegated (work or school account)</span></span> | <span data-ttu-id="045c5-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="045c5-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="045c5-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="045c5-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="045c5-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="045c5-113">Not supported.</span></span>    |
|<span data-ttu-id="045c5-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="045c5-114">Application</span></span> | <span data-ttu-id="045c5-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="045c5-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="045c5-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="045c5-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/planner/plans
GET /users/{id}/planner/plans
GET /drive/root/createdByUser/planner/plans
```

## <a name="request-headers"></a><span data-ttu-id="045c5-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="045c5-117">Request headers</span></span>
| <span data-ttu-id="045c5-118">Nome</span><span class="sxs-lookup"><span data-stu-id="045c5-118">Name</span></span>      |<span data-ttu-id="045c5-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="045c5-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="045c5-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="045c5-120">Authorization</span></span>  | <span data-ttu-id="045c5-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="045c5-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="045c5-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="045c5-123">Request body</span></span>
<span data-ttu-id="045c5-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="045c5-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="045c5-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="045c5-125">Response</span></span>

<span data-ttu-id="045c5-126">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [plannerPlan](../resources/plannerplan.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="045c5-126">If successful, this method returns a `200 OK` response code and collection of [plannerPlan](../resources/plannerplan.md) objects in the response body.</span></span>

<span data-ttu-id="045c5-127">Este método pode retornar qualquer um dos [códigos de status de HTTP](/graph/errors).</span><span class="sxs-lookup"><span data-stu-id="045c5-127">This method can return any of the [HTTP status codes](/graph/errors).</span></span> <span data-ttu-id="045c5-128">Os erros mais comuns que os aplicativos devem tratar para esse método são as respostas 403 e 404.</span><span class="sxs-lookup"><span data-stu-id="045c5-128">The most common errors that apps should handle for this method are the 403 and 404 responses.</span></span> <span data-ttu-id="045c5-129">Saiba mais sobre esses erros em [Condições de erro comuns do Planner](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="045c5-129">For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="045c5-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="045c5-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="045c5-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="045c5-131">Request</span></span>
<span data-ttu-id="045c5-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="045c5-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_plans"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/planner/plans
```
##### <a name="response"></a><span data-ttu-id="045c5-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="045c5-133">Response</span></span>
<span data-ttu-id="045c5-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="045c5-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="045c5-137">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="045c5-137">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="045c5-138">Basic</span><span class="sxs-lookup"><span data-stu-id="045c5-138">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_plans-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="045c5-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="045c5-139">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_plans-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List plans",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/planneruser-list-plans.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/planneruser-list-plans.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
