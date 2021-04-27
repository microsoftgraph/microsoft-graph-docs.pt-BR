---
title: Listar programas
description: No recurso de revisões de acesso do Azure AD, liste todos os objetos do programa.
localization_priority: Normal
doc_type: apiPageType
ms.prod: governance
author: markwahl-msft
ms.openlocfilehash: 4995cd66af99031051e67a2853f4a2453430f684
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52049832"
---
# <a name="list-programs"></a><span data-ttu-id="8c0e2-103">Listar programas</span><span class="sxs-lookup"><span data-stu-id="8c0e2-103">List programs</span></span>

<span data-ttu-id="8c0e2-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8c0e2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8c0e2-105">No recurso de revisões de acesso do Azure [AD,](../resources/accessreviews-root.md) liste todos os [objetos do](../resources/program.md) programa.</span><span class="sxs-lookup"><span data-stu-id="8c0e2-105">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, list all the [program](../resources/program.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="8c0e2-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="8c0e2-106">Permissions</span></span>
<span data-ttu-id="8c0e2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8c0e2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8c0e2-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8c0e2-109">Permission type</span></span>                        | <span data-ttu-id="8c0e2-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8c0e2-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="8c0e2-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8c0e2-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="8c0e2-112">ProgramControl.Read.All, ProgramControl.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8c0e2-112">ProgramControl.Read.All, ProgramControl.ReadWrite.All</span></span>  |
|<span data-ttu-id="8c0e2-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8c0e2-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8c0e2-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8c0e2-114">Not supported.</span></span> |
|<span data-ttu-id="8c0e2-115">Application</span><span class="sxs-lookup"><span data-stu-id="8c0e2-115">Application</span></span>                            | <span data-ttu-id="8c0e2-116">ProgramControl.Read.All, ProgramControl.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8c0e2-116">ProgramControl.Read.All, ProgramControl.ReadWrite.All</span></span>  |

 <span data-ttu-id="8c0e2-117">O usuário inscreveu também deve estar em uma função de diretório que permita que ele leia um programa.</span><span class="sxs-lookup"><span data-stu-id="8c0e2-117">The signed in user must also be in a directory role that permits them to read a program.</span></span>

## <a name="http-request"></a><span data-ttu-id="8c0e2-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8c0e2-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /programs
```
## <a name="request-headers"></a><span data-ttu-id="8c0e2-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8c0e2-119">Request headers</span></span>
| <span data-ttu-id="8c0e2-120">Nome</span><span class="sxs-lookup"><span data-stu-id="8c0e2-120">Name</span></span>         | <span data-ttu-id="8c0e2-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="8c0e2-121">Type</span></span>        | <span data-ttu-id="8c0e2-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="8c0e2-122">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="8c0e2-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="8c0e2-123">Authorization</span></span> | <span data-ttu-id="8c0e2-124">string</span><span class="sxs-lookup"><span data-stu-id="8c0e2-124">string</span></span> | <span data-ttu-id="8c0e2-p102">\{token\} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8c0e2-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8c0e2-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8c0e2-127">Request body</span></span>
<span data-ttu-id="8c0e2-128">Nenhum corpo de solicitação deve ser fornecido.</span><span class="sxs-lookup"><span data-stu-id="8c0e2-128">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="8c0e2-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="8c0e2-129">Response</span></span>
<span data-ttu-id="8c0e2-130">Se tiver êxito, este método retornará um código de resposta e uma matriz de objetos `200, OK` [de](../resources/program.md) programa no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8c0e2-130">If successful, this method returns a `200, OK` response code and an array of [program](../resources/program.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8c0e2-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8c0e2-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8c0e2-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8c0e2-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="8c0e2-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="8c0e2-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_program"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/programs
```
# <a name="c"></a>[<span data-ttu-id="8c0e2-134">C#</span><span class="sxs-lookup"><span data-stu-id="8c0e2-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-program-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8c0e2-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8c0e2-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-program-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8c0e2-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8c0e2-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-program-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8c0e2-137">Java</span><span class="sxs-lookup"><span data-stu-id="8c0e2-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-program-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="8c0e2-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="8c0e2-138">Response</span></span>
><span data-ttu-id="8c0e2-139">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="8c0e2-139">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.program",
    "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
        {
            "id": "7e59d237-2fb0-4e5d-b7bb-d4f9f9129213",
            "displayName": "testprogram3",
            "description": "test description"
        },
        {
            "id": "b4afdd74-b6cf-4239-9b08-dde9a91d18d2",
            "displayName": "Default Program",
            "description": "Built-in program to start managing access reviews"
        }
    ]
}

```

## <a name="see-also"></a><span data-ttu-id="8c0e2-140">Confira também</span><span class="sxs-lookup"><span data-stu-id="8c0e2-140">See also</span></span>

| <span data-ttu-id="8c0e2-141">Método</span><span class="sxs-lookup"><span data-stu-id="8c0e2-141">Method</span></span>           | <span data-ttu-id="8c0e2-142">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="8c0e2-142">Return Type</span></span>    |<span data-ttu-id="8c0e2-143">Descrição</span><span class="sxs-lookup"><span data-stu-id="8c0e2-143">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="8c0e2-144">Listar programControls de um programa</span><span class="sxs-lookup"><span data-stu-id="8c0e2-144">List programControls of a program</span></span>](program-listcontrols.md) |     <span data-ttu-id="8c0e2-145">[Coleção programControl](../resources/programcontrol.md)</span><span class="sxs-lookup"><span data-stu-id="8c0e2-145">[programControl](../resources/programcontrol.md) collection</span></span>|    <span data-ttu-id="8c0e2-146">Obter uma coleção dos controles de um programa.</span><span class="sxs-lookup"><span data-stu-id="8c0e2-146">Get a collection of the controls of a program.</span></span>|


<!--
{
  "type": "#page.annotation",
  "description": "List programs",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


