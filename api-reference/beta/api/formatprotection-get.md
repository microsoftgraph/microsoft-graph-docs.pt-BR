---
title: Obter FormatProtection
description: Recupere as propriedades e os relacionamentos do objeto formatprotection.
localization_priority: Normal
doc_type: apiPageType
author: ruoyingl
ms.prod: ''
ms.openlocfilehash: 83e6eb0c684e129ec79aa49be83a356238196f03
ms.sourcegitcommit: 7ceec757fd82ef3fd80aa3089ef46d3807aa3aa2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/09/2020
ms.locfileid: "48403168"
---
# <a name="get-formatprotection"></a><span data-ttu-id="ad916-103">Get FormatProtection</span><span class="sxs-lookup"><span data-stu-id="ad916-103">Get FormatProtection</span></span>

<span data-ttu-id="ad916-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ad916-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ad916-105">Recupere as propriedades e os relacionamentos do objeto formatprotection.</span><span class="sxs-lookup"><span data-stu-id="ad916-105">Retrieve the properties and relationships of formatprotection object.</span></span>
## <a name="permissions"></a><span data-ttu-id="ad916-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="ad916-106">Permissions</span></span>
<span data-ttu-id="ad916-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ad916-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ad916-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ad916-109">Permission type</span></span>      | <span data-ttu-id="ad916-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ad916-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ad916-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ad916-111">Delegated (work or school account)</span></span> | <span data-ttu-id="ad916-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ad916-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="ad916-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ad916-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ad916-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ad916-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="ad916-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ad916-115">Application</span></span> | <span data-ttu-id="ad916-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ad916-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ad916-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ad916-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names/{name}/range/format/protection
GET /workbook/worksheets/{id|name}/range(<address>)/format/protection
GET /workbook/tables/{id|name}/columns/{id|name}/range/format/protection
```
## <a name="optional-query-parameters"></a><span data-ttu-id="ad916-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="ad916-118">Optional query parameters</span></span>
<span data-ttu-id="ad916-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="ad916-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ad916-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ad916-120">Request headers</span></span>
| <span data-ttu-id="ad916-121">Nome</span><span class="sxs-lookup"><span data-stu-id="ad916-121">Name</span></span>      |<span data-ttu-id="ad916-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="ad916-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="ad916-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="ad916-123">Authorization</span></span>  | <span data-ttu-id="ad916-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ad916-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ad916-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ad916-126">Request body</span></span>
<span data-ttu-id="ad916-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ad916-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ad916-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="ad916-128">Response</span></span>

<span data-ttu-id="ad916-129">Se bem sucedido, este método retorna um código de resposta `200 OK` e um objeto [FormatProtection](../resources/formatprotection.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ad916-129">If successful, this method returns a `200 OK` response code and [FormatProtection](../resources/formatprotection.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ad916-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ad916-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ad916-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ad916-131">Request</span></span>
<span data-ttu-id="ad916-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ad916-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ad916-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="ad916-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_formatprotection"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names/{name}/range/format/protection
```
# <a name="c"></a>[<span data-ttu-id="ad916-134">C#</span><span class="sxs-lookup"><span data-stu-id="ad916-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-formatprotection-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ad916-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ad916-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-formatprotection-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ad916-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ad916-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-formatprotection-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="ad916-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="ad916-137">Response</span></span>
<span data-ttu-id="ad916-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ad916-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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