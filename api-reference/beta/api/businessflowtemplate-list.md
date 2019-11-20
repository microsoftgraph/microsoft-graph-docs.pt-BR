---
title: Listar businessFlowTemplates
description: No recurso de revisões do Azure AD Access, liste todos os objetos businessFlowTemplate.
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: markwahl-msft
ms.openlocfilehash: 8a46bff027ecfa98924fbfe66b6fd8b2b8035efd
ms.sourcegitcommit: d40d2a9266bd376d713382925323aefab285ed69
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/20/2019
ms.locfileid: "38747599"
---
# <a name="list-businessflowtemplates"></a><span data-ttu-id="bd6dd-103">Listar businessFlowTemplates</span><span class="sxs-lookup"><span data-stu-id="bd6dd-103">List businessFlowTemplates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bd6dd-104">No recurso de revisões do Azure AD [Access](../resources/accessreviews-root.md) , liste todos os objetos [businessFlowTemplate](../resources/businessflowtemplate.md) .</span><span class="sxs-lookup"><span data-stu-id="bd6dd-104">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, list all the [businessFlowTemplate](../resources/businessflowtemplate.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="bd6dd-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="bd6dd-105">Permissions</span></span>
<span data-ttu-id="bd6dd-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bd6dd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bd6dd-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bd6dd-108">Permission type</span></span>                        | <span data-ttu-id="bd6dd-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="bd6dd-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="bd6dd-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bd6dd-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="bd6dd-111">AccessReview. Read. All, AccessReview. ReadWrite. Membership, AccessReview. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="bd6dd-111">AccessReview.Read.All, AccessReview.ReadWrite.Membership, AccessReview.ReadWrite.All</span></span>  |
|<span data-ttu-id="bd6dd-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bd6dd-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bd6dd-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bd6dd-113">Not supported.</span></span> |
|<span data-ttu-id="bd6dd-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bd6dd-114">Application</span></span>                            | <span data-ttu-id="bd6dd-115">AccessReview. Read. All, AccessReview. ReadWrite. Membership</span><span class="sxs-lookup"><span data-stu-id="bd6dd-115">AccessReview.Read.All, AccessReview.ReadWrite.Membership</span></span> |

<span data-ttu-id="bd6dd-116">O usuário conectado também deve estar em uma função de diretório que permite que ele leia uma revisão do Access.</span><span class="sxs-lookup"><span data-stu-id="bd6dd-116">The signed in user must also be in a directory role that permits them to read an access review.</span></span>

## <a name="http-request"></a><span data-ttu-id="bd6dd-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bd6dd-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /businessFlowTemplates
```
## <a name="request-headers"></a><span data-ttu-id="bd6dd-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bd6dd-118">Request headers</span></span>
| <span data-ttu-id="bd6dd-119">Nome</span><span class="sxs-lookup"><span data-stu-id="bd6dd-119">Name</span></span>         | <span data-ttu-id="bd6dd-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="bd6dd-120">Type</span></span>        | <span data-ttu-id="bd6dd-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="bd6dd-121">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="bd6dd-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="bd6dd-122">Authorization</span></span> | <span data-ttu-id="bd6dd-123">string</span><span class="sxs-lookup"><span data-stu-id="bd6dd-123">string</span></span> | <span data-ttu-id="bd6dd-p102">\{token\} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bd6dd-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="bd6dd-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bd6dd-126">Request body</span></span>
<span data-ttu-id="bd6dd-127">Nenhum corpo de solicitação deve ser fornecido.</span><span class="sxs-lookup"><span data-stu-id="bd6dd-127">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="bd6dd-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="bd6dd-128">Response</span></span>
<span data-ttu-id="bd6dd-129">Se tiver êxito, este método retornará `200, OK` um código de resposta e uma matriz de objetos [businessFlowTemplate](../resources/businessflowtemplate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bd6dd-129">If successful, this method returns a `200, OK` response code and an array of [businessFlowTemplate](../resources/businessflowtemplate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bd6dd-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bd6dd-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="bd6dd-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bd6dd-131">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="bd6dd-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="bd6dd-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_businessFlowTemplate"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/businessFlowTemplates
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="bd6dd-133">C#</span><span class="sxs-lookup"><span data-stu-id="bd6dd-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-businessflowtemplate-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="bd6dd-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bd6dd-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-businessflowtemplate-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="bd6dd-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bd6dd-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-businessflowtemplate-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="bd6dd-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="bd6dd-136">Response</span></span>
><span data-ttu-id="bd6dd-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="bd6dd-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="bd6dd-139">Confira também</span><span class="sxs-lookup"><span data-stu-id="bd6dd-139">See also</span></span>

| <span data-ttu-id="bd6dd-140">Método</span><span class="sxs-lookup"><span data-stu-id="bd6dd-140">Method</span></span>           | <span data-ttu-id="bd6dd-141">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="bd6dd-141">Return Type</span></span>    |<span data-ttu-id="bd6dd-142">Descrição</span><span class="sxs-lookup"><span data-stu-id="bd6dd-142">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="bd6dd-143">Criar accessReview</span><span class="sxs-lookup"><span data-stu-id="bd6dd-143">Create accessReview</span></span>](accessreview-create.md) |    [<span data-ttu-id="bd6dd-144">accessReview</span><span class="sxs-lookup"><span data-stu-id="bd6dd-144">accessReview</span></span>](../resources/accessreview.md) |  <span data-ttu-id="bd6dd-145">Criar um novo accessReview.</span><span class="sxs-lookup"><span data-stu-id="bd6dd-145">Create a new accessReview.</span></span> |




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
