---
title: Listar businessFlowTemplates
description: No recurso de revisões do Azure AD Access, liste todos os objetos businessFlowTemplate.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: markwahl-msft
ms.openlocfilehash: 3ea42f9d287aa255390fec357708643058c4c6b5
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48960135"
---
# <a name="list-businessflowtemplates"></a><span data-ttu-id="aa90e-103">Listar businessFlowTemplates</span><span class="sxs-lookup"><span data-stu-id="aa90e-103">List businessFlowTemplates</span></span>

<span data-ttu-id="aa90e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="aa90e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="aa90e-105">No recurso de revisões do Azure AD [Access](../resources/accessreviews-root.md) , liste todos os objetos [businessFlowTemplate](../resources/businessflowtemplate.md) .</span><span class="sxs-lookup"><span data-stu-id="aa90e-105">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, list all the [businessFlowTemplate](../resources/businessflowtemplate.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="aa90e-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="aa90e-106">Permissions</span></span>
<span data-ttu-id="aa90e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="aa90e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="aa90e-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="aa90e-109">Permission type</span></span>                        | <span data-ttu-id="aa90e-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="aa90e-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="aa90e-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="aa90e-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="aa90e-112">AccessReview. Read. All, AccessReview. ReadWrite. Membership, AccessReview. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="aa90e-112">AccessReview.Read.All, AccessReview.ReadWrite.Membership, AccessReview.ReadWrite.All</span></span>  |
|<span data-ttu-id="aa90e-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="aa90e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="aa90e-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="aa90e-114">Not supported.</span></span> |
|<span data-ttu-id="aa90e-115">Application</span><span class="sxs-lookup"><span data-stu-id="aa90e-115">Application</span></span>                            | <span data-ttu-id="aa90e-116">AccessReview. Read. All, AccessReview. ReadWrite. Membership</span><span class="sxs-lookup"><span data-stu-id="aa90e-116">AccessReview.Read.All, AccessReview.ReadWrite.Membership</span></span> |

<span data-ttu-id="aa90e-117">O usuário conectado também deve estar em uma função de diretório que permite que ele leia uma revisão do Access.</span><span class="sxs-lookup"><span data-stu-id="aa90e-117">The signed in user must also be in a directory role that permits them to read an access review.</span></span>

## <a name="http-request"></a><span data-ttu-id="aa90e-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="aa90e-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /businessFlowTemplates
```
## <a name="request-headers"></a><span data-ttu-id="aa90e-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="aa90e-119">Request headers</span></span>
| <span data-ttu-id="aa90e-120">Nome</span><span class="sxs-lookup"><span data-stu-id="aa90e-120">Name</span></span>         | <span data-ttu-id="aa90e-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="aa90e-121">Type</span></span>        | <span data-ttu-id="aa90e-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="aa90e-122">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="aa90e-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="aa90e-123">Authorization</span></span> | <span data-ttu-id="aa90e-124">string</span><span class="sxs-lookup"><span data-stu-id="aa90e-124">string</span></span> | <span data-ttu-id="aa90e-p102">\{token\} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="aa90e-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="aa90e-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="aa90e-127">Request body</span></span>
<span data-ttu-id="aa90e-128">Nenhum corpo de solicitação deve ser fornecido.</span><span class="sxs-lookup"><span data-stu-id="aa90e-128">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="aa90e-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="aa90e-129">Response</span></span>
<span data-ttu-id="aa90e-130">Se tiver êxito, este método retornará um `200, OK` código de resposta e uma matriz de objetos [businessFlowTemplate](../resources/businessflowtemplate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="aa90e-130">If successful, this method returns a `200, OK` response code and an array of [businessFlowTemplate](../resources/businessflowtemplate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="aa90e-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="aa90e-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="aa90e-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="aa90e-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="aa90e-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="aa90e-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_businessFlowTemplate"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/businessFlowTemplates
```
# <a name="c"></a>[<span data-ttu-id="aa90e-134">C#</span><span class="sxs-lookup"><span data-stu-id="aa90e-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-businessflowtemplate-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="aa90e-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="aa90e-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-businessflowtemplate-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="aa90e-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="aa90e-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-businessflowtemplate-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="aa90e-137">Java</span><span class="sxs-lookup"><span data-stu-id="aa90e-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-businessflowtemplate-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="aa90e-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="aa90e-138">Response</span></span>
><span data-ttu-id="aa90e-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="aa90e-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="aa90e-141">Confira também</span><span class="sxs-lookup"><span data-stu-id="aa90e-141">See also</span></span>

| <span data-ttu-id="aa90e-142">Método</span><span class="sxs-lookup"><span data-stu-id="aa90e-142">Method</span></span>           | <span data-ttu-id="aa90e-143">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="aa90e-143">Return Type</span></span>    |<span data-ttu-id="aa90e-144">Descrição</span><span class="sxs-lookup"><span data-stu-id="aa90e-144">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="aa90e-145">Criar accessReview</span><span class="sxs-lookup"><span data-stu-id="aa90e-145">Create accessReview</span></span>](accessreview-create.md) |    [<span data-ttu-id="aa90e-146">accessReview</span><span class="sxs-lookup"><span data-stu-id="aa90e-146">accessReview</span></span>](../resources/accessreview.md) |  <span data-ttu-id="aa90e-147">Criar um novo accessReview.</span><span class="sxs-lookup"><span data-stu-id="aa90e-147">Create a new accessReview.</span></span> |




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


