---
title: Listar programas
description: No recurso de revisões do Azure AD Access, liste todos os objetos de programa.
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: d71f4c550bbde753a9f77008a6f2ad1c7e89e265
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35978596"
---
# <a name="list-programs"></a><span data-ttu-id="0f685-103">Listar programas</span><span class="sxs-lookup"><span data-stu-id="0f685-103">List programs</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0f685-104">No recurso de revisões do Azure AD [Access](../resources/accessreviews-root.md) , liste todos os objetos de [programa](../resources/program.md) .</span><span class="sxs-lookup"><span data-stu-id="0f685-104">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, list all the [program](../resources/program.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="0f685-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="0f685-105">Permissions</span></span>
<span data-ttu-id="0f685-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0f685-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0f685-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0f685-108">Permission type</span></span>                        | <span data-ttu-id="0f685-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0f685-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="0f685-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0f685-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="0f685-111">ProgramControl. Read. All, ProgramControl. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="0f685-111">ProgramControl.Read.All, ProgramControl.ReadWrite.All</span></span>  |
|<span data-ttu-id="0f685-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0f685-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0f685-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0f685-113">Not supported.</span></span> |
|<span data-ttu-id="0f685-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0f685-114">Application</span></span>                            | <span data-ttu-id="0f685-115">ProgramControl. Read. All, ProgramControl. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="0f685-115">ProgramControl.Read.All, ProgramControl.ReadWrite.All</span></span>  |

 <span data-ttu-id="0f685-116">O usuário conectado também deve estar em uma função de diretório que permite que ele leia um programa.</span><span class="sxs-lookup"><span data-stu-id="0f685-116">The signed in user must also be in a directory role that permits them to read a program.</span></span>

## <a name="http-request"></a><span data-ttu-id="0f685-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0f685-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /programs
```
## <a name="request-headers"></a><span data-ttu-id="0f685-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0f685-118">Request headers</span></span>
| <span data-ttu-id="0f685-119">Nome</span><span class="sxs-lookup"><span data-stu-id="0f685-119">Name</span></span>         | <span data-ttu-id="0f685-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="0f685-120">Type</span></span>        | <span data-ttu-id="0f685-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="0f685-121">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="0f685-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="0f685-122">Authorization</span></span> | <span data-ttu-id="0f685-123">string</span><span class="sxs-lookup"><span data-stu-id="0f685-123">string</span></span> | <span data-ttu-id="0f685-p102">\{token\} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0f685-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0f685-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0f685-126">Request body</span></span>
<span data-ttu-id="0f685-127">Nenhum corpo de solicitação deve ser fornecido.</span><span class="sxs-lookup"><span data-stu-id="0f685-127">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="0f685-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="0f685-128">Response</span></span>
<span data-ttu-id="0f685-129">Se tiver êxito, este método retornará `200, OK` um código de resposta e uma matriz de objetos de [programa](../resources/program.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0f685-129">If successful, this method returns a `200, OK` response code and an array of [program](../resources/program.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0f685-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0f685-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0f685-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0f685-131">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="0f685-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="0f685-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_program"
}-->
```http
GET https://graph.microsoft.com/beta/programs
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="0f685-133">C#</span><span class="sxs-lookup"><span data-stu-id="0f685-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-program-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0f685-134">Javascript</span><span class="sxs-lookup"><span data-stu-id="0f685-134">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-program-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="0f685-135">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="0f685-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-program-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="0f685-136">Java</span><span class="sxs-lookup"><span data-stu-id="0f685-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-program-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="0f685-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="0f685-137">Response</span></span>
><span data-ttu-id="0f685-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0f685-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="0f685-140">Confira também</span><span class="sxs-lookup"><span data-stu-id="0f685-140">See also</span></span>

| <span data-ttu-id="0f685-141">Método</span><span class="sxs-lookup"><span data-stu-id="0f685-141">Method</span></span>           | <span data-ttu-id="0f685-142">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="0f685-142">Return Type</span></span>    |<span data-ttu-id="0f685-143">Descrição</span><span class="sxs-lookup"><span data-stu-id="0f685-143">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="0f685-144">Listar programControls de um programa</span><span class="sxs-lookup"><span data-stu-id="0f685-144">List programControls of a program</span></span>](program-listcontrols.md) |     <span data-ttu-id="0f685-145">coleção [programControl](../resources/programcontrol.md)</span><span class="sxs-lookup"><span data-stu-id="0f685-145">[programControl](../resources/programcontrol.md) collection</span></span>|    <span data-ttu-id="0f685-146">Obter uma coleção de controles de um programa.</span><span class="sxs-lookup"><span data-stu-id="0f685-146">Get a collection of the controls of a program.</span></span>|


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
