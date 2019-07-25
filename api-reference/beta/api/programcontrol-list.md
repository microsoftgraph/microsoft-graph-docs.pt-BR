---
title: Listar programControls
description: No recurso de revisões do Azure AD Access, liste todos os objetos programControl em todos os programas no locatário.
localization_priority: Normal
ms.openlocfilehash: 431adc38a6f456990d06f7df6cc343b90bee9084
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35875287"
---
# <a name="list-programcontrols"></a><span data-ttu-id="712ea-103">Listar programControls</span><span class="sxs-lookup"><span data-stu-id="712ea-103">List programControls</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="712ea-104">No recurso de revisões do Azure AD [Access](../resources/accessreviews-root.md) , liste todos os objetos [programControl](../resources/programcontrol.md) em todos os programas no locatário.</span><span class="sxs-lookup"><span data-stu-id="712ea-104">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, list all the [programControl](../resources/programcontrol.md) objects, across all programs in the tenant.</span></span>
## <a name="permissions"></a><span data-ttu-id="712ea-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="712ea-105">Permissions</span></span>
<span data-ttu-id="712ea-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="712ea-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="712ea-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="712ea-108">Permission type</span></span>                        | <span data-ttu-id="712ea-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="712ea-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="712ea-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="712ea-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="712ea-111">ProgramControl. Read. All, ProgramControl. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="712ea-111">ProgramControl.Read.All, ProgramControl.ReadWrite.All</span></span>   |
|<span data-ttu-id="712ea-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="712ea-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="712ea-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="712ea-113">Not supported.</span></span> |
|<span data-ttu-id="712ea-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="712ea-114">Application</span></span>                            | <span data-ttu-id="712ea-115">ProgramControl. Read. All, ProgramControl. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="712ea-115">ProgramControl.Read.All, ProgramControl.ReadWrite.All</span></span>  |

<span data-ttu-id="712ea-116">O usuário conectado também deve estar em uma função de diretório que permite que ele leia um programa.</span><span class="sxs-lookup"><span data-stu-id="712ea-116">The signed in user must also be in a directory role that permits them to read a program.</span></span>

## <a name="http-request"></a><span data-ttu-id="712ea-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="712ea-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /programControls
```
## <a name="request-headers"></a><span data-ttu-id="712ea-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="712ea-118">Request headers</span></span>
| <span data-ttu-id="712ea-119">Nome</span><span class="sxs-lookup"><span data-stu-id="712ea-119">Name</span></span>         | <span data-ttu-id="712ea-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="712ea-120">Type</span></span>        | <span data-ttu-id="712ea-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="712ea-121">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="712ea-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="712ea-122">Authorization</span></span> | <span data-ttu-id="712ea-123">string</span><span class="sxs-lookup"><span data-stu-id="712ea-123">string</span></span> | <span data-ttu-id="712ea-p102">\{token\} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="712ea-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="712ea-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="712ea-126">Request body</span></span>
<span data-ttu-id="712ea-127">Nenhum corpo de solicitação deve ser fornecido.</span><span class="sxs-lookup"><span data-stu-id="712ea-127">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="712ea-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="712ea-128">Response</span></span>
<span data-ttu-id="712ea-129">Se tiver êxito, este método retornará `200, OK` um código de resposta e uma matriz de objetos [programControl](../resources/programcontrol.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="712ea-129">If successful, this method returns a `200, OK` response code and an array of [programControl](../resources/programcontrol.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="712ea-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="712ea-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="712ea-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="712ea-131">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="712ea-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="712ea-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_programControl"
}-->
```http
GET https://graph.microsoft.com/beta/programControls
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="712ea-133">C#</span><span class="sxs-lookup"><span data-stu-id="712ea-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-programcontrol-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="712ea-134">Javascript</span><span class="sxs-lookup"><span data-stu-id="712ea-134">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-programcontrol-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="712ea-135">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="712ea-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-programcontrol-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="712ea-136">Java</span><span class="sxs-lookup"><span data-stu-id="712ea-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-programcontrol-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="712ea-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="712ea-137">Response</span></span>
><span data-ttu-id="712ea-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="712ea-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="712ea-140">Confira também</span><span class="sxs-lookup"><span data-stu-id="712ea-140">See also</span></span>

| <span data-ttu-id="712ea-141">Método</span><span class="sxs-lookup"><span data-stu-id="712ea-141">Method</span></span>           | <span data-ttu-id="712ea-142">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="712ea-142">Return Type</span></span>    |<span data-ttu-id="712ea-143">Descrição</span><span class="sxs-lookup"><span data-stu-id="712ea-143">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="712ea-144">Listar programControls de um programa</span><span class="sxs-lookup"><span data-stu-id="712ea-144">List programControls of a program</span></span>](program-listcontrols.md) |     <span data-ttu-id="712ea-145">coleção [programControl](../resources/programcontrol.md)</span><span class="sxs-lookup"><span data-stu-id="712ea-145">[programControl](../resources/programcontrol.md) collection</span></span>|    <span data-ttu-id="712ea-146">Obter uma coleção de controles de um programa.</span><span class="sxs-lookup"><span data-stu-id="712ea-146">Get a collection of the controls of a program.</span></span>|


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
