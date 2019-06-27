---
title: Obter categoria do Outlook
description: Obtenha as propriedades e as relações do objeto outlookCategory especificado.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 64990c82ce7c8de65274c37b76ae64f2750015dd
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35265797"
---
# <a name="get-outlook-category"></a><span data-ttu-id="30ff7-103">Obter categoria do Outlook</span><span class="sxs-lookup"><span data-stu-id="30ff7-103">Get Outlook category</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="30ff7-104">Obtenha as propriedades e as relações do objeto [outlookCategory](../resources/outlookcategory.md) especificado.</span><span class="sxs-lookup"><span data-stu-id="30ff7-104">Get the properties and relationships of the specified [outlookCategory](../resources/outlookcategory.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="30ff7-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="30ff7-105">Permissions</span></span>
<span data-ttu-id="30ff7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="30ff7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="30ff7-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="30ff7-108">Permission type</span></span>      | <span data-ttu-id="30ff7-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="30ff7-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="30ff7-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="30ff7-110">Delegated (work or school account)</span></span> | <span data-ttu-id="30ff7-111">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="30ff7-111">MailboxSettings.Read</span></span>    |
|<span data-ttu-id="30ff7-112">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="30ff7-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="30ff7-113">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="30ff7-113">MailboxSettings.Read</span></span>    |
|<span data-ttu-id="30ff7-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="30ff7-114">Application</span></span> | <span data-ttu-id="30ff7-115">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="30ff7-115">MailboxSettings.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="30ff7-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="30ff7-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/outlook/masterCategories/{id}
GET /users/{id|userPrincipalName}/outlook/masterCategories/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="30ff7-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="30ff7-117">Optional query parameters</span></span>
<span data-ttu-id="30ff7-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="30ff7-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="30ff7-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="30ff7-119">Request headers</span></span>
| <span data-ttu-id="30ff7-120">Nome</span><span class="sxs-lookup"><span data-stu-id="30ff7-120">Name</span></span>      |<span data-ttu-id="30ff7-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="30ff7-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="30ff7-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="30ff7-122">Authorization</span></span>  | <span data-ttu-id="30ff7-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="30ff7-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="30ff7-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="30ff7-125">Request body</span></span>
<span data-ttu-id="30ff7-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="30ff7-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="30ff7-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="30ff7-127">Response</span></span>

<span data-ttu-id="30ff7-128">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [outlookCategory](../resources/outlookcategory.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="30ff7-128">If successful, this method returns a `200 OK` response code and [outlookCategory](../resources/outlookcategory.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="30ff7-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="30ff7-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="30ff7-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="30ff7-130">Request</span></span>
<span data-ttu-id="30ff7-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="30ff7-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_outlookcategory"
}-->
```http
GET https://graph.microsoft.com/beta/me/outlook/masterCategories/de912e4d-c790-4da9-949c-ccd933aaa0f7
```
##### <a name="response"></a><span data-ttu-id="30ff7-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="30ff7-132">Response</span></span>
<span data-ttu-id="30ff7-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="30ff7-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="30ff7-136">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="30ff7-136">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="30ff7-137">C#</span><span class="sxs-lookup"><span data-stu-id="30ff7-137">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_outlookcategory-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="30ff7-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="30ff7-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_outlookcategory-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="30ff7-139">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="30ff7-139">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_outlookcategory-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/outlookcategory-get.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/outlookcategory-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/outlookcategory-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
