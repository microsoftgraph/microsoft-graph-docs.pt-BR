---
title: Listar programas
description: No recurso de revisões do Azure AD Access, liste todos os objetos de programa.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: markwahl-msft
ms.openlocfilehash: eab96053d43634cd4280e2e633b1de5da8ff5a17
ms.sourcegitcommit: bd40e302ce04b686e86989246ab7c4cc9ad3f320
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/03/2020
ms.locfileid: "43123059"
---
# <a name="list-programs"></a><span data-ttu-id="aafbd-103">Listar programas</span><span class="sxs-lookup"><span data-stu-id="aafbd-103">List programs</span></span>

<span data-ttu-id="aafbd-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="aafbd-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="aafbd-105">No recurso de revisões do Azure AD [Access](../resources/accessreviews-root.md) , liste todos os objetos de [programa](../resources/program.md) .</span><span class="sxs-lookup"><span data-stu-id="aafbd-105">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, list all the [program](../resources/program.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="aafbd-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="aafbd-106">Permissions</span></span>
<span data-ttu-id="aafbd-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="aafbd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="aafbd-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="aafbd-109">Permission type</span></span>                        | <span data-ttu-id="aafbd-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="aafbd-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="aafbd-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="aafbd-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="aafbd-112">ProgramControl. Read. All, ProgramControl. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="aafbd-112">ProgramControl.Read.All, ProgramControl.ReadWrite.All</span></span>  |
|<span data-ttu-id="aafbd-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="aafbd-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="aafbd-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="aafbd-114">Not supported.</span></span> |
|<span data-ttu-id="aafbd-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="aafbd-115">Application</span></span>                            | <span data-ttu-id="aafbd-116">ProgramControl. Read. All, ProgramControl. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="aafbd-116">ProgramControl.Read.All, ProgramControl.ReadWrite.All</span></span>  |

 <span data-ttu-id="aafbd-117">O usuário conectado também deve estar em uma função de diretório que permite que ele leia um programa.</span><span class="sxs-lookup"><span data-stu-id="aafbd-117">The signed in user must also be in a directory role that permits them to read a program.</span></span>

## <a name="http-request"></a><span data-ttu-id="aafbd-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="aafbd-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /programs
```
## <a name="request-headers"></a><span data-ttu-id="aafbd-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="aafbd-119">Request headers</span></span>
| <span data-ttu-id="aafbd-120">Nome</span><span class="sxs-lookup"><span data-stu-id="aafbd-120">Name</span></span>         | <span data-ttu-id="aafbd-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="aafbd-121">Type</span></span>        | <span data-ttu-id="aafbd-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="aafbd-122">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="aafbd-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="aafbd-123">Authorization</span></span> | <span data-ttu-id="aafbd-124">string</span><span class="sxs-lookup"><span data-stu-id="aafbd-124">string</span></span> | <span data-ttu-id="aafbd-p102">\{token\} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="aafbd-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="aafbd-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="aafbd-127">Request body</span></span>
<span data-ttu-id="aafbd-128">Nenhum corpo de solicitação deve ser fornecido.</span><span class="sxs-lookup"><span data-stu-id="aafbd-128">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="aafbd-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="aafbd-129">Response</span></span>
<span data-ttu-id="aafbd-130">Se tiver êxito, este método retornará `200, OK` um código de resposta e uma matriz de objetos de [programa](../resources/program.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="aafbd-130">If successful, this method returns a `200, OK` response code and an array of [program](../resources/program.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="aafbd-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="aafbd-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="aafbd-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="aafbd-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="aafbd-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="aafbd-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_program"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/programs
```
# <a name="c"></a>[<span data-ttu-id="aafbd-134">C#</span><span class="sxs-lookup"><span data-stu-id="aafbd-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-program-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="aafbd-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="aafbd-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-program-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="aafbd-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="aafbd-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-program-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="aafbd-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="aafbd-137">Response</span></span>
><span data-ttu-id="aafbd-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="aafbd-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="aafbd-140">Confira também</span><span class="sxs-lookup"><span data-stu-id="aafbd-140">See also</span></span>

| <span data-ttu-id="aafbd-141">Método</span><span class="sxs-lookup"><span data-stu-id="aafbd-141">Method</span></span>           | <span data-ttu-id="aafbd-142">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="aafbd-142">Return Type</span></span>    |<span data-ttu-id="aafbd-143">Descrição</span><span class="sxs-lookup"><span data-stu-id="aafbd-143">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="aafbd-144">Listar programControls de um programa</span><span class="sxs-lookup"><span data-stu-id="aafbd-144">List programControls of a program</span></span>](program-listcontrols.md) |     <span data-ttu-id="aafbd-145">coleção [programControl](../resources/programcontrol.md)</span><span class="sxs-lookup"><span data-stu-id="aafbd-145">[programControl](../resources/programcontrol.md) collection</span></span>|    <span data-ttu-id="aafbd-146">Obter uma coleção de controles de um programa.</span><span class="sxs-lookup"><span data-stu-id="aafbd-146">Get a collection of the controls of a program.</span></span>|


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
