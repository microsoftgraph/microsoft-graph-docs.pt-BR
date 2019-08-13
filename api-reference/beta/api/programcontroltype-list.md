---
title: Listar programControlTypes
description: No recurso de revisões do Azure AD Access, liste todos os objetos programControlType.
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: 9ab4525e3b52ef8438d77434ca9cd799f36bb160
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36342233"
---
# <a name="list-programcontroltypes"></a><span data-ttu-id="6da8a-103">Listar programControlTypes</span><span class="sxs-lookup"><span data-stu-id="6da8a-103">List programControlTypes</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6da8a-104">No recurso de revisões do Azure AD [Access](../resources/accessreviews-root.md) , liste todos os objetos [programControlType](../resources/programcontroltype.md) .</span><span class="sxs-lookup"><span data-stu-id="6da8a-104">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, list all the [programControlType](../resources/programcontroltype.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="6da8a-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="6da8a-105">Permissions</span></span>
<span data-ttu-id="6da8a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6da8a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6da8a-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6da8a-108">Permission type</span></span>                        | <span data-ttu-id="6da8a-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6da8a-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="6da8a-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6da8a-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="6da8a-111">ProgramControl. Read. All, ProgramControl. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="6da8a-111">ProgramControl.Read.All, ProgramControl.ReadWrite.All</span></span>   |
|<span data-ttu-id="6da8a-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6da8a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6da8a-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6da8a-113">Not supported.</span></span> |
|<span data-ttu-id="6da8a-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6da8a-114">Application</span></span>                            | <span data-ttu-id="6da8a-115">ProgramControl. Read. All ', ProgramControl. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="6da8a-115">ProgramControl.Read.All\`, ProgramControl.ReadWrite.All</span></span>  |

<span data-ttu-id="6da8a-116">O usuário conectado também deve estar em uma função de diretório que permite que ele leia um programa.</span><span class="sxs-lookup"><span data-stu-id="6da8a-116">The signed in user must also be in a directory role that permits them to read a program.</span></span>

## <a name="http-request"></a><span data-ttu-id="6da8a-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6da8a-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /programControlTypes
```
## <a name="request-headers"></a><span data-ttu-id="6da8a-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6da8a-118">Request headers</span></span>
| <span data-ttu-id="6da8a-119">Nome</span><span class="sxs-lookup"><span data-stu-id="6da8a-119">Name</span></span>         | <span data-ttu-id="6da8a-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="6da8a-120">Type</span></span>        | <span data-ttu-id="6da8a-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="6da8a-121">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="6da8a-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="6da8a-122">Authorization</span></span> | <span data-ttu-id="6da8a-123">string</span><span class="sxs-lookup"><span data-stu-id="6da8a-123">string</span></span> | <span data-ttu-id="6da8a-p102">\{token\} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6da8a-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6da8a-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6da8a-126">Request body</span></span>
<span data-ttu-id="6da8a-127">Nenhum corpo de solicitação deve ser fornecido.</span><span class="sxs-lookup"><span data-stu-id="6da8a-127">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="6da8a-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="6da8a-128">Response</span></span>
<span data-ttu-id="6da8a-129">Se tiver êxito, este método retornará `200, OK` um código de resposta e uma matriz de objetos [programControlType](../resources/programcontroltype.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6da8a-129">If successful, this method returns a `200, OK` response code and an array of [programControlType](../resources/programcontroltype.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6da8a-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6da8a-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6da8a-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6da8a-131">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="6da8a-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="6da8a-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_programcontroltype"
}-->
```http
GET https://graph.microsoft.com/beta/programControlTypes
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="6da8a-133">C#</span><span class="sxs-lookup"><span data-stu-id="6da8a-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-programcontroltype-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6da8a-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6da8a-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-programcontroltype-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="6da8a-135">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="6da8a-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-programcontroltype-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="6da8a-136">Java</span><span class="sxs-lookup"><span data-stu-id="6da8a-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-programcontroltype-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="6da8a-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="6da8a-137">Response</span></span>
><span data-ttu-id="6da8a-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6da8a-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
            "displayName": "Access Reviews for Office 365 Groups' membership"
        }
    ]
}

```

## <a name="see-also"></a><span data-ttu-id="6da8a-140">Confira também</span><span class="sxs-lookup"><span data-stu-id="6da8a-140">See also</span></span>

| <span data-ttu-id="6da8a-141">Método</span><span class="sxs-lookup"><span data-stu-id="6da8a-141">Method</span></span>           | <span data-ttu-id="6da8a-142">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="6da8a-142">Return Type</span></span>    |<span data-ttu-id="6da8a-143">Descrição</span><span class="sxs-lookup"><span data-stu-id="6da8a-143">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="6da8a-144">Listar programControls de um programa</span><span class="sxs-lookup"><span data-stu-id="6da8a-144">List programControls of a program</span></span>](program-listcontrols.md) |     <span data-ttu-id="6da8a-145">coleção [programControl](../resources/programcontrol.md)</span><span class="sxs-lookup"><span data-stu-id="6da8a-145">[programControl](../resources/programcontrol.md) collection</span></span>|    <span data-ttu-id="6da8a-146">Obter uma coleção de controles de um programa.</span><span class="sxs-lookup"><span data-stu-id="6da8a-146">Get a collection of the controls of a program.</span></span>|


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
