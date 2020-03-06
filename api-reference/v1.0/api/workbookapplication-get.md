---
title: Obter workbookApplication
description: Recupere as propriedades e os relacionamentos de um objeto workbookApplication.
localization_priority: Normal
author: grangeryy
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: f03aeca5c15d26854954ecd4f459e5c0ab49cb4e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42508818"
---
# <a name="get-workbookapplication"></a><span data-ttu-id="081cb-103">Obter workbookApplication</span><span class="sxs-lookup"><span data-stu-id="081cb-103">Get workbookApplication</span></span>

<span data-ttu-id="081cb-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="081cb-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="081cb-105">Recupere as propriedades e os relacionamentos de um objeto [workbookApplication](../resources/workbookapplication.md) .</span><span class="sxs-lookup"><span data-stu-id="081cb-105">Retrieve the properties and relationships of a [workbookApplication](../resources/workbookapplication.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="081cb-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="081cb-106">Permissions</span></span>
<span data-ttu-id="081cb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="081cb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="081cb-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="081cb-109">Permission type</span></span>      | <span data-ttu-id="081cb-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="081cb-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="081cb-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="081cb-111">Delegated (work or school account)</span></span> | <span data-ttu-id="081cb-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="081cb-112">Files.ReadWrite</span></span>   |
|<span data-ttu-id="081cb-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="081cb-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="081cb-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="081cb-114">Not supported.</span></span>    |
|<span data-ttu-id="081cb-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="081cb-115">Application</span></span> | <span data-ttu-id="081cb-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="081cb-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="081cb-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="081cb-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/application
```

## <a name="request-headers"></a><span data-ttu-id="081cb-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="081cb-118">Request headers</span></span>
| <span data-ttu-id="081cb-119">Nome</span><span class="sxs-lookup"><span data-stu-id="081cb-119">Name</span></span>      |<span data-ttu-id="081cb-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="081cb-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="081cb-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="081cb-121">Authorization</span></span>  | <span data-ttu-id="081cb-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="081cb-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="081cb-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="081cb-124">Request body</span></span>
<span data-ttu-id="081cb-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="081cb-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="081cb-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="081cb-126">Response</span></span>

<span data-ttu-id="081cb-127">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [workbookApplication](../resources/workbookapplication.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="081cb-127">If successful, this method returns a `200 OK` response code and a [workbookApplication](../resources/workbookapplication.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="081cb-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="081cb-128">Example</span></span>
### <a name="request"></a><span data-ttu-id="081cb-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="081cb-129">Request</span></span>
<span data-ttu-id="081cb-130">Veja a seguir um exemplo de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="081cb-130">Here is an example of a request.</span></span>


# <a name="http"></a>[<span data-ttu-id="081cb-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="081cb-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_workbookApplication"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/application
```
# <a name="c"></a>[<span data-ttu-id="081cb-132">C#</span><span class="sxs-lookup"><span data-stu-id="081cb-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-workbookapplication-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="081cb-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="081cb-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-workbookapplication-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="081cb-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="081cb-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-workbookapplication-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="081cb-135">Java</span><span class="sxs-lookup"><span data-stu-id="081cb-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-workbookapplication-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="081cb-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="081cb-136">Response</span></span>
<span data-ttu-id="081cb-137">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="081cb-137">Here is an example of the response.</span></span> 

> <span data-ttu-id="081cb-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="081cb-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
