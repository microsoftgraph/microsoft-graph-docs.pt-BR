---
title: 'Worksheet: Range'
description: Obtém o objeto de intervalo especificado pelo nome ou endereço.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 5aecc0100d0915c16afa72a95e162fa2907b4a55
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/04/2019
ms.locfileid: "36728830"
---
# <a name="worksheet-range"></a><span data-ttu-id="4ba53-103">Worksheet: Range</span><span class="sxs-lookup"><span data-stu-id="4ba53-103">Worksheet: Range</span></span>

<span data-ttu-id="4ba53-104">Obtém o objeto de intervalo especificado pelo nome ou endereço.</span><span class="sxs-lookup"><span data-stu-id="4ba53-104">Gets the range object specified by the address or name.</span></span>
## <a name="permissions"></a><span data-ttu-id="4ba53-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="4ba53-105">Permissions</span></span>
<span data-ttu-id="4ba53-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4ba53-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4ba53-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4ba53-108">Permission type</span></span>      | <span data-ttu-id="4ba53-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4ba53-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4ba53-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4ba53-110">Delegated (work or school account)</span></span> | <span data-ttu-id="4ba53-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4ba53-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="4ba53-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4ba53-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4ba53-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4ba53-113">Not supported.</span></span>    |
|<span data-ttu-id="4ba53-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4ba53-114">Application</span></span> | <span data-ttu-id="4ba53-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4ba53-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4ba53-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4ba53-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets/{id|name}/range

```
## <a name="request-headers"></a><span data-ttu-id="4ba53-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4ba53-117">Request headers</span></span>
| <span data-ttu-id="4ba53-118">Nome</span><span class="sxs-lookup"><span data-stu-id="4ba53-118">Name</span></span>       | <span data-ttu-id="4ba53-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="4ba53-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="4ba53-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="4ba53-120">Authorization</span></span>  | <span data-ttu-id="4ba53-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4ba53-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="4ba53-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="4ba53-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="4ba53-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="4ba53-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="function-parameters"></a><span data-ttu-id="4ba53-126">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="4ba53-126">Function parameters</span></span>

| <span data-ttu-id="4ba53-127">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="4ba53-127">Parameter</span></span>    | <span data-ttu-id="4ba53-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="4ba53-128">Type</span></span>   |<span data-ttu-id="4ba53-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="4ba53-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4ba53-130">address</span><span class="sxs-lookup"><span data-stu-id="4ba53-130">address</span></span>|<span data-ttu-id="4ba53-131">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4ba53-131">string</span></span>|<span data-ttu-id="4ba53-p104">Opcional. O endereço ou nome do intervalo. Caso não seja especificado, todo o intervalo da planilha será retornado.</span><span class="sxs-lookup"><span data-stu-id="4ba53-p104">Optional. The address or the name of the range. If not specified, the entire worksheet range is returned.</span></span>|

## <a name="response"></a><span data-ttu-id="4ba53-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="4ba53-135">Response</span></span>

<span data-ttu-id="4ba53-136">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [Range](../resources/range.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4ba53-136">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4ba53-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4ba53-137">Example</span></span>
<span data-ttu-id="4ba53-138">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="4ba53-138">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="4ba53-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4ba53-139">Request</span></span>
<span data-ttu-id="4ba53-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4ba53-140">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="4ba53-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="4ba53-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "worksheet_range"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/range(address='A1:B2')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="4ba53-142">C#</span><span class="sxs-lookup"><span data-stu-id="4ba53-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/worksheet-range-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="4ba53-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4ba53-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/worksheet-range-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="4ba53-144">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="4ba53-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/worksheet-range-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="4ba53-145">Java</span><span class="sxs-lookup"><span data-stu-id="4ba53-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/worksheet-range-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="4ba53-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="4ba53-146">Response</span></span>
<span data-ttu-id="4ba53-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4ba53-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRange"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 169

{
  "address": "address-value",
  "addressLocal": "addressLocal-value",
  "cellCount": 99,
  "columnCount": 99,
  "columnIndex": 99,
  "valueTypes": "valueTypes-value"
}
```

<span data-ttu-id="4ba53-150">Se o parâmetro `address` optional não for especificado, essa função retornará todo o intervalo de planilha.</span><span class="sxs-lookup"><span data-stu-id="4ba53-150">If the optional `address` parameter is not specified, this function returns the entire worksheet range.</span></span>

##### <a name="request"></a><span data-ttu-id="4ba53-151">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4ba53-151">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="4ba53-152">HTTP</span><span class="sxs-lookup"><span data-stu-id="4ba53-152">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "worksheet_range_noaddress"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/range
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="4ba53-153">C#</span><span class="sxs-lookup"><span data-stu-id="4ba53-153">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/worksheet-range-noaddress-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="4ba53-154">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4ba53-154">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/worksheet-range-noaddress-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="4ba53-155">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="4ba53-155">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/worksheet-range-noaddress-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="4ba53-156">Java</span><span class="sxs-lookup"><span data-stu-id="4ba53-156">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/worksheet-range-noaddress-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="4ba53-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="4ba53-157">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRange"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 169

{
  "address": "address-value",
  "addressLocal": "addressLocal-value",
  "cellCount": 99,
  "columnCount": 99,
  "columnIndex": 99,
  "valueTypes": "valueTypes-value"
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Worksheet: Range",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
