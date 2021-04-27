---
title: Obter workbookApplication
description: Recupere as propriedades e as relações do objeto workbookApplication.
localization_priority: Normal
author: lumine2008
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 9832431657097efc28b77a72a23de23feeb40e5a
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52049573"
---
# <a name="get-workbookapplication"></a><span data-ttu-id="1c381-103">Obter workbookApplication</span><span class="sxs-lookup"><span data-stu-id="1c381-103">Get workbookApplication</span></span>

<span data-ttu-id="1c381-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1c381-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1c381-105">Recupere as propriedades e as relações de um [objeto workbookApplication.](../resources/workbookapplication.md)</span><span class="sxs-lookup"><span data-stu-id="1c381-105">Retrieve the properties and relationships of a [workbookApplication](../resources/workbookapplication.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="1c381-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="1c381-106">Permissions</span></span>
<span data-ttu-id="1c381-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1c381-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1c381-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1c381-109">Permission type</span></span>      | <span data-ttu-id="1c381-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1c381-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1c381-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1c381-111">Delegated (work or school account)</span></span> | <span data-ttu-id="1c381-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1c381-112">Files.ReadWrite</span></span>     |
|<span data-ttu-id="1c381-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1c381-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1c381-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1c381-114">Not supported.</span></span>    |
|<span data-ttu-id="1c381-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1c381-115">Application</span></span> | <span data-ttu-id="1c381-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1c381-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1c381-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1c381-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/items/{id}/workbook/application
GET /me/drive/root:/{item-path}:/workbook/application
```
## <a name="optional-query-parameters"></a><span data-ttu-id="1c381-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="1c381-118">Optional query parameters</span></span>
<span data-ttu-id="1c381-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="1c381-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1c381-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1c381-120">Request headers</span></span>
| <span data-ttu-id="1c381-121">Nome</span><span class="sxs-lookup"><span data-stu-id="1c381-121">Name</span></span>      |<span data-ttu-id="1c381-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="1c381-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="1c381-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="1c381-123">Authorization</span></span>  | <span data-ttu-id="1c381-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1c381-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1c381-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1c381-126">Request body</span></span>
<span data-ttu-id="1c381-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1c381-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1c381-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="1c381-128">Response</span></span>

<span data-ttu-id="1c381-129">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto workbookApplication](../resources/workbookapplication.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1c381-129">If successful, this method returns a `200 OK` response code and a [workbookApplication](../resources/workbookapplication.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="1c381-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1c381-130">Example</span></span>
### <a name="request"></a><span data-ttu-id="1c381-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1c381-131">Request</span></span>
<span data-ttu-id="1c381-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1c381-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="1c381-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="1c381-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_workbookApplication"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/application
```
# <a name="c"></a>[<span data-ttu-id="1c381-134">C#</span><span class="sxs-lookup"><span data-stu-id="1c381-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-workbookapplication-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1c381-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1c381-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-workbookapplication-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1c381-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1c381-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-workbookapplication-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1c381-137">Java</span><span class="sxs-lookup"><span data-stu-id="1c381-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-workbookapplication-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="1c381-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="1c381-138">Response</span></span>
<span data-ttu-id="1c381-139">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1c381-139">Here is an example of the response.</span></span> 

><span data-ttu-id="1c381-140">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="1c381-140">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookApplication"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 48

{
  "calculationMode": "calculationMode-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get workbookApplication",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


