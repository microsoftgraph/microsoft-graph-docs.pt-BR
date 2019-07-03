---
title: Obter FormatProtection
description: Recupere as propriedades e os relacionamentos do objeto formatprotection.
localization_priority: Normal
ms.openlocfilehash: 8bedae4f9f53bb26caff385236ab9c54cd7a33fe
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35440831"
---
# <a name="get-formatprotection"></a><span data-ttu-id="89ab2-103">Obter FormatProtection</span><span class="sxs-lookup"><span data-stu-id="89ab2-103">Get FormatProtection</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="89ab2-104">Recupere as propriedades e os relacionamentos do objeto formatprotection.</span><span class="sxs-lookup"><span data-stu-id="89ab2-104">Retrieve the properties and relationships of formatprotection object.</span></span>
## <a name="permissions"></a><span data-ttu-id="89ab2-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="89ab2-105">Permissions</span></span>
<span data-ttu-id="89ab2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="89ab2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="89ab2-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="89ab2-108">Permission type</span></span>      | <span data-ttu-id="89ab2-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="89ab2-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="89ab2-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="89ab2-110">Delegated (work or school account)</span></span> | <span data-ttu-id="89ab2-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="89ab2-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="89ab2-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="89ab2-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="89ab2-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="89ab2-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="89ab2-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="89ab2-114">Application</span></span> | <span data-ttu-id="89ab2-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="89ab2-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="89ab2-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="89ab2-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names/{name}/range/format/protection
GET /workbook/worksheets/{id|name}/range(<address>)/format/protection
GET /workbook/tables/{id|name}/columns/{id|name}/range/format/protection
```
## <a name="optional-query-parameters"></a><span data-ttu-id="89ab2-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="89ab2-117">Optional query parameters</span></span>
<span data-ttu-id="89ab2-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="89ab2-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="89ab2-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="89ab2-119">Request headers</span></span>
| <span data-ttu-id="89ab2-120">Nome</span><span class="sxs-lookup"><span data-stu-id="89ab2-120">Name</span></span>      |<span data-ttu-id="89ab2-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="89ab2-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="89ab2-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="89ab2-122">Authorization</span></span>  | <span data-ttu-id="89ab2-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="89ab2-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="89ab2-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="89ab2-125">Request body</span></span>
<span data-ttu-id="89ab2-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="89ab2-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="89ab2-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="89ab2-127">Response</span></span>

<span data-ttu-id="89ab2-128">Se bem sucedido, este método retorna um código de resposta `200 OK` e um objeto [FormatProtection](../resources/formatprotection.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="89ab2-128">If successful, this method returns a `200 OK` response code and [FormatProtection](../resources/formatprotection.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="89ab2-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="89ab2-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="89ab2-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="89ab2-130">Request</span></span>
<span data-ttu-id="89ab2-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="89ab2-131">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="89ab2-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="89ab2-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_formatprotection"
}-->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names/{name}/range/format/protection
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="89ab2-133">C#</span><span class="sxs-lookup"><span data-stu-id="89ab2-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-formatprotection-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="89ab2-134">Javascript</span><span class="sxs-lookup"><span data-stu-id="89ab2-134">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-formatprotection-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="89ab2-135">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="89ab2-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-formatprotection-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="89ab2-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="89ab2-136">Response</span></span>
<span data-ttu-id="89ab2-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="89ab2-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.formatProtection"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 45

{
  "locked": true,
  "formulaHidden": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get FormatProtection",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
