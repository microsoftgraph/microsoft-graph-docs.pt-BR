---
title: 'Worksheet: Range'
description: Obtém o objeto de intervalo especificado pelo nome ou endereço.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 804ce9a4caa19d427e47599a7be0a8f49b6fba5f
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/09/2021
ms.locfileid: "50575046"
---
# <a name="worksheet-range"></a><span data-ttu-id="aa64c-103">Worksheet: Range</span><span class="sxs-lookup"><span data-stu-id="aa64c-103">Worksheet: Range</span></span>

<span data-ttu-id="aa64c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="aa64c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="aa64c-105">Obtém o objeto de intervalo especificado pelo nome ou endereço.</span><span class="sxs-lookup"><span data-stu-id="aa64c-105">Gets the range object specified by the address or name.</span></span>
## <a name="permissions"></a><span data-ttu-id="aa64c-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="aa64c-106">Permissions</span></span>
<span data-ttu-id="aa64c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="aa64c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="aa64c-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="aa64c-109">Permission type</span></span>      | <span data-ttu-id="aa64c-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="aa64c-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="aa64c-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="aa64c-111">Delegated (work or school account)</span></span> | <span data-ttu-id="aa64c-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="aa64c-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="aa64c-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="aa64c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="aa64c-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="aa64c-114">Not supported.</span></span>    |
|<span data-ttu-id="aa64c-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="aa64c-115">Application</span></span> | <span data-ttu-id="aa64c-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="aa64c-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="aa64c-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="aa64c-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/items/{id}/workbook/worksheets/{id|name}/range
GET /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/range

```
## <a name="request-headers"></a><span data-ttu-id="aa64c-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="aa64c-118">Request headers</span></span>
| <span data-ttu-id="aa64c-119">Nome</span><span class="sxs-lookup"><span data-stu-id="aa64c-119">Name</span></span>       | <span data-ttu-id="aa64c-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="aa64c-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="aa64c-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="aa64c-121">Authorization</span></span>  | <span data-ttu-id="aa64c-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="aa64c-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="aa64c-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="aa64c-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="aa64c-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="aa64c-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="function-parameters"></a><span data-ttu-id="aa64c-127">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="aa64c-127">Function parameters</span></span>

| <span data-ttu-id="aa64c-128">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="aa64c-128">Parameter</span></span>    | <span data-ttu-id="aa64c-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="aa64c-129">Type</span></span>   |<span data-ttu-id="aa64c-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="aa64c-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="aa64c-131">address</span><span class="sxs-lookup"><span data-stu-id="aa64c-131">address</span></span>|<span data-ttu-id="aa64c-132">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="aa64c-132">string</span></span>|<span data-ttu-id="aa64c-p104">Opcional. O endereço ou nome do intervalo. Caso não seja especificado, todo o intervalo da planilha será retornado.</span><span class="sxs-lookup"><span data-stu-id="aa64c-p104">Optional. The address or the name of the range. If not specified, the entire worksheet range is returned.</span></span>|

## <a name="response"></a><span data-ttu-id="aa64c-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="aa64c-136">Response</span></span>

<span data-ttu-id="aa64c-137">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [Range](../resources/range.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="aa64c-137">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="aa64c-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="aa64c-138">Example</span></span>
<span data-ttu-id="aa64c-139">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="aa64c-139">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="aa64c-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="aa64c-140">Request</span></span>
<span data-ttu-id="aa64c-141">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="aa64c-141">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="aa64c-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="aa64c-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "worksheet_range"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/range(address='A1:B2')
```
# <a name="c"></a>[<span data-ttu-id="aa64c-143">C#</span><span class="sxs-lookup"><span data-stu-id="aa64c-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/worksheet-range-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="aa64c-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="aa64c-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/worksheet-range-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="aa64c-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="aa64c-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/worksheet-range-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="aa64c-146">Java</span><span class="sxs-lookup"><span data-stu-id="aa64c-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/worksheet-range-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="aa64c-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="aa64c-147">Response</span></span>
<span data-ttu-id="aa64c-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="aa64c-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

<span data-ttu-id="aa64c-151">Se o parâmetro `address` opcional não for especificado, essa função retornará todo o intervalo de planilhas.</span><span class="sxs-lookup"><span data-stu-id="aa64c-151">If the optional `address` parameter is not specified, this function returns the entire worksheet range.</span></span>

##### <a name="request"></a><span data-ttu-id="aa64c-152">Solicitação</span><span class="sxs-lookup"><span data-stu-id="aa64c-152">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="aa64c-153">HTTP</span><span class="sxs-lookup"><span data-stu-id="aa64c-153">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "worksheet_range_noaddress"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/range
```
# <a name="c"></a>[<span data-ttu-id="aa64c-154">C#</span><span class="sxs-lookup"><span data-stu-id="aa64c-154">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/worksheet-range-noaddress-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="aa64c-155">JavaScript</span><span class="sxs-lookup"><span data-stu-id="aa64c-155">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/worksheet-range-noaddress-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="aa64c-156">Objective-C</span><span class="sxs-lookup"><span data-stu-id="aa64c-156">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/worksheet-range-noaddress-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="aa64c-157">Java</span><span class="sxs-lookup"><span data-stu-id="aa64c-157">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/worksheet-range-noaddress-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="aa64c-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="aa64c-158">Response</span></span>

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

