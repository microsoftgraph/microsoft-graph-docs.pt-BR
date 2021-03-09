---
title: 'Worksheet: UsedRange'
description: O intervalo usado é o menor intervalo que abrange todas as células que têm um valor ou uma formatação atribuído a elas. Se a planilha estiver em branco, esta função retorna a célula superior esquerda.
localization_priority: Normal
author: lumine2008
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 3da9ece84c8c6fedd36a08bb6f489eaa89bb8b7c
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/09/2021
ms.locfileid: "50578145"
---
# <a name="worksheet-usedrange"></a><span data-ttu-id="f9ba6-104">Worksheet: UsedRange</span><span class="sxs-lookup"><span data-stu-id="f9ba6-104">Worksheet: UsedRange</span></span>

<span data-ttu-id="f9ba6-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f9ba6-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f9ba6-p102">O intervalo usado é o menor intervalo que abrange todas as células que têm um valor ou uma formatação atribuído a elas. Se a planilha estiver em branco, esta função retorna a célula superior esquerda.</span><span class="sxs-lookup"><span data-stu-id="f9ba6-p102">The used range is the smallest range that encompasses any cells that have a value or formatting assigned to them. If the worksheet is blank, this function will return the top left cell.</span></span>
## <a name="permissions"></a><span data-ttu-id="f9ba6-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="f9ba6-108">Permissions</span></span>
<span data-ttu-id="f9ba6-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f9ba6-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f9ba6-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f9ba6-111">Permission type</span></span>      | <span data-ttu-id="f9ba6-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f9ba6-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f9ba6-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f9ba6-113">Delegated (work or school account)</span></span> | <span data-ttu-id="f9ba6-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f9ba6-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="f9ba6-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f9ba6-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f9ba6-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f9ba6-116">Not supported.</span></span>    |
|<span data-ttu-id="f9ba6-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f9ba6-117">Application</span></span> | <span data-ttu-id="f9ba6-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f9ba6-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f9ba6-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f9ba6-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/items/{id}/workbook/worksheets/{id|name}/UsedRange
GET /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/UsedRange

```

## <a name="function-parameters"></a><span data-ttu-id="f9ba6-120">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="f9ba6-120">Function parameters</span></span>
<span data-ttu-id="f9ba6-121">Na URL de solicitação, forneça um parâmetro de consulta opcional.</span><span class="sxs-lookup"><span data-stu-id="f9ba6-121">In the request URL, provide an optional query parameter.</span></span>

| <span data-ttu-id="f9ba6-122">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="f9ba6-122">Parameter</span></span>    | <span data-ttu-id="f9ba6-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="f9ba6-123">Type</span></span>   |<span data-ttu-id="f9ba6-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="f9ba6-124">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f9ba6-125">valuesOnly</span><span class="sxs-lookup"><span data-stu-id="f9ba6-125">valuesOnly</span></span>|<span data-ttu-id="f9ba6-126">Boolean</span><span class="sxs-lookup"><span data-stu-id="f9ba6-126">Boolean</span></span>|<span data-ttu-id="f9ba6-127">Opcional.</span><span class="sxs-lookup"><span data-stu-id="f9ba6-127">Optional.</span></span> <span data-ttu-id="f9ba6-128">Considera apenas as células com valores como células usadas (ignora a formatação).</span><span class="sxs-lookup"><span data-stu-id="f9ba6-128">Considers only cells with values as used cells (ignores formatting).</span></span>|

## <a name="request-headers"></a><span data-ttu-id="f9ba6-129">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f9ba6-129">Request headers</span></span>
| <span data-ttu-id="f9ba6-130">Nome</span><span class="sxs-lookup"><span data-stu-id="f9ba6-130">Name</span></span>       | <span data-ttu-id="f9ba6-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="f9ba6-131">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="f9ba6-132">Autorização</span><span class="sxs-lookup"><span data-stu-id="f9ba6-132">Authorization</span></span>  | <span data-ttu-id="f9ba6-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f9ba6-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f9ba6-135">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="f9ba6-135">Workbook-Session-Id</span></span>  | <span data-ttu-id="f9ba6-p106">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="f9ba6-p106">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f9ba6-138">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f9ba6-138">Request body</span></span>
<span data-ttu-id="f9ba6-139">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f9ba6-139">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f9ba6-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="f9ba6-140">Response</span></span>

<span data-ttu-id="f9ba6-141">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [workbookRange](../resources/workbookrange.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f9ba6-141">If successful, this method returns `200 OK` response code and [workbookRange](../resources/workbookrange.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f9ba6-142">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f9ba6-142">Example</span></span>
<span data-ttu-id="f9ba6-143">Aqui está um exemplo que mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="f9ba6-143">Here is an example that shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="f9ba6-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f9ba6-144">Request</span></span>
<span data-ttu-id="f9ba6-145">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f9ba6-145">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="f9ba6-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="f9ba6-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "worksheet_usedrange"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/UsedRange(valuesOnly=true)
```
# <a name="c"></a>[<span data-ttu-id="f9ba6-147">C#</span><span class="sxs-lookup"><span data-stu-id="f9ba6-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/worksheet-usedrange-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f9ba6-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f9ba6-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/worksheet-usedrange-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f9ba6-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f9ba6-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/worksheet-usedrange-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f9ba6-150">Java</span><span class="sxs-lookup"><span data-stu-id="f9ba6-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/worksheet-usedrange-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="f9ba6-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="f9ba6-151">Response</span></span>
<span data-ttu-id="f9ba6-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f9ba6-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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


