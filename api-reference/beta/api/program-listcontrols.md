---
title: Listar programControls de um programa
description: No recurso de revisões do Azure AD Access, liste todos os objetos programControl vinculados a um programa específico.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: markwahl-msft
ms.openlocfilehash: e24c41ea7e0f99af914bf396766ae2120d556eca
ms.sourcegitcommit: bd40e302ce04b686e86989246ab7c4cc9ad3f320
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/03/2020
ms.locfileid: "43123068"
---
# <a name="list-programcontrols-of-a-program"></a><span data-ttu-id="e71c8-103">Listar programControls de um programa</span><span class="sxs-lookup"><span data-stu-id="e71c8-103">List programControls of a program</span></span>

<span data-ttu-id="e71c8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e71c8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e71c8-105">No recurso de revisões do Azure AD [Access](../resources/accessreviews-root.md) , liste todos os objetos [programControl](../resources/programcontrol.md) vinculados a um programa específico.</span><span class="sxs-lookup"><span data-stu-id="e71c8-105">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, list all the [programControl](../resources/programcontrol.md) objects, linked to a particular program.</span></span>
## <a name="permissions"></a><span data-ttu-id="e71c8-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="e71c8-106">Permissions</span></span>
<span data-ttu-id="e71c8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e71c8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e71c8-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e71c8-109">Permission type</span></span>                        | <span data-ttu-id="e71c8-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e71c8-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="e71c8-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e71c8-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="e71c8-112">ProgramControl. Read. All, ProgramControl. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="e71c8-112">ProgramControl.Read.All, ProgramControl.ReadWrite.All</span></span>  |
|<span data-ttu-id="e71c8-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e71c8-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e71c8-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e71c8-114">Not supported.</span></span> |
|<span data-ttu-id="e71c8-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e71c8-115">Application</span></span>                            | <span data-ttu-id="e71c8-116">ProgramControl. Read. All, ProgramControl. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="e71c8-116">ProgramControl.Read.All, ProgramControl.ReadWrite.All</span></span>  |

 <span data-ttu-id="e71c8-117">O usuário conectado também deve estar em uma função de diretório que permite que ele leia um programa.</span><span class="sxs-lookup"><span data-stu-id="e71c8-117">The signed in user must also be in a directory role that permits them to read a program.</span></span>

## <a name="http-request"></a><span data-ttu-id="e71c8-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e71c8-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /programs('{programId}')/controls
```
## <a name="request-headers"></a><span data-ttu-id="e71c8-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e71c8-119">Request headers</span></span>
| <span data-ttu-id="e71c8-120">Nome</span><span class="sxs-lookup"><span data-stu-id="e71c8-120">Name</span></span>         | <span data-ttu-id="e71c8-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="e71c8-121">Type</span></span>        | <span data-ttu-id="e71c8-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="e71c8-122">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="e71c8-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="e71c8-123">Authorization</span></span> | <span data-ttu-id="e71c8-124">string</span><span class="sxs-lookup"><span data-stu-id="e71c8-124">string</span></span> | <span data-ttu-id="e71c8-p102">\{token\} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e71c8-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e71c8-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e71c8-127">Request body</span></span>
<span data-ttu-id="e71c8-128">Nenhum corpo de solicitação deve ser fornecido.</span><span class="sxs-lookup"><span data-stu-id="e71c8-128">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="e71c8-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="e71c8-129">Response</span></span>
<span data-ttu-id="e71c8-130">Se tiver êxito, este método retornará `200, OK` um código de resposta e uma matriz de objetos [programControl](../resources/programcontrol.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e71c8-130">If successful, this method returns a `200, OK` response code and an array of [programControl](../resources/programcontrol.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e71c8-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e71c8-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e71c8-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e71c8-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="e71c8-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="e71c8-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_programControl_from_program"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/programs/673a7379-9c38-4f01-bd9d-4fda7260b807/controls
```
# <a name="c"></a>[<span data-ttu-id="e71c8-134">C#</span><span class="sxs-lookup"><span data-stu-id="e71c8-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-programcontrol-from-program-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e71c8-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e71c8-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-programcontrol-from-program-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e71c8-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e71c8-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-programcontrol-from-program-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="e71c8-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="e71c8-137">Response</span></span>
><span data-ttu-id="e71c8-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e71c8-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.programControl",
    "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{

    "value": [
        {
            "id": "bd68f301-e44b-4ad1-ba6d-a07314ed2e79",
            "controlId": "bc81d51d-be53-4606-a8c2-f90a2beb5f40",
            "programId": "673a7379-9c38-4f01-bd9d-4fda7260b807",
            "controlTypeId": "6e4f3d20-c5c3-407f-9695-8460952bcc68",
            "displayName": "guest user review",
            "status": "Completed",
            "createdDateTime": "2017-09-20T20:18:05.1318394Z"
        }
    ]
}

```


<!--
{
  "type": "#page.annotation",
  "description": "List programControls of a program",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
