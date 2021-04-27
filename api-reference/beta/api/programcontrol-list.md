---
title: Listar programControls
description: No recurso de revisões de acesso do Azure AD, liste todos os objetos programControl, em todos os programas no locatário.
localization_priority: Normal
doc_type: apiPageType
ms.prod: governance
author: markwahl-msft
ms.openlocfilehash: a08b1c476b5e91032c0156a4d7c88d9d79849637
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52055215"
---
# <a name="list-programcontrols"></a><span data-ttu-id="df9d0-103">Listar programControls</span><span class="sxs-lookup"><span data-stu-id="df9d0-103">List programControls</span></span>

<span data-ttu-id="df9d0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="df9d0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="df9d0-105">No recurso de revisões de acesso do Azure [AD,](../resources/accessreviews-root.md) liste todos os objetos [programControl,](../resources/programcontrol.md) em todos os programas no locatário.</span><span class="sxs-lookup"><span data-stu-id="df9d0-105">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, list all the [programControl](../resources/programcontrol.md) objects, across all programs in the tenant.</span></span>
## <a name="permissions"></a><span data-ttu-id="df9d0-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="df9d0-106">Permissions</span></span>
<span data-ttu-id="df9d0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="df9d0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="df9d0-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="df9d0-109">Permission type</span></span>                        | <span data-ttu-id="df9d0-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="df9d0-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="df9d0-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="df9d0-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="df9d0-112">ProgramControl.Read.All, ProgramControl.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="df9d0-112">ProgramControl.Read.All, ProgramControl.ReadWrite.All</span></span>   |
|<span data-ttu-id="df9d0-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="df9d0-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="df9d0-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="df9d0-114">Not supported.</span></span> |
|<span data-ttu-id="df9d0-115">Application</span><span class="sxs-lookup"><span data-stu-id="df9d0-115">Application</span></span>                            | <span data-ttu-id="df9d0-116">ProgramControl.Read.All, ProgramControl.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="df9d0-116">ProgramControl.Read.All, ProgramControl.ReadWrite.All</span></span>  |

<span data-ttu-id="df9d0-117">O usuário inscreveu também deve estar em uma função de diretório que permita que ele leia um programa.</span><span class="sxs-lookup"><span data-stu-id="df9d0-117">The signed in user must also be in a directory role that permits them to read a program.</span></span>

## <a name="http-request"></a><span data-ttu-id="df9d0-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="df9d0-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /programControls
```
## <a name="request-headers"></a><span data-ttu-id="df9d0-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="df9d0-119">Request headers</span></span>
| <span data-ttu-id="df9d0-120">Nome</span><span class="sxs-lookup"><span data-stu-id="df9d0-120">Name</span></span>         | <span data-ttu-id="df9d0-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="df9d0-121">Type</span></span>        | <span data-ttu-id="df9d0-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="df9d0-122">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="df9d0-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="df9d0-123">Authorization</span></span> | <span data-ttu-id="df9d0-124">string</span><span class="sxs-lookup"><span data-stu-id="df9d0-124">string</span></span> | <span data-ttu-id="df9d0-p102">\{token\} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="df9d0-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="df9d0-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="df9d0-127">Request body</span></span>
<span data-ttu-id="df9d0-128">Nenhum corpo de solicitação deve ser fornecido.</span><span class="sxs-lookup"><span data-stu-id="df9d0-128">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="df9d0-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="df9d0-129">Response</span></span>
<span data-ttu-id="df9d0-130">Se tiver êxito, este método retornará um código de resposta e uma `200, OK` matriz de [objetos programControl](../resources/programcontrol.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="df9d0-130">If successful, this method returns a `200, OK` response code and an array of [programControl](../resources/programcontrol.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="df9d0-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="df9d0-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="df9d0-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="df9d0-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="df9d0-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="df9d0-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_programControl"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/programControls
```
# <a name="c"></a>[<span data-ttu-id="df9d0-134">C#</span><span class="sxs-lookup"><span data-stu-id="df9d0-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-programcontrol-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="df9d0-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="df9d0-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-programcontrol-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="df9d0-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="df9d0-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-programcontrol-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="df9d0-137">Java</span><span class="sxs-lookup"><span data-stu-id="df9d0-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-programcontrol-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="df9d0-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="df9d0-138">Response</span></span>
><span data-ttu-id="df9d0-139">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="df9d0-139">**Note:** The response object shown here might be shortened for readability.</span></span>
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
            "id": "f6abf8ef-a05e-4788-adc9-5af909c400af",
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

## <a name="see-also"></a><span data-ttu-id="df9d0-140">Confira também</span><span class="sxs-lookup"><span data-stu-id="df9d0-140">See also</span></span>

| <span data-ttu-id="df9d0-141">Método</span><span class="sxs-lookup"><span data-stu-id="df9d0-141">Method</span></span>           | <span data-ttu-id="df9d0-142">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="df9d0-142">Return Type</span></span>    |<span data-ttu-id="df9d0-143">Descrição</span><span class="sxs-lookup"><span data-stu-id="df9d0-143">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="df9d0-144">Listar programControls de um programa</span><span class="sxs-lookup"><span data-stu-id="df9d0-144">List programControls of a program</span></span>](program-listcontrols.md) |     <span data-ttu-id="df9d0-145">[Coleção programControl](../resources/programcontrol.md)</span><span class="sxs-lookup"><span data-stu-id="df9d0-145">[programControl](../resources/programcontrol.md) collection</span></span>|    <span data-ttu-id="df9d0-146">Obter uma coleção dos controles de um programa.</span><span class="sxs-lookup"><span data-stu-id="df9d0-146">Get a collection of the controls of a program.</span></span>|


<!--
{
  "type": "#page.annotation",
  "description": "List programControls",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


