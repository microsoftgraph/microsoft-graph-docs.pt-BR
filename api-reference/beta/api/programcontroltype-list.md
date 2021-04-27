---
title: Listar programControlTypes
description: No recurso de revisões de acesso do Azure AD, liste todos os objetos programControlType.
localization_priority: Normal
doc_type: apiPageType
ms.prod: governance
author: markwahl-msft
ms.openlocfilehash: aea4607e5020207ecfe85968d5048dd33f1f9b3e
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52055208"
---
# <a name="list-programcontroltypes"></a><span data-ttu-id="c5565-103">Listar programControlTypes</span><span class="sxs-lookup"><span data-stu-id="c5565-103">List programControlTypes</span></span>

<span data-ttu-id="c5565-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c5565-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c5565-105">No recurso de revisões de acesso do Azure [AD,](../resources/accessreviews-root.md) liste todos os [objetos programControlType.](../resources/programcontroltype.md)</span><span class="sxs-lookup"><span data-stu-id="c5565-105">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, list all the [programControlType](../resources/programcontroltype.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="c5565-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="c5565-106">Permissions</span></span>
<span data-ttu-id="c5565-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c5565-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c5565-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c5565-109">Permission type</span></span>                        | <span data-ttu-id="c5565-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c5565-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="c5565-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c5565-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="c5565-112">ProgramControl.Read.All, ProgramControl.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c5565-112">ProgramControl.Read.All, ProgramControl.ReadWrite.All</span></span>   |
|<span data-ttu-id="c5565-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c5565-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c5565-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c5565-114">Not supported.</span></span> |
|<span data-ttu-id="c5565-115">Application</span><span class="sxs-lookup"><span data-stu-id="c5565-115">Application</span></span>                            | <span data-ttu-id="c5565-116">ProgramControl.Read.All', ProgramControl.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c5565-116">ProgramControl.Read.All\`, ProgramControl.ReadWrite.All</span></span>  |

<span data-ttu-id="c5565-117">O usuário inscreveu também deve estar em uma função de diretório que permita que ele leia um programa.</span><span class="sxs-lookup"><span data-stu-id="c5565-117">The signed in user must also be in a directory role that permits them to read a program.</span></span>

## <a name="http-request"></a><span data-ttu-id="c5565-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c5565-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /programControlTypes
```
## <a name="request-headers"></a><span data-ttu-id="c5565-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c5565-119">Request headers</span></span>
| <span data-ttu-id="c5565-120">Nome</span><span class="sxs-lookup"><span data-stu-id="c5565-120">Name</span></span>         | <span data-ttu-id="c5565-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="c5565-121">Type</span></span>        | <span data-ttu-id="c5565-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="c5565-122">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="c5565-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="c5565-123">Authorization</span></span> | <span data-ttu-id="c5565-124">string</span><span class="sxs-lookup"><span data-stu-id="c5565-124">string</span></span> | <span data-ttu-id="c5565-p102">\{token\} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c5565-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c5565-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c5565-127">Request body</span></span>
<span data-ttu-id="c5565-128">Nenhum corpo de solicitação deve ser fornecido.</span><span class="sxs-lookup"><span data-stu-id="c5565-128">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="c5565-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="c5565-129">Response</span></span>
<span data-ttu-id="c5565-130">Se tiver êxito, este método retornará um código de resposta e uma `200, OK` matriz de [objetos programControlType](../resources/programcontroltype.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c5565-130">If successful, this method returns a `200, OK` response code and an array of [programControlType](../resources/programcontroltype.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c5565-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c5565-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c5565-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c5565-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="c5565-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="c5565-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_programcontroltype"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/programControlTypes
```
# <a name="c"></a>[<span data-ttu-id="c5565-134">C#</span><span class="sxs-lookup"><span data-stu-id="c5565-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-programcontroltype-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c5565-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c5565-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-programcontroltype-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c5565-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c5565-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-programcontroltype-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c5565-137">Java</span><span class="sxs-lookup"><span data-stu-id="c5565-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-programcontroltype-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="c5565-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="c5565-138">Response</span></span>
><span data-ttu-id="c5565-139">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="c5565-139">**Note:** The response object shown here might be shortened for readability.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="c5565-140">Confira também</span><span class="sxs-lookup"><span data-stu-id="c5565-140">See also</span></span>

| <span data-ttu-id="c5565-141">Método</span><span class="sxs-lookup"><span data-stu-id="c5565-141">Method</span></span>           | <span data-ttu-id="c5565-142">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="c5565-142">Return Type</span></span>    |<span data-ttu-id="c5565-143">Descrição</span><span class="sxs-lookup"><span data-stu-id="c5565-143">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="c5565-144">Listar programControls de um programa</span><span class="sxs-lookup"><span data-stu-id="c5565-144">List programControls of a program</span></span>](program-listcontrols.md) |     <span data-ttu-id="c5565-145">[Coleção programControl](../resources/programcontrol.md)</span><span class="sxs-lookup"><span data-stu-id="c5565-145">[programControl](../resources/programcontrol.md) collection</span></span>|    <span data-ttu-id="c5565-146">Obter uma coleção dos controles de um programa.</span><span class="sxs-lookup"><span data-stu-id="c5565-146">Get a collection of the controls of a program.</span></span>|


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


