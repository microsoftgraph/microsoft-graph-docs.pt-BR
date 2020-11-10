---
title: Obter workbookApplication
description: Recupere as propriedades e os relacionamentos do objeto workbookApplication.
localization_priority: Normal
author: lumine2008
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: d8b660e2e12ea7c209a3e38d9f56bc5f89234de4
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48977518"
---
# <a name="get-workbookapplication"></a><span data-ttu-id="b8998-103">Obter workbookApplication</span><span class="sxs-lookup"><span data-stu-id="b8998-103">Get workbookApplication</span></span>

<span data-ttu-id="b8998-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b8998-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b8998-105">Recupere as propriedades e os relacionamentos de um objeto [workbookApplication](../resources/workbookapplication.md) .</span><span class="sxs-lookup"><span data-stu-id="b8998-105">Retrieve the properties and relationships of a [workbookApplication](../resources/workbookapplication.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="b8998-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="b8998-106">Permissions</span></span>
<span data-ttu-id="b8998-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b8998-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b8998-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b8998-109">Permission type</span></span>      | <span data-ttu-id="b8998-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b8998-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b8998-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b8998-111">Delegated (work or school account)</span></span> | <span data-ttu-id="b8998-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b8998-112">Files.ReadWrite</span></span>     |
|<span data-ttu-id="b8998-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b8998-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b8998-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b8998-114">Not supported.</span></span>    |
|<span data-ttu-id="b8998-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b8998-115">Application</span></span> | <span data-ttu-id="b8998-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b8998-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b8998-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b8998-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/application
```
## <a name="optional-query-parameters"></a><span data-ttu-id="b8998-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="b8998-118">Optional query parameters</span></span>
<span data-ttu-id="b8998-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="b8998-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b8998-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b8998-120">Request headers</span></span>
| <span data-ttu-id="b8998-121">Nome</span><span class="sxs-lookup"><span data-stu-id="b8998-121">Name</span></span>      |<span data-ttu-id="b8998-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="b8998-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="b8998-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="b8998-123">Authorization</span></span>  | <span data-ttu-id="b8998-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b8998-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b8998-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b8998-126">Request body</span></span>
<span data-ttu-id="b8998-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b8998-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b8998-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="b8998-128">Response</span></span>

<span data-ttu-id="b8998-129">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [workbookApplication](../resources/workbookapplication.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b8998-129">If successful, this method returns a `200 OK` response code and a [workbookApplication](../resources/workbookapplication.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b8998-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b8998-130">Example</span></span>
### <a name="request"></a><span data-ttu-id="b8998-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b8998-131">Request</span></span>
<span data-ttu-id="b8998-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b8998-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b8998-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="b8998-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_workbookApplication"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/application
```
# <a name="c"></a>[<span data-ttu-id="b8998-134">C#</span><span class="sxs-lookup"><span data-stu-id="b8998-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-workbookapplication-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b8998-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b8998-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-workbookapplication-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b8998-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b8998-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-workbookapplication-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b8998-137">Java</span><span class="sxs-lookup"><span data-stu-id="b8998-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-workbookapplication-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="b8998-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="b8998-138">Response</span></span>
<span data-ttu-id="b8998-139">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b8998-139">Here is an example of the response.</span></span> 

><span data-ttu-id="b8998-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b8998-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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


