---
title: Obter onenoteOperation
description: 'Obter o status de uma operação de execução longa do OneNote. Isso se aplica às operações que retornam o cabeçalho **Operation-Location** na resposta, como `CopyNotebook`, `CopyToNotebook` `CopyToSectionGroup`,, `and CopyToSection`.   '
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
doc_type: apiPageType
ms.openlocfilehash: 097e089a4703a8ff1ac6e34ff5fa282f79ebf00d
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/15/2019
ms.locfileid: "36414589"
---
# <a name="get-onenoteoperation"></a><span data-ttu-id="0c0a4-104">Obter onenoteOperation</span><span class="sxs-lookup"><span data-stu-id="0c0a4-104">Get onenoteOperation</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0c0a4-105">Obter o status de uma operação de execução longa do OneNote.</span><span class="sxs-lookup"><span data-stu-id="0c0a4-105">Get the status of a long-running OneNote operation.</span></span> <span data-ttu-id="0c0a4-106">Isso se aplica às operações que retornam o cabeçalho **Operation-Location** na resposta, como `CopyNotebook`, `CopyToNotebook` `CopyToSectionGroup`,, `and CopyToSection`.</span><span class="sxs-lookup"><span data-stu-id="0c0a4-106">This applies to operations that return the **Operation-Location** header in the response, such as `CopyNotebook`, `CopyToNotebook`, `CopyToSectionGroup`, `and CopyToSection`.</span></span>   

<span data-ttu-id="0c0a4-107">Você pode sondar o ponto de extremidade da operação `status` -local `completed` até `failed`que a propriedade retorne ou.</span><span class="sxs-lookup"><span data-stu-id="0c0a4-107">You can poll the Operation-Location endpoint until the `status` property returns `completed` or `failed`.</span></span> 

<span data-ttu-id="0c0a4-108">Se o status for `completed`, a `resourceLocation` Propriedade conterá o URI do ponto de extremidade do recurso.</span><span class="sxs-lookup"><span data-stu-id="0c0a4-108">If the status is `completed`, the `resourceLocation` property contains the resource endpoint URI.</span></span> 

<span data-ttu-id="0c0a4-109">Se o status for `failed`, o erro e `@api.diagnostics` as propriedades fornecerão informações de erro.</span><span class="sxs-lookup"><span data-stu-id="0c0a4-109">If the status is `failed`, the error and `@api.diagnostics` properties provide error information.</span></span>

## <a name="permissions"></a><span data-ttu-id="0c0a4-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="0c0a4-110">Permissions</span></span>
<span data-ttu-id="0c0a4-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0c0a4-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0c0a4-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0c0a4-113">Permission type</span></span>      | <span data-ttu-id="0c0a4-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0c0a4-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0c0a4-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0c0a4-115">Delegated (work or school account)</span></span> | <span data-ttu-id="0c0a4-116">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0c0a4-116">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="0c0a4-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0c0a4-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0c0a4-118">Notes.Create, Notes.Read, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0c0a4-118">Notes.Create, Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="0c0a4-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0c0a4-119">Application</span></span> | <span data-ttu-id="0c0a4-120">Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0c0a4-120">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0c0a4-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0c0a4-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/operations/{id}
GET /users/{id | userPrincipalName}/onenote/operations/{id}
GET /groups/{id}/onenote/operations/{id}
GET /sites/{id}/onenote/operations/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="0c0a4-122">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="0c0a4-122">Optional query parameters</span></span>
<span data-ttu-id="0c0a4-123">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="0c0a4-123">None.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0c0a4-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0c0a4-124">Request headers</span></span>
| <span data-ttu-id="0c0a4-125">Nome</span><span class="sxs-lookup"><span data-stu-id="0c0a4-125">Name</span></span>       | <span data-ttu-id="0c0a4-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="0c0a4-126">Type</span></span> | <span data-ttu-id="0c0a4-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="0c0a4-127">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="0c0a4-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="0c0a4-128">Authorization</span></span>  | <span data-ttu-id="0c0a4-129">string</span><span class="sxs-lookup"><span data-stu-id="0c0a4-129">string</span></span>  | <span data-ttu-id="0c0a4-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0c0a4-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="0c0a4-132">Aceitar</span><span class="sxs-lookup"><span data-stu-id="0c0a4-132">Accept</span></span> | <span data-ttu-id="0c0a4-133">string</span><span class="sxs-lookup"><span data-stu-id="0c0a4-133">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="0c0a4-134">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0c0a4-134">Request body</span></span>
<span data-ttu-id="0c0a4-135">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="0c0a4-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0c0a4-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="0c0a4-136">Response</span></span>

<span data-ttu-id="0c0a4-137">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [onenoteOperation](../resources/onenoteoperation.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0c0a4-137">If successful, this method returns a `200 OK` response code and [onenoteOperation](../resources/onenoteoperation.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="0c0a4-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0c0a4-138">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0c0a4-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0c0a4-139">Request</span></span>
<span data-ttu-id="0c0a4-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0c0a4-140">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="0c0a4-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="0c0a4-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_onenoteoperation"
}-->
```http
GET https://graph.microsoft.com/beta/me/onenote/operations/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="0c0a4-142">C#</span><span class="sxs-lookup"><span data-stu-id="0c0a4-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-onenoteoperation-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0c0a4-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0c0a4-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-onenoteoperation-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="0c0a4-144">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="0c0a4-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-onenoteoperation-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="0c0a4-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="0c0a4-145">Response</span></span>
<span data-ttu-id="0c0a4-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0c0a4-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onenoteOperation"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 215

{
  "id": "id-value",
  "status": "status-value",
  "createdDateTime": "2016-10-19T10:37:00Z",
  "lastActionDateTime": "2016-10-19T10:37:00Z",
  "resourceLocation": "resourceLocation-value",
  "resourceId": "resourceId-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get onenoteOperation",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
