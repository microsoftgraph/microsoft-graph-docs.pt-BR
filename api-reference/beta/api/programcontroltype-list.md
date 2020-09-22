---
title: Listar programControlTypes
description: No recurso de revisões do Azure AD Access, liste todos os objetos programControlType.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: markwahl-msft
ms.openlocfilehash: a73f85b93c346dbf75d78593b74d08e1de35b925
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47986210"
---
# <a name="list-programcontroltypes"></a><span data-ttu-id="64f31-103">Listar programControlTypes</span><span class="sxs-lookup"><span data-stu-id="64f31-103">List programControlTypes</span></span>

<span data-ttu-id="64f31-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="64f31-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="64f31-105">No recurso de revisões do Azure AD [Access](../resources/accessreviews-root.md) , liste todos os objetos [programControlType](../resources/programcontroltype.md) .</span><span class="sxs-lookup"><span data-stu-id="64f31-105">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, list all the [programControlType](../resources/programcontroltype.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="64f31-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="64f31-106">Permissions</span></span>
<span data-ttu-id="64f31-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="64f31-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="64f31-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="64f31-109">Permission type</span></span>                        | <span data-ttu-id="64f31-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="64f31-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="64f31-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="64f31-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="64f31-112">ProgramControl. Read. All, ProgramControl. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="64f31-112">ProgramControl.Read.All, ProgramControl.ReadWrite.All</span></span>   |
|<span data-ttu-id="64f31-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="64f31-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="64f31-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="64f31-114">Not supported.</span></span> |
|<span data-ttu-id="64f31-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="64f31-115">Application</span></span>                            | <span data-ttu-id="64f31-116">ProgramControl. Read. All ', ProgramControl. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="64f31-116">ProgramControl.Read.All\`, ProgramControl.ReadWrite.All</span></span>  |

<span data-ttu-id="64f31-117">O usuário conectado também deve estar em uma função de diretório que permite que ele leia um programa.</span><span class="sxs-lookup"><span data-stu-id="64f31-117">The signed in user must also be in a directory role that permits them to read a program.</span></span>

## <a name="http-request"></a><span data-ttu-id="64f31-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="64f31-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /programControlTypes
```
## <a name="request-headers"></a><span data-ttu-id="64f31-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="64f31-119">Request headers</span></span>
| <span data-ttu-id="64f31-120">Nome</span><span class="sxs-lookup"><span data-stu-id="64f31-120">Name</span></span>         | <span data-ttu-id="64f31-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="64f31-121">Type</span></span>        | <span data-ttu-id="64f31-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="64f31-122">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="64f31-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="64f31-123">Authorization</span></span> | <span data-ttu-id="64f31-124">string</span><span class="sxs-lookup"><span data-stu-id="64f31-124">string</span></span> | <span data-ttu-id="64f31-p102">\{token\} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="64f31-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="64f31-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="64f31-127">Request body</span></span>
<span data-ttu-id="64f31-128">Nenhum corpo de solicitação deve ser fornecido.</span><span class="sxs-lookup"><span data-stu-id="64f31-128">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="64f31-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="64f31-129">Response</span></span>
<span data-ttu-id="64f31-130">Se tiver êxito, este método retornará um `200, OK` código de resposta e uma matriz de objetos [programControlType](../resources/programcontroltype.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="64f31-130">If successful, this method returns a `200, OK` response code and an array of [programControlType](../resources/programcontroltype.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="64f31-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="64f31-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="64f31-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="64f31-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="64f31-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="64f31-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_programcontroltype"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/programControlTypes
```
# <a name="c"></a>[<span data-ttu-id="64f31-134">C#</span><span class="sxs-lookup"><span data-stu-id="64f31-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-programcontroltype-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="64f31-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="64f31-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-programcontroltype-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="64f31-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="64f31-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-programcontroltype-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="64f31-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="64f31-137">Response</span></span>
><span data-ttu-id="64f31-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="64f31-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="64f31-140">Confira também</span><span class="sxs-lookup"><span data-stu-id="64f31-140">See also</span></span>

| <span data-ttu-id="64f31-141">Método</span><span class="sxs-lookup"><span data-stu-id="64f31-141">Method</span></span>           | <span data-ttu-id="64f31-142">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="64f31-142">Return Type</span></span>    |<span data-ttu-id="64f31-143">Descrição</span><span class="sxs-lookup"><span data-stu-id="64f31-143">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="64f31-144">Listar programControls de um programa</span><span class="sxs-lookup"><span data-stu-id="64f31-144">List programControls of a program</span></span>](program-listcontrols.md) |     <span data-ttu-id="64f31-145">coleção [programControl](../resources/programcontrol.md)</span><span class="sxs-lookup"><span data-stu-id="64f31-145">[programControl](../resources/programcontrol.md) collection</span></span>|    <span data-ttu-id="64f31-146">Obter uma coleção de controles de um programa.</span><span class="sxs-lookup"><span data-stu-id="64f31-146">Get a collection of the controls of a program.</span></span>|


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


