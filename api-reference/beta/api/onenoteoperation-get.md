---
title: Obter o onenoteOperation
description: 'Obter o status de uma operação de OneNote de longo prazo. Isso se aplica a operações que retornam o header **Operation-Location** na resposta, como `CopyNotebook` , , , `CopyToNotebook` `CopyToSectionGroup` `and CopyToSection` .   '
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
doc_type: apiPageType
ms.openlocfilehash: 5dd65d44ea9d4df3bdd494586a17b67cc1e5b82b
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52050098"
---
# <a name="get-onenoteoperation"></a><span data-ttu-id="4a869-104">Obter o onenoteOperation</span><span class="sxs-lookup"><span data-stu-id="4a869-104">Get onenoteOperation</span></span>

<span data-ttu-id="4a869-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4a869-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4a869-106">Obter o status de uma operação de OneNote de longo prazo.</span><span class="sxs-lookup"><span data-stu-id="4a869-106">Get the status of a long-running OneNote operation.</span></span> <span data-ttu-id="4a869-107">Isso se aplica a operações que retornam o header **Operation-Location** na resposta, como `CopyNotebook` , , , `CopyToNotebook` `CopyToSectionGroup` `and CopyToSection` .</span><span class="sxs-lookup"><span data-stu-id="4a869-107">This applies to operations that return the **Operation-Location** header in the response, such as `CopyNotebook`, `CopyToNotebook`, `CopyToSectionGroup`, `and CopyToSection`.</span></span>   

<span data-ttu-id="4a869-108">Você pode sondar o ponto de extremidade Operation-Location até que `status` a propriedade retorne ou `completed` `failed` .</span><span class="sxs-lookup"><span data-stu-id="4a869-108">You can poll the Operation-Location endpoint until the `status` property returns `completed` or `failed`.</span></span> 

<span data-ttu-id="4a869-109">Se o status for `completed` , `resourceLocation` a propriedade conterá o URI do ponto de extremidade do recurso.</span><span class="sxs-lookup"><span data-stu-id="4a869-109">If the status is `completed`, the `resourceLocation` property contains the resource endpoint URI.</span></span> 

<span data-ttu-id="4a869-110">Se o status for `failed` , o erro e as propriedades `@api.diagnostics` fornecerão informações de erro.</span><span class="sxs-lookup"><span data-stu-id="4a869-110">If the status is `failed`, the error and `@api.diagnostics` properties provide error information.</span></span>

## <a name="permissions"></a><span data-ttu-id="4a869-111">Permissões</span><span class="sxs-lookup"><span data-stu-id="4a869-111">Permissions</span></span>
<span data-ttu-id="4a869-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4a869-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4a869-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4a869-114">Permission type</span></span>      | <span data-ttu-id="4a869-115">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4a869-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4a869-116">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4a869-116">Delegated (work or school account)</span></span> | <span data-ttu-id="4a869-117">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4a869-117">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="4a869-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4a869-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4a869-119">Notes.Create, Notes.Read, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4a869-119">Notes.Create, Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="4a869-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4a869-120">Application</span></span> | <span data-ttu-id="4a869-121">Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4a869-121">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4a869-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4a869-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/operations/{id}
GET /users/{id | userPrincipalName}/onenote/operations/{id}
GET /groups/{id}/onenote/operations/{id}
GET /sites/{id}/onenote/operations/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="4a869-123">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="4a869-123">Optional query parameters</span></span>
<span data-ttu-id="4a869-124">Nenhum</span><span class="sxs-lookup"><span data-stu-id="4a869-124">None.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4a869-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4a869-125">Request headers</span></span>
| <span data-ttu-id="4a869-126">Nome</span><span class="sxs-lookup"><span data-stu-id="4a869-126">Name</span></span>       | <span data-ttu-id="4a869-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="4a869-127">Type</span></span> | <span data-ttu-id="4a869-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="4a869-128">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="4a869-129">Autorização</span><span class="sxs-lookup"><span data-stu-id="4a869-129">Authorization</span></span>  | <span data-ttu-id="4a869-130">string</span><span class="sxs-lookup"><span data-stu-id="4a869-130">string</span></span>  | <span data-ttu-id="4a869-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4a869-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="4a869-133">Aceitar</span><span class="sxs-lookup"><span data-stu-id="4a869-133">Accept</span></span> | <span data-ttu-id="4a869-134">string</span><span class="sxs-lookup"><span data-stu-id="4a869-134">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="4a869-135">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4a869-135">Request body</span></span>
<span data-ttu-id="4a869-136">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="4a869-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4a869-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="4a869-137">Response</span></span>

<span data-ttu-id="4a869-138">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto onenoteOperation](../resources/onenoteoperation.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4a869-138">If successful, this method returns a `200 OK` response code and [onenoteOperation](../resources/onenoteoperation.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="4a869-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4a869-139">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4a869-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4a869-140">Request</span></span>
<span data-ttu-id="4a869-141">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4a869-141">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="4a869-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="4a869-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_onenoteoperation"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/onenote/operations/{id}
```
# <a name="c"></a>[<span data-ttu-id="4a869-143">C#</span><span class="sxs-lookup"><span data-stu-id="4a869-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-onenoteoperation-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4a869-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4a869-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-onenoteoperation-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4a869-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4a869-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-onenoteoperation-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4a869-146">Java</span><span class="sxs-lookup"><span data-stu-id="4a869-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-onenoteoperation-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="4a869-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="4a869-147">Response</span></span>
<span data-ttu-id="4a869-148">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4a869-148">Here is an example of the response.</span></span> <span data-ttu-id="4a869-149">Observação: o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="4a869-149">Note: The response object shown here might be shortened for readability.</span></span>
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


