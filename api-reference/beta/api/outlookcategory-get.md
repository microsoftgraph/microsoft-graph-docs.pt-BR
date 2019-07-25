---
title: Obter categoria do Outlook
description: Obtenha as propriedades e as relações do objeto outlookCategory especificado.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 015946263a5ad169a85a147a20ebe84d078300de
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35877782"
---
# <a name="get-outlook-category"></a><span data-ttu-id="510a6-103">Obter categoria do Outlook</span><span class="sxs-lookup"><span data-stu-id="510a6-103">Get Outlook category</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="510a6-104">Obtenha as propriedades e as relações do objeto [outlookCategory](../resources/outlookcategory.md) especificado.</span><span class="sxs-lookup"><span data-stu-id="510a6-104">Get the properties and relationships of the specified [outlookCategory](../resources/outlookcategory.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="510a6-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="510a6-105">Permissions</span></span>
<span data-ttu-id="510a6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="510a6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="510a6-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="510a6-108">Permission type</span></span>      | <span data-ttu-id="510a6-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="510a6-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="510a6-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="510a6-110">Delegated (work or school account)</span></span> | <span data-ttu-id="510a6-111">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="510a6-111">MailboxSettings.Read</span></span>    |
|<span data-ttu-id="510a6-112">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="510a6-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="510a6-113">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="510a6-113">MailboxSettings.Read</span></span>    |
|<span data-ttu-id="510a6-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="510a6-114">Application</span></span> | <span data-ttu-id="510a6-115">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="510a6-115">MailboxSettings.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="510a6-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="510a6-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/outlook/masterCategories/{id}
GET /users/{id|userPrincipalName}/outlook/masterCategories/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="510a6-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="510a6-117">Optional query parameters</span></span>
<span data-ttu-id="510a6-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="510a6-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="510a6-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="510a6-119">Request headers</span></span>
| <span data-ttu-id="510a6-120">Nome</span><span class="sxs-lookup"><span data-stu-id="510a6-120">Name</span></span>      |<span data-ttu-id="510a6-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="510a6-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="510a6-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="510a6-122">Authorization</span></span>  | <span data-ttu-id="510a6-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="510a6-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="510a6-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="510a6-125">Request body</span></span>
<span data-ttu-id="510a6-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="510a6-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="510a6-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="510a6-127">Response</span></span>

<span data-ttu-id="510a6-128">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [outlookCategory](../resources/outlookcategory.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="510a6-128">If successful, this method returns a `200 OK` response code and [outlookCategory](../resources/outlookcategory.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="510a6-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="510a6-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="510a6-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="510a6-130">Request</span></span>
<span data-ttu-id="510a6-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="510a6-131">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="510a6-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="510a6-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_outlookcategory"
}-->
```http
GET https://graph.microsoft.com/beta/me/outlook/masterCategories/de912e4d-c790-4da9-949c-ccd933aaa0f7
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="510a6-133">C#</span><span class="sxs-lookup"><span data-stu-id="510a6-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-outlookcategory-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="510a6-134">Javascript</span><span class="sxs-lookup"><span data-stu-id="510a6-134">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-outlookcategory-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="510a6-135">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="510a6-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-outlookcategory-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="510a6-136">Java</span><span class="sxs-lookup"><span data-stu-id="510a6-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-outlookcategory-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="510a6-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="510a6-137">Response</span></span>
<span data-ttu-id="510a6-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="510a6-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.outlookCategory",
  "isCollection": false
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 249

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#users('8ae6f565-0d7f-4ead-853e-7db94c912a1f')/outlook/masterCategories/$entity",
  "id":"de912e4d-c790-4da9-949c-ccd933aaa0f7",
  "displayName":"Yellow category",
  "color":"preset3"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get outlookCategory",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
