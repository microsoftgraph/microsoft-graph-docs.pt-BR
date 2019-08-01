---
title: 'Worksheet: UsedRange'
description: O intervalo usado é o menor intervalo que abrange todas as células que têm um valor ou uma formatação atribuído a elas. Se a planilha estiver em branco, esta função retorna a célula superior esquerda.
localization_priority: Normal
author: lumine2008
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 756fccce62bab54296e5aa4ba44291ab903e24bf
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36026107"
---
# <a name="worksheet-usedrange"></a><span data-ttu-id="293db-104">Worksheet: UsedRange</span><span class="sxs-lookup"><span data-stu-id="293db-104">Worksheet: UsedRange</span></span>

<span data-ttu-id="293db-p102">O intervalo usado é o menor intervalo que abrange todas as células que têm um valor ou uma formatação atribuído a elas. Se a planilha estiver em branco, esta função retorna a célula superior esquerda.</span><span class="sxs-lookup"><span data-stu-id="293db-p102">The used range is the smallest range that encompasses any cells that have a value or formatting assigned to them. If the worksheet is blank, this function will return the top left cell.</span></span>
## <a name="permissions"></a><span data-ttu-id="293db-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="293db-107">Permissions</span></span>
<span data-ttu-id="293db-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="293db-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="293db-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="293db-110">Permission type</span></span>      | <span data-ttu-id="293db-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="293db-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="293db-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="293db-112">Delegated (work or school account)</span></span> | <span data-ttu-id="293db-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="293db-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="293db-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="293db-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="293db-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="293db-115">Not supported.</span></span>    |
|<span data-ttu-id="293db-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="293db-116">Application</span></span> | <span data-ttu-id="293db-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="293db-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="293db-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="293db-118">HTTP request</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="293db-119">HTTP</span><span class="sxs-lookup"><span data-stu-id="293db-119">HTTP</span></span>](#tab/http)
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets/{id|name}/usedRange

```

## <a name="function-parameters"></a><span data-ttu-id="293db-120">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="293db-120">Function parameters</span></span>
<span data-ttu-id="293db-121">Na URL da solicitação, você pode fornecer parâmetros opcionais.</span><span class="sxs-lookup"><span data-stu-id="293db-121">In the request URL you may provide optional parameters.</span></span>

| <span data-ttu-id="293db-122">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="293db-122">Parameter</span></span>    | <span data-ttu-id="293db-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="293db-123">Type</span></span>   |<span data-ttu-id="293db-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="293db-124">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="293db-125">valuesOnly</span><span class="sxs-lookup"><span data-stu-id="293db-125">valuesOnly</span></span>|<span data-ttu-id="293db-126">Booliano</span><span class="sxs-lookup"><span data-stu-id="293db-126">Boolean</span></span>|<span data-ttu-id="293db-127">Opcional.</span><span class="sxs-lookup"><span data-stu-id="293db-127">Optional.</span></span> <span data-ttu-id="293db-128">Considera apenas as células com valores como células usadas (ignora a formatação).</span><span class="sxs-lookup"><span data-stu-id="293db-128">Considers only cells with values as used cells (ignores formatting).</span></span>|

## <a name="request-headers"></a><span data-ttu-id="293db-129">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="293db-129">Request headers</span></span>
| <span data-ttu-id="293db-130">Nome</span><span class="sxs-lookup"><span data-stu-id="293db-130">Name</span></span>       | <span data-ttu-id="293db-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="293db-131">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="293db-132">Autorização</span><span class="sxs-lookup"><span data-stu-id="293db-132">Authorization</span></span>  | <span data-ttu-id="293db-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="293db-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="293db-135">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="293db-135">Workbook-Session-Id</span></span>  | <span data-ttu-id="293db-p106">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="293db-p106">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="293db-138">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="293db-138">Request body</span></span>
<span data-ttu-id="293db-139">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="293db-139">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="293db-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="293db-140">Response</span></span>

<span data-ttu-id="293db-141">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [Range](../resources/range.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="293db-141">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="293db-142">Exemplo</span><span class="sxs-lookup"><span data-stu-id="293db-142">Example</span></span>
<span data-ttu-id="293db-143">Veja a seguir um exemplo que mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="293db-143">Here is an example that shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="293db-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="293db-144">Request</span></span>
<span data-ttu-id="293db-145">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="293db-145">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "worksheet_usedrange"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/usedRange
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="293db-146">C#</span><span class="sxs-lookup"><span data-stu-id="293db-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/worksheet-usedrange-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="293db-147">Javascript</span><span class="sxs-lookup"><span data-stu-id="293db-147">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/worksheet-usedrange-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="293db-148">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="293db-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/worksheet-usedrange-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="293db-149">Java</span><span class="sxs-lookup"><span data-stu-id="293db-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/worksheet-usedrange-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="293db-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="293db-150">Response</span></span>
<span data-ttu-id="293db-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="293db-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="293db-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="293db-154">HTTP</span></span>](#tab/http)
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
  "addressLocal": "addressLocal-value"
}
```

<span data-ttu-id="293db-155">Como alternativa, essa função pode ser chamada com o parâmetro `valuesOnly` opcional.</span><span class="sxs-lookup"><span data-stu-id="293db-155">Alternatively, this function can be called with the optional `valuesOnly` parameter.</span></span>

##### <a name="request"></a><span data-ttu-id="293db-156">Solicitação</span><span class="sxs-lookup"><span data-stu-id="293db-156">Request</span></span>
<span data-ttu-id="293db-157">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="293db-157">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "worksheet_usedrange_valuesonly"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/usedRange(valuesOnly=true)
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="293db-158">C#</span><span class="sxs-lookup"><span data-stu-id="293db-158">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/worksheet-usedrange-valuesonly-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="293db-159">Javascript</span><span class="sxs-lookup"><span data-stu-id="293db-159">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/worksheet-usedrange-valuesonly-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="293db-160">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="293db-160">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/worksheet-usedrange-valuesonly-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="293db-161">Java</span><span class="sxs-lookup"><span data-stu-id="293db-161">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/worksheet-usedrange-valuesonly-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="293db-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="293db-162">Response</span></span>
<span data-ttu-id="293db-p108">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="293db-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "addressLocal": "addressLocal-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Worksheet: UsedRange",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
