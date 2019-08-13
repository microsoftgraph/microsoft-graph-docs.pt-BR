---
title: Obter workbookApplication
description: Recupere as propriedades e os relacionamentos do objeto workbookApplication.
localization_priority: Normal
author: lumine2008
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: dfe43bea86a733fc129a0119b576625ff27eaea1
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36325892"
---
# <a name="get-workbookapplication"></a><span data-ttu-id="460cb-103">Obter workbookApplication</span><span class="sxs-lookup"><span data-stu-id="460cb-103">Get workbookApplication</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="460cb-104">Recupere as propriedades e os relacionamentos do objeto workbookApplication.</span><span class="sxs-lookup"><span data-stu-id="460cb-104">Retrieve the properties and relationships of workbookApplication object.</span></span>
## <a name="permissions"></a><span data-ttu-id="460cb-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="460cb-105">Permissions</span></span>
<span data-ttu-id="460cb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="460cb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="460cb-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="460cb-108">Permission type</span></span>      | <span data-ttu-id="460cb-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="460cb-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="460cb-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="460cb-110">Delegated (work or school account)</span></span> | <span data-ttu-id="460cb-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="460cb-111">Not supported.</span></span>    |
|<span data-ttu-id="460cb-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="460cb-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="460cb-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="460cb-113">Not supported.</span></span>    |
|<span data-ttu-id="460cb-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="460cb-114">Application</span></span> | <span data-ttu-id="460cb-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="460cb-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="460cb-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="460cb-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/application
```
## <a name="optional-query-parameters"></a><span data-ttu-id="460cb-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="460cb-117">Optional query parameters</span></span>
<span data-ttu-id="460cb-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="460cb-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="460cb-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="460cb-119">Request headers</span></span>
| <span data-ttu-id="460cb-120">Nome</span><span class="sxs-lookup"><span data-stu-id="460cb-120">Name</span></span>      |<span data-ttu-id="460cb-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="460cb-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="460cb-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="460cb-122">Authorization</span></span>  | <span data-ttu-id="460cb-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="460cb-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="460cb-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="460cb-125">Request body</span></span>
<span data-ttu-id="460cb-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="460cb-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="460cb-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="460cb-127">Response</span></span>

<span data-ttu-id="460cb-128">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [workbookApplication](../resources/workbookapplication.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="460cb-128">If successful, this method returns a `200 OK` response code and [workbookApplication](../resources/workbookapplication.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="460cb-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="460cb-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="460cb-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="460cb-130">Request</span></span>
<span data-ttu-id="460cb-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="460cb-131">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="460cb-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="460cb-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_workbookApplication"
}-->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/application
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="460cb-133">C#</span><span class="sxs-lookup"><span data-stu-id="460cb-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-workbookapplication-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="460cb-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="460cb-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-workbookapplication-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="460cb-135">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="460cb-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-workbookapplication-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="460cb-136">Java</span><span class="sxs-lookup"><span data-stu-id="460cb-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-workbookapplication-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="460cb-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="460cb-137">Response</span></span>
<span data-ttu-id="460cb-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="460cb-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
