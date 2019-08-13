---
title: 'workbookRange: columnsBefore'
description: Obtém um determinado número de colunas à esquerda do intervalo especificado.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 528b5e9a76c4b916b4026bbf5755f7fa94ae1f67
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36361909"
---
# <a name="workbookrange-columnsbefore"></a><span data-ttu-id="da212-103">workbookRange: columnsBefore</span><span class="sxs-lookup"><span data-stu-id="da212-103">workbookRange: columnsBefore</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="da212-104">Obtém um determinado número de colunas à esquerda do intervalo especificado.</span><span class="sxs-lookup"><span data-stu-id="da212-104">Gets a certain number of columns to the left of the given range.</span></span>

## <a name="permissions"></a><span data-ttu-id="da212-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="da212-105">Permissions</span></span>
<span data-ttu-id="da212-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="da212-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="da212-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="da212-108">Permission type</span></span>      | <span data-ttu-id="da212-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="da212-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="da212-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="da212-110">Delegated (work or school account)</span></span> | <span data-ttu-id="da212-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="da212-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="da212-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="da212-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="da212-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="da212-113">Not supported.</span></span>    |
|<span data-ttu-id="da212-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="da212-114">Application</span></span> | <span data-ttu-id="da212-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="da212-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="da212-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="da212-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/root/workbook/worksheets/{id}/range/columnsBefore(count=n)

```

## <a name="function-parameters"></a><span data-ttu-id="da212-117">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="da212-117">Function parameters</span></span>

| <span data-ttu-id="da212-118">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="da212-118">Parameter</span></span>    | <span data-ttu-id="da212-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="da212-119">Type</span></span>   |<span data-ttu-id="da212-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="da212-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="da212-121">Count</span><span class="sxs-lookup"><span data-stu-id="da212-121">count</span></span>|<span data-ttu-id="da212-122">Int32</span><span class="sxs-lookup"><span data-stu-id="da212-122">Int32</span></span>|<span data-ttu-id="da212-123">O número de colunas a serem incluídas no intervalo resultante.</span><span class="sxs-lookup"><span data-stu-id="da212-123">The number of columns to include in the resulting range.</span></span> <span data-ttu-id="da212-124">Em geral, use um número positivo para criar um intervalo fora do intervalo atual.</span><span class="sxs-lookup"><span data-stu-id="da212-124">In general, use a positive number to create a range outside the current range.</span></span> <span data-ttu-id="da212-125">Você também pode usar um número negativo para criar um intervalo dentro do intervalo atual.</span><span class="sxs-lookup"><span data-stu-id="da212-125">You can also use a negative number to create a range within the current range.</span></span> <span data-ttu-id="da212-126">O valor padrão é 1.</span><span class="sxs-lookup"><span data-stu-id="da212-126">The default value is 1.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="da212-127">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="da212-127">Request headers</span></span>
| <span data-ttu-id="da212-128">Nome</span><span class="sxs-lookup"><span data-stu-id="da212-128">Name</span></span>       | <span data-ttu-id="da212-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="da212-129">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="da212-130">Autorização</span><span class="sxs-lookup"><span data-stu-id="da212-130">Authorization</span></span>  | <span data-ttu-id="da212-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="da212-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="da212-133">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="da212-133">Workbook-Session-Id</span></span>  | <span data-ttu-id="da212-p104">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="da212-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="da212-136">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="da212-136">Request body</span></span>
<span data-ttu-id="da212-137">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="da212-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="da212-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="da212-138">Response</span></span>
<span data-ttu-id="da212-139">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [workbookRange](../resources/workbookrange.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="da212-139">If successful, this method returns `200 OK` response code and [workbookRange](../resources/workbookrange.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="da212-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="da212-140">Example</span></span>
<span data-ttu-id="da212-141">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="da212-141">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="da212-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="da212-142">Request</span></span>
<span data-ttu-id="da212-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="da212-143">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="da212-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="da212-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "workbookrange_columnsbefore"
}-->
```http
POST https://graph.microsoft.com/beta/drive/root/workbook/worksheets/{id}/range/columnsBefore(count=2)
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="da212-145">C#</span><span class="sxs-lookup"><span data-stu-id="da212-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/workbookrange-columnsbefore-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="da212-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="da212-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/workbookrange-columnsbefore-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="da212-147">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="da212-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/workbookrange-columnsbefore-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="da212-148">Java</span><span class="sxs-lookup"><span data-stu-id="da212-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/workbookrange-columnsbefore-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="da212-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="da212-149">Response</span></span>
<span data-ttu-id="da212-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="da212-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRange"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 157

{
  "address": "address-value",
  "addressLocal": "addressLocal-value",
  "cellCount": 99,
  "columnCount": 99,
  "columnHidden": true,
  "columnIndex": 99
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79 
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Example",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
