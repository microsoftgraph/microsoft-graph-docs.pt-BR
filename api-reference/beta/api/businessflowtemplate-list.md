---
title: Listar businessFlowTemplates
description: No recurso de análises de acesso do Azure AD, liste todos os objetos businessFlowTemplate.
localization_priority: Normal
doc_type: apiPageType
ms.prod: governance
author: markwahl-msft
ms.openlocfilehash: 1b6a970e9e7336ba4773c3ecbe0e53f7c02e8700
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52047767"
---
# <a name="list-businessflowtemplates"></a><span data-ttu-id="88378-103">Listar businessFlowTemplates</span><span class="sxs-lookup"><span data-stu-id="88378-103">List businessFlowTemplates</span></span>

<span data-ttu-id="88378-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="88378-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="88378-105">No recurso de análises de acesso do Azure [AD,](../resources/accessreviews-root.md) liste todos os [objetos businessFlowTemplate.](../resources/businessflowtemplate.md)</span><span class="sxs-lookup"><span data-stu-id="88378-105">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, list all the [businessFlowTemplate](../resources/businessflowtemplate.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="88378-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="88378-106">Permissions</span></span>
<span data-ttu-id="88378-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="88378-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="88378-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="88378-109">Permission type</span></span>                        | <span data-ttu-id="88378-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="88378-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="88378-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="88378-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="88378-112">AccessReview.Read.All, AccessReview.ReadWrite.Membership, AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="88378-112">AccessReview.Read.All, AccessReview.ReadWrite.Membership, AccessReview.ReadWrite.All</span></span>  |
|<span data-ttu-id="88378-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="88378-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="88378-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="88378-114">Not supported.</span></span> |
|<span data-ttu-id="88378-115">Application</span><span class="sxs-lookup"><span data-stu-id="88378-115">Application</span></span>                            | <span data-ttu-id="88378-116">AccessReview.Read.All, AccessReview.ReadWrite.Membership</span><span class="sxs-lookup"><span data-stu-id="88378-116">AccessReview.Read.All, AccessReview.ReadWrite.Membership</span></span> |

<span data-ttu-id="88378-117">O usuário inscreveu também deve estar em uma função de diretório que permita que ele leia uma revisão de acesso.</span><span class="sxs-lookup"><span data-stu-id="88378-117">The signed in user must also be in a directory role that permits them to read an access review.</span></span>

## <a name="http-request"></a><span data-ttu-id="88378-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="88378-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /businessFlowTemplates
```
## <a name="request-headers"></a><span data-ttu-id="88378-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="88378-119">Request headers</span></span>
| <span data-ttu-id="88378-120">Nome</span><span class="sxs-lookup"><span data-stu-id="88378-120">Name</span></span>         | <span data-ttu-id="88378-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="88378-121">Type</span></span>        | <span data-ttu-id="88378-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="88378-122">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="88378-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="88378-123">Authorization</span></span> | <span data-ttu-id="88378-124">string</span><span class="sxs-lookup"><span data-stu-id="88378-124">string</span></span> | <span data-ttu-id="88378-p102">\{token\} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="88378-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="88378-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="88378-127">Request body</span></span>
<span data-ttu-id="88378-128">Nenhum corpo de solicitação deve ser fornecido.</span><span class="sxs-lookup"><span data-stu-id="88378-128">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="88378-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="88378-129">Response</span></span>
<span data-ttu-id="88378-130">Se tiver êxito, este método retornará um código de resposta e uma `200, OK` matriz de [objetos businessFlowTemplate](../resources/businessflowtemplate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="88378-130">If successful, this method returns a `200, OK` response code and an array of [businessFlowTemplate](../resources/businessflowtemplate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="88378-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="88378-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="88378-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="88378-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="88378-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="88378-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_businessFlowTemplate"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/businessFlowTemplates
```
# <a name="c"></a>[<span data-ttu-id="88378-134">C#</span><span class="sxs-lookup"><span data-stu-id="88378-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-businessflowtemplate-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="88378-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="88378-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-businessflowtemplate-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="88378-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="88378-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-businessflowtemplate-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="88378-137">Java</span><span class="sxs-lookup"><span data-stu-id="88378-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-businessflowtemplate-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="88378-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="88378-138">Response</span></span>
><span data-ttu-id="88378-139">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="88378-139">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.businessFlowTemplate",
    "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value":[
        {
            "id": "842169fe-e1b7-4ce9-98b6-6a9db02eec6b",
            "displayName": "Access reviews of guest user memberships of a group"
        },
        {
            "id": "7fbc909b-efe1-4c72-8ae6-99cb30b882de",
            "displayName": "Access reviews of guest user assignments to an application"
        },
        {
            "id": "50839a84-e23c-44a7-a8cc-16e162afc656",
            "displayName": "Access reviews of assignments to an application"
        },
        {
            "id": "6e4f3d20-c5c3-407f-9695-8460952bcc68",
            "displayName": "Access reviews of memberships of a group"
        },
        {
            "id": "d7e0b82d-997f-44d0-ac5e-de9deb087c15",
            "displayName": "Access reviews of memberships of an Azure AD role"
        }
    ]
}

```

## <a name="see-also"></a><span data-ttu-id="88378-140">Confira também</span><span class="sxs-lookup"><span data-stu-id="88378-140">See also</span></span>

| <span data-ttu-id="88378-141">Método</span><span class="sxs-lookup"><span data-stu-id="88378-141">Method</span></span>           | <span data-ttu-id="88378-142">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="88378-142">Return Type</span></span>    |<span data-ttu-id="88378-143">Descrição</span><span class="sxs-lookup"><span data-stu-id="88378-143">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="88378-144">Criar accessReview</span><span class="sxs-lookup"><span data-stu-id="88378-144">Create accessReview</span></span>](accessreview-create.md) |    [<span data-ttu-id="88378-145">accessReview</span><span class="sxs-lookup"><span data-stu-id="88378-145">accessReview</span></span>](../resources/accessreview.md) |  <span data-ttu-id="88378-146">Crie um novo accessReview.</span><span class="sxs-lookup"><span data-stu-id="88378-146">Create a new accessReview.</span></span> |




<!--
{
  "type": "#page.annotation",
  "description": "List business flow template",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


