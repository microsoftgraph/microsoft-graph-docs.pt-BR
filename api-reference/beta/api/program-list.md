---
title: Listar programas
description: No recurso de revisões do Azure AD Access, liste todos os objetos de programa.
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: 9998fbc123d38e478a00d64d8e78f0f734914632
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42454987"
---
# <a name="list-programs"></a><span data-ttu-id="769f0-103">Listar programas</span><span class="sxs-lookup"><span data-stu-id="769f0-103">List programs</span></span>

<span data-ttu-id="769f0-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="769f0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="769f0-105">No recurso de revisões do Azure AD [Access](../resources/accessreviews-root.md) , liste todos os objetos de [programa](../resources/program.md) .</span><span class="sxs-lookup"><span data-stu-id="769f0-105">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, list all the [program](../resources/program.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="769f0-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="769f0-106">Permissions</span></span>
<span data-ttu-id="769f0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="769f0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="769f0-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="769f0-109">Permission type</span></span>                        | <span data-ttu-id="769f0-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="769f0-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="769f0-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="769f0-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="769f0-112">ProgramControl. Read. All, ProgramControl. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="769f0-112">ProgramControl.Read.All, ProgramControl.ReadWrite.All</span></span>  |
|<span data-ttu-id="769f0-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="769f0-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="769f0-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="769f0-114">Not supported.</span></span> |
|<span data-ttu-id="769f0-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="769f0-115">Application</span></span>                            | <span data-ttu-id="769f0-116">ProgramControl. Read. All, ProgramControl. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="769f0-116">ProgramControl.Read.All, ProgramControl.ReadWrite.All</span></span>  |

 <span data-ttu-id="769f0-117">O usuário conectado também deve estar em uma função de diretório que permite que ele leia um programa.</span><span class="sxs-lookup"><span data-stu-id="769f0-117">The signed in user must also be in a directory role that permits them to read a program.</span></span>

## <a name="http-request"></a><span data-ttu-id="769f0-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="769f0-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /programs
```
## <a name="request-headers"></a><span data-ttu-id="769f0-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="769f0-119">Request headers</span></span>
| <span data-ttu-id="769f0-120">Nome</span><span class="sxs-lookup"><span data-stu-id="769f0-120">Name</span></span>         | <span data-ttu-id="769f0-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="769f0-121">Type</span></span>        | <span data-ttu-id="769f0-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="769f0-122">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="769f0-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="769f0-123">Authorization</span></span> | <span data-ttu-id="769f0-124">string</span><span class="sxs-lookup"><span data-stu-id="769f0-124">string</span></span> | <span data-ttu-id="769f0-p102">\{token\} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="769f0-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="769f0-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="769f0-127">Request body</span></span>
<span data-ttu-id="769f0-128">Nenhum corpo de solicitação deve ser fornecido.</span><span class="sxs-lookup"><span data-stu-id="769f0-128">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="769f0-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="769f0-129">Response</span></span>
<span data-ttu-id="769f0-130">Se tiver êxito, este método retornará `200, OK` um código de resposta e uma matriz de objetos de [programa](../resources/program.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="769f0-130">If successful, this method returns a `200, OK` response code and an array of [program](../resources/program.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="769f0-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="769f0-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="769f0-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="769f0-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="769f0-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="769f0-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_program"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/programs
```
# <a name="c"></a>[<span data-ttu-id="769f0-134">C#</span><span class="sxs-lookup"><span data-stu-id="769f0-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-program-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="769f0-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="769f0-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-program-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="769f0-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="769f0-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-program-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="769f0-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="769f0-137">Response</span></span>
><span data-ttu-id="769f0-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="769f0-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="769f0-140">Confira também</span><span class="sxs-lookup"><span data-stu-id="769f0-140">See also</span></span>

| <span data-ttu-id="769f0-141">Método</span><span class="sxs-lookup"><span data-stu-id="769f0-141">Method</span></span>           | <span data-ttu-id="769f0-142">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="769f0-142">Return Type</span></span>    |<span data-ttu-id="769f0-143">Descrição</span><span class="sxs-lookup"><span data-stu-id="769f0-143">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="769f0-144">Listar programControls de um programa</span><span class="sxs-lookup"><span data-stu-id="769f0-144">List programControls of a program</span></span>](program-listcontrols.md) |     <span data-ttu-id="769f0-145">coleção [programControl](../resources/programcontrol.md)</span><span class="sxs-lookup"><span data-stu-id="769f0-145">[programControl](../resources/programcontrol.md) collection</span></span>|    <span data-ttu-id="769f0-146">Obter uma coleção de controles de um programa.</span><span class="sxs-lookup"><span data-stu-id="769f0-146">Get a collection of the controls of a program.</span></span>|


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
