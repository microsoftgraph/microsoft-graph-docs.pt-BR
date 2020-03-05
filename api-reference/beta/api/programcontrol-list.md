---
title: Listar programControls
description: No recurso de revisões do Azure AD Access, liste todos os objetos programControl em todos os programas no locatário.
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: e486e99fb3607d7cd093a269331ec75f5146d583
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42454952"
---
# <a name="list-programcontrols"></a><span data-ttu-id="3153a-103">Listar programControls</span><span class="sxs-lookup"><span data-stu-id="3153a-103">List programControls</span></span>

<span data-ttu-id="3153a-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="3153a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3153a-105">No recurso de revisões do Azure AD [Access](../resources/accessreviews-root.md) , liste todos os objetos [programControl](../resources/programcontrol.md) em todos os programas no locatário.</span><span class="sxs-lookup"><span data-stu-id="3153a-105">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, list all the [programControl](../resources/programcontrol.md) objects, across all programs in the tenant.</span></span>
## <a name="permissions"></a><span data-ttu-id="3153a-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="3153a-106">Permissions</span></span>
<span data-ttu-id="3153a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3153a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3153a-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3153a-109">Permission type</span></span>                        | <span data-ttu-id="3153a-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3153a-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="3153a-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3153a-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="3153a-112">ProgramControl. Read. All, ProgramControl. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="3153a-112">ProgramControl.Read.All, ProgramControl.ReadWrite.All</span></span>   |
|<span data-ttu-id="3153a-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3153a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3153a-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3153a-114">Not supported.</span></span> |
|<span data-ttu-id="3153a-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3153a-115">Application</span></span>                            | <span data-ttu-id="3153a-116">ProgramControl. Read. All, ProgramControl. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="3153a-116">ProgramControl.Read.All, ProgramControl.ReadWrite.All</span></span>  |

<span data-ttu-id="3153a-117">O usuário conectado também deve estar em uma função de diretório que permite que ele leia um programa.</span><span class="sxs-lookup"><span data-stu-id="3153a-117">The signed in user must also be in a directory role that permits them to read a program.</span></span>

## <a name="http-request"></a><span data-ttu-id="3153a-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3153a-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /programControls
```
## <a name="request-headers"></a><span data-ttu-id="3153a-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3153a-119">Request headers</span></span>
| <span data-ttu-id="3153a-120">Nome</span><span class="sxs-lookup"><span data-stu-id="3153a-120">Name</span></span>         | <span data-ttu-id="3153a-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="3153a-121">Type</span></span>        | <span data-ttu-id="3153a-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="3153a-122">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="3153a-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="3153a-123">Authorization</span></span> | <span data-ttu-id="3153a-124">string</span><span class="sxs-lookup"><span data-stu-id="3153a-124">string</span></span> | <span data-ttu-id="3153a-p102">\{token\} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3153a-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3153a-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3153a-127">Request body</span></span>
<span data-ttu-id="3153a-128">Nenhum corpo de solicitação deve ser fornecido.</span><span class="sxs-lookup"><span data-stu-id="3153a-128">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="3153a-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="3153a-129">Response</span></span>
<span data-ttu-id="3153a-130">Se tiver êxito, este método retornará `200, OK` um código de resposta e uma matriz de objetos [programControl](../resources/programcontrol.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3153a-130">If successful, this method returns a `200, OK` response code and an array of [programControl](../resources/programcontrol.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3153a-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3153a-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3153a-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3153a-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="3153a-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="3153a-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_programControl"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/programControls
```
# <a name="c"></a>[<span data-ttu-id="3153a-134">C#</span><span class="sxs-lookup"><span data-stu-id="3153a-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-programcontrol-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3153a-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3153a-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-programcontrol-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3153a-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3153a-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-programcontrol-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="3153a-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="3153a-137">Response</span></span>
><span data-ttu-id="3153a-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3153a-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="3153a-140">Confira também</span><span class="sxs-lookup"><span data-stu-id="3153a-140">See also</span></span>

| <span data-ttu-id="3153a-141">Método</span><span class="sxs-lookup"><span data-stu-id="3153a-141">Method</span></span>           | <span data-ttu-id="3153a-142">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="3153a-142">Return Type</span></span>    |<span data-ttu-id="3153a-143">Descrição</span><span class="sxs-lookup"><span data-stu-id="3153a-143">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="3153a-144">Listar programControls de um programa</span><span class="sxs-lookup"><span data-stu-id="3153a-144">List programControls of a program</span></span>](program-listcontrols.md) |     <span data-ttu-id="3153a-145">coleção [programControl](../resources/programcontrol.md)</span><span class="sxs-lookup"><span data-stu-id="3153a-145">[programControl](../resources/programcontrol.md) collection</span></span>|    <span data-ttu-id="3153a-146">Obter uma coleção de controles de um programa.</span><span class="sxs-lookup"><span data-stu-id="3153a-146">Get a collection of the controls of a program.</span></span>|


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
