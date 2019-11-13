---
title: Obter workbookApplication
description: Recupere as propriedades e os relacionamentos de um objeto workbookApplication.
localization_priority: Normal
author: grangeryy
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 06d144097eb7689b75f6ae0e7be941e254cc9592
ms.sourcegitcommit: fa08172601324fc01b090f8135fba4600bd1a9f8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/13/2019
ms.locfileid: "38302308"
---
# <a name="get-workbookapplication"></a><span data-ttu-id="f5e8d-103">Obter workbookApplication</span><span class="sxs-lookup"><span data-stu-id="f5e8d-103">Get workbookApplication</span></span>

<span data-ttu-id="f5e8d-104">Recupere as propriedades e os relacionamentos de um objeto [workbookApplication](../resources/workbookapplication.md) .</span><span class="sxs-lookup"><span data-stu-id="f5e8d-104">Retrieve the properties and relationships of a [workbookApplication](../resources/workbookapplication.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="f5e8d-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="f5e8d-105">Permissions</span></span>
<span data-ttu-id="f5e8d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f5e8d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f5e8d-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f5e8d-108">Permission type</span></span>      | <span data-ttu-id="f5e8d-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f5e8d-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f5e8d-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f5e8d-110">Delegated (work or school account)</span></span> | <span data-ttu-id="f5e8d-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f5e8d-111">Files.ReadWrite</span></span>   |
|<span data-ttu-id="f5e8d-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f5e8d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f5e8d-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f5e8d-113">Not supported.</span></span>    |
|<span data-ttu-id="f5e8d-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f5e8d-114">Application</span></span> | <span data-ttu-id="f5e8d-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f5e8d-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f5e8d-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f5e8d-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/application
```

## <a name="request-headers"></a><span data-ttu-id="f5e8d-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f5e8d-117">Request headers</span></span>
| <span data-ttu-id="f5e8d-118">Nome</span><span class="sxs-lookup"><span data-stu-id="f5e8d-118">Name</span></span>      |<span data-ttu-id="f5e8d-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="f5e8d-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="f5e8d-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="f5e8d-120">Authorization</span></span>  | <span data-ttu-id="f5e8d-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f5e8d-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f5e8d-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f5e8d-123">Request body</span></span>
<span data-ttu-id="f5e8d-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f5e8d-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f5e8d-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="f5e8d-125">Response</span></span>

<span data-ttu-id="f5e8d-126">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [workbookApplication](../resources/workbookapplication.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f5e8d-126">If successful, this method returns a `200 OK` response code and a [workbookApplication](../resources/workbookapplication.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f5e8d-127">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f5e8d-127">Example</span></span>
### <a name="request"></a><span data-ttu-id="f5e8d-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f5e8d-128">Request</span></span>
<span data-ttu-id="f5e8d-129">Veja a seguir um exemplo de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="f5e8d-129">Here is an example of a request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="f5e8d-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="f5e8d-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_workbookApplication"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/application
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="f5e8d-131">C#</span><span class="sxs-lookup"><span data-stu-id="f5e8d-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-workbookapplication-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f5e8d-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f5e8d-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-workbookapplication-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="f5e8d-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f5e8d-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-workbookapplication-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="f5e8d-134">Java</span><span class="sxs-lookup"><span data-stu-id="f5e8d-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-workbookapplication-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="f5e8d-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="f5e8d-135">Response</span></span>
<span data-ttu-id="f5e8d-136">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f5e8d-136">Here is an example of the response.</span></span> 

> <span data-ttu-id="f5e8d-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f5e8d-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
