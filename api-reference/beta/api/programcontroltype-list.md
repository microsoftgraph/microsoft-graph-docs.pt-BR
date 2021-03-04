---
title: Listar programControlTypes
description: No recurso de revisões de acesso do Azure AD, liste todos os objetos programControlType.
localization_priority: Normal
doc_type: apiPageType
ms.prod: governance
author: markwahl-msft
ms.openlocfilehash: b693b47f716c9f89a49bee9c76baf5025fa0bd61
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50442184"
---
# <a name="list-programcontroltypes"></a><span data-ttu-id="5ecb4-103">Listar programControlTypes</span><span class="sxs-lookup"><span data-stu-id="5ecb4-103">List programControlTypes</span></span>

<span data-ttu-id="5ecb4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5ecb4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5ecb4-105">No recurso de revisões de acesso do Azure [AD,](../resources/accessreviews-root.md) liste todos os [objetos programControlType.](../resources/programcontroltype.md)</span><span class="sxs-lookup"><span data-stu-id="5ecb4-105">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, list all the [programControlType](../resources/programcontroltype.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="5ecb4-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="5ecb4-106">Permissions</span></span>
<span data-ttu-id="5ecb4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5ecb4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5ecb4-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5ecb4-109">Permission type</span></span>                        | <span data-ttu-id="5ecb4-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5ecb4-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="5ecb4-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5ecb4-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="5ecb4-112">ProgramControl.Read.All, ProgramControl.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5ecb4-112">ProgramControl.Read.All, ProgramControl.ReadWrite.All</span></span>   |
|<span data-ttu-id="5ecb4-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5ecb4-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5ecb4-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5ecb4-114">Not supported.</span></span> |
|<span data-ttu-id="5ecb4-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5ecb4-115">Application</span></span>                            | <span data-ttu-id="5ecb4-116">ProgramControl.Read.All', ProgramControl.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5ecb4-116">ProgramControl.Read.All\`, ProgramControl.ReadWrite.All</span></span>  |

<span data-ttu-id="5ecb4-117">O usuário inscreveu também deve estar em uma função de diretório que permita que ele leia um programa.</span><span class="sxs-lookup"><span data-stu-id="5ecb4-117">The signed in user must also be in a directory role that permits them to read a program.</span></span>

## <a name="http-request"></a><span data-ttu-id="5ecb4-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5ecb4-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /programControlTypes
```
## <a name="request-headers"></a><span data-ttu-id="5ecb4-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5ecb4-119">Request headers</span></span>
| <span data-ttu-id="5ecb4-120">Nome</span><span class="sxs-lookup"><span data-stu-id="5ecb4-120">Name</span></span>         | <span data-ttu-id="5ecb4-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="5ecb4-121">Type</span></span>        | <span data-ttu-id="5ecb4-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="5ecb4-122">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="5ecb4-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="5ecb4-123">Authorization</span></span> | <span data-ttu-id="5ecb4-124">string</span><span class="sxs-lookup"><span data-stu-id="5ecb4-124">string</span></span> | <span data-ttu-id="5ecb4-p102">\{token\} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5ecb4-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5ecb4-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5ecb4-127">Request body</span></span>
<span data-ttu-id="5ecb4-128">Nenhum corpo de solicitação deve ser fornecido.</span><span class="sxs-lookup"><span data-stu-id="5ecb4-128">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="5ecb4-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="5ecb4-129">Response</span></span>
<span data-ttu-id="5ecb4-130">Se tiver êxito, este método retornará um código de resposta e uma `200, OK` matriz de [objetos programControlType](../resources/programcontroltype.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5ecb4-130">If successful, this method returns a `200, OK` response code and an array of [programControlType](../resources/programcontroltype.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5ecb4-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5ecb4-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5ecb4-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5ecb4-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="5ecb4-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="5ecb4-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_programcontroltype"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/programControlTypes
```
# <a name="c"></a>[<span data-ttu-id="5ecb4-134">C#</span><span class="sxs-lookup"><span data-stu-id="5ecb4-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-programcontroltype-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5ecb4-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5ecb4-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-programcontroltype-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5ecb4-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5ecb4-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-programcontroltype-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5ecb4-137">Java</span><span class="sxs-lookup"><span data-stu-id="5ecb4-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-programcontroltype-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="5ecb4-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="5ecb4-138">Response</span></span>
><span data-ttu-id="5ecb4-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5ecb4-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.programControlType",
    "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value":[
        {
            "id": "842169fe-e1b7-4ce9-98b6-6a9db02eec6b",
            "displayName": "Access Reviews for External Users' access to groups"
        },
        {
            "id": "7fbc909b-efe1-4c72-8ae6-99cb30b882de",
            "displayName": "Access Reviews for External Users' access to applications"
        },
        {
            "id": "50839a84-e23c-44a7-a8cc-16e162afc656",
            "displayName": "Access Reviews for All Users' assignment to applications"
        },
        {
            "id": "6e4f3d20-c5c3-407f-9695-8460952bcc68",
            "displayName": "Access Reviews for Microsoft 365 groups' membership"
        }
    ]
}

```

## <a name="see-also"></a><span data-ttu-id="5ecb4-141">Confira também</span><span class="sxs-lookup"><span data-stu-id="5ecb4-141">See also</span></span>

| <span data-ttu-id="5ecb4-142">Método</span><span class="sxs-lookup"><span data-stu-id="5ecb4-142">Method</span></span>           | <span data-ttu-id="5ecb4-143">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="5ecb4-143">Return Type</span></span>    |<span data-ttu-id="5ecb4-144">Descrição</span><span class="sxs-lookup"><span data-stu-id="5ecb4-144">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="5ecb4-145">Listar programControls de um programa</span><span class="sxs-lookup"><span data-stu-id="5ecb4-145">List programControls of a program</span></span>](program-listcontrols.md) |     <span data-ttu-id="5ecb4-146">[Coleção programControl](../resources/programcontrol.md)</span><span class="sxs-lookup"><span data-stu-id="5ecb4-146">[programControl](../resources/programcontrol.md) collection</span></span>|    <span data-ttu-id="5ecb4-147">Obter uma coleção dos controles de um programa.</span><span class="sxs-lookup"><span data-stu-id="5ecb4-147">Get a collection of the controls of a program.</span></span>|


<!--
{
  "type": "#page.annotation",
  "description": "List program control types",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


