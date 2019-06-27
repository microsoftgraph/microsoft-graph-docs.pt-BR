---
title: Listar programControlTypes
description: No recurso de revisões do Azure AD Access, liste todos os objetos programControlType.
localization_priority: Normal
ms.openlocfilehash: 2a2767a0dc55e5d2d046e897ec0ac6cde10af945
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35264075"
---
# <a name="list-programcontroltypes"></a><span data-ttu-id="f4391-103">Listar programControlTypes</span><span class="sxs-lookup"><span data-stu-id="f4391-103">List programControlTypes</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f4391-104">No recurso de revisões do Azure AD [Access](../resources/accessreviews-root.md) , liste todos os objetos [programControlType](../resources/programcontroltype.md) .</span><span class="sxs-lookup"><span data-stu-id="f4391-104">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, list all the [programControlType](../resources/programcontroltype.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="f4391-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="f4391-105">Permissions</span></span>
<span data-ttu-id="f4391-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f4391-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f4391-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f4391-108">Permission type</span></span>                        | <span data-ttu-id="f4391-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f4391-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="f4391-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f4391-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="f4391-111">ProgramControl. Read. All, ProgramControl. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="f4391-111">ProgramControl.Read.All, ProgramControl.ReadWrite.All</span></span>   |
|<span data-ttu-id="f4391-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f4391-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f4391-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f4391-113">Not supported.</span></span> |
|<span data-ttu-id="f4391-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f4391-114">Application</span></span>                            | <span data-ttu-id="f4391-115">ProgramControl. Read. All ', ProgramControl. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="f4391-115">ProgramControl.Read.All\`, ProgramControl.ReadWrite.All</span></span>  |

<span data-ttu-id="f4391-116">O usuário conectado também deve estar em uma função de diretório que permite que ele leia um programa.</span><span class="sxs-lookup"><span data-stu-id="f4391-116">The signed in user must also be in a directory role that permits them to read a program.</span></span>

## <a name="http-request"></a><span data-ttu-id="f4391-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f4391-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /programControlTypes
```
## <a name="request-headers"></a><span data-ttu-id="f4391-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f4391-118">Request headers</span></span>
| <span data-ttu-id="f4391-119">Nome</span><span class="sxs-lookup"><span data-stu-id="f4391-119">Name</span></span>         | <span data-ttu-id="f4391-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="f4391-120">Type</span></span>        | <span data-ttu-id="f4391-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="f4391-121">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="f4391-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="f4391-122">Authorization</span></span> | <span data-ttu-id="f4391-123">string</span><span class="sxs-lookup"><span data-stu-id="f4391-123">string</span></span> | <span data-ttu-id="f4391-p102">\{token\} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f4391-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f4391-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f4391-126">Request body</span></span>
<span data-ttu-id="f4391-127">Nenhum corpo de solicitação deve ser fornecido.</span><span class="sxs-lookup"><span data-stu-id="f4391-127">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="f4391-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="f4391-128">Response</span></span>
<span data-ttu-id="f4391-129">Se tiver êxito, este método retornará `200, OK` um código de resposta e uma matriz de objetos [programControlType](../resources/programcontroltype.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f4391-129">If successful, this method returns a `200, OK` response code and an array of [programControlType](../resources/programcontroltype.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f4391-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f4391-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f4391-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f4391-131">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_programcontroltype"
}-->
```http
GET https://graph.microsoft.com/beta/programControlTypes
```

##### <a name="response"></a><span data-ttu-id="f4391-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="f4391-132">Response</span></span>
><span data-ttu-id="f4391-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f4391-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="f4391-135">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="f4391-135">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="f4391-136">C#</span><span class="sxs-lookup"><span data-stu-id="f4391-136">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_programcontroltype-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f4391-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="f4391-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_programcontroltype-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="f4391-138">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="f4391-138">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_programcontroltype-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="see-also"></a><span data-ttu-id="f4391-139">Confira também</span><span class="sxs-lookup"><span data-stu-id="f4391-139">See also</span></span>

| <span data-ttu-id="f4391-140">Método</span><span class="sxs-lookup"><span data-stu-id="f4391-140">Method</span></span>           | <span data-ttu-id="f4391-141">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="f4391-141">Return Type</span></span>    |<span data-ttu-id="f4391-142">Descrição</span><span class="sxs-lookup"><span data-stu-id="f4391-142">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="f4391-143">Listar programControls de um programa</span><span class="sxs-lookup"><span data-stu-id="f4391-143">List programControls of a program</span></span>](program-listcontrols.md) |     <span data-ttu-id="f4391-144">coleção [programControl](../resources/programcontrol.md)</span><span class="sxs-lookup"><span data-stu-id="f4391-144">[programControl](../resources/programcontrol.md) collection</span></span>|    <span data-ttu-id="f4391-145">Obter uma coleção de controles de um programa.</span><span class="sxs-lookup"><span data-stu-id="f4391-145">Get a collection of the controls of a program.</span></span>|


<!--
{
  "type": "#page.annotation",
  "description": "List program control types",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/programcontroltype-list.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/programcontroltype-list.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/programcontroltype-list.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
