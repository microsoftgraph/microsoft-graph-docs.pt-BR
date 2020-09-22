---
title: Adicionar professor
description: Adicione um professor a uma aula.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 14fc9a60ee1275b4c92a23cd955bba912b5ace3c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48007543"
---
# <a name="add-teacher"></a><span data-ttu-id="cbaea-103">Adicionar professor</span><span class="sxs-lookup"><span data-stu-id="cbaea-103">Add teacher</span></span>

<span data-ttu-id="cbaea-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cbaea-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cbaea-105">Adicione um professor a uma aula.</span><span class="sxs-lookup"><span data-stu-id="cbaea-105">Add a teacher to a class.</span></span>

## <a name="permissions"></a><span data-ttu-id="cbaea-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="cbaea-106">Permissions</span></span>
<span data-ttu-id="cbaea-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cbaea-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cbaea-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cbaea-109">Permission type</span></span>      | <span data-ttu-id="cbaea-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="cbaea-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cbaea-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cbaea-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="cbaea-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cbaea-112">Not supported.</span></span>  |
|<span data-ttu-id="cbaea-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cbaea-113">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="cbaea-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cbaea-114">Not supported.</span></span>  |
|<span data-ttu-id="cbaea-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cbaea-115">Application</span></span> | <span data-ttu-id="cbaea-116">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cbaea-116">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="cbaea-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cbaea-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/teachers/$ref
```
## <a name="request-headers"></a><span data-ttu-id="cbaea-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cbaea-118">Request headers</span></span>
| <span data-ttu-id="cbaea-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="cbaea-119">Header</span></span>       | <span data-ttu-id="cbaea-120">Valor</span><span class="sxs-lookup"><span data-stu-id="cbaea-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="cbaea-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="cbaea-121">Authorization</span></span>  | <span data-ttu-id="cbaea-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cbaea-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="cbaea-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="cbaea-124">Content-Type</span></span>  | <span data-ttu-id="cbaea-125">application/json</span><span class="sxs-lookup"><span data-stu-id="cbaea-125">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="cbaea-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cbaea-126">Request body</span></span>
<span data-ttu-id="cbaea-127">No corpo da solicitação, forneça uma representação JSON de um objeto [educationUser](../resources/educationuser.md).</span><span class="sxs-lookup"><span data-stu-id="cbaea-127">In the request body, supply a JSON representation of an [educationUser](../resources/educationuser.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="cbaea-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="cbaea-128">Response</span></span>
<span data-ttu-id="cbaea-129">Se bem-sucedido, esse método retornará um código de resposta `204 No Content` e um objeto [educationClass](../resources/educationclass.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cbaea-129">If successful, this method returns a `204 No Content` response code and an [educationClass](../resources/educationclass.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cbaea-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="cbaea-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="cbaea-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cbaea-131">Request</span></span>
<span data-ttu-id="cbaea-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="cbaea-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="cbaea-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="cbaea-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_educationuser_from_educationclass"
}-->
```http
POST https://graph.microsoft.com/beta/education/classes/11017/teachers/$ref
Content-type: application/json
Content-length: 508

{
  "@odata.id":"https://graph.microsoft.com/beta/education/users/14011"
}
```
# <a name="javascript"></a>[<span data-ttu-id="cbaea-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cbaea-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-educationuser-from-educationclass-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cbaea-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cbaea-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-educationuser-from-educationclass-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="cbaea-136">C#</span><span class="sxs-lookup"><span data-stu-id="cbaea-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-educationuser-from-educationclass-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="cbaea-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="cbaea-137">Response</span></span>
<span data-ttu-id="cbaea-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="cbaea-138">The following is an example of the response.</span></span> 

<!-- Add the educationClass object to the response -->

><span data-ttu-id="cbaea-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="cbaea-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationUser"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create educationUser",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


