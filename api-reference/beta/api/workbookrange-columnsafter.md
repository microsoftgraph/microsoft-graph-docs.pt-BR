---
title: 'workbookRange: columnsAfter'
description: Obtém um determinado número de colunas à direita do intervalo especificado.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 900e0f1c35aa9a793d8c4cd7d7e5699311de9e3c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42451375"
---
# <a name="workbookrange-columnsafter"></a><span data-ttu-id="ec228-103">workbookRange: columnsAfter</span><span class="sxs-lookup"><span data-stu-id="ec228-103">workbookRange: columnsAfter</span></span>

<span data-ttu-id="ec228-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="ec228-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ec228-105">Obtém um determinado número de colunas à direita do intervalo especificado.</span><span class="sxs-lookup"><span data-stu-id="ec228-105">Gets a certain number of columns to the right of the given range.</span></span>

## <a name="permissions"></a><span data-ttu-id="ec228-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="ec228-106">Permissions</span></span>
<span data-ttu-id="ec228-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ec228-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ec228-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ec228-109">Permission type</span></span>      | <span data-ttu-id="ec228-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ec228-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ec228-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ec228-111">Delegated (work or school account)</span></span> | <span data-ttu-id="ec228-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ec228-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="ec228-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ec228-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ec228-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ec228-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="ec228-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ec228-115">Application</span></span> | <span data-ttu-id="ec228-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ec228-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ec228-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ec228-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/root/workbook/worksheets/{id}/range/columnsAfter(count=n)

```
## <a name="function-parameters"></a><span data-ttu-id="ec228-118">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="ec228-118">Function parameters</span></span>

| <span data-ttu-id="ec228-119">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="ec228-119">Parameter</span></span>    | <span data-ttu-id="ec228-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="ec228-120">Type</span></span>   |<span data-ttu-id="ec228-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="ec228-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ec228-122">Count</span><span class="sxs-lookup"><span data-stu-id="ec228-122">count</span></span>|<span data-ttu-id="ec228-123">Int32</span><span class="sxs-lookup"><span data-stu-id="ec228-123">Int32</span></span>|<span data-ttu-id="ec228-p102">O número de colunas a serem incluídas no intervalo resultante. Em geral, use um número positivo para criar um intervalo fora do intervalo atual. Você também pode usar um número negativo para criar um intervalo dentro do intervalo atual. O valor padrão é 1</span><span class="sxs-lookup"><span data-stu-id="ec228-p102">The number of columns to include in the resulting range. In general, use a positive number to create a range outside the current range. You can also use a negative number to create a range within the current range. The default value is 1</span></span>|

## <a name="request-headers"></a><span data-ttu-id="ec228-128">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ec228-128">Request headers</span></span>
| <span data-ttu-id="ec228-129">Nome</span><span class="sxs-lookup"><span data-stu-id="ec228-129">Name</span></span>       | <span data-ttu-id="ec228-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="ec228-130">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="ec228-131">Autorização</span><span class="sxs-lookup"><span data-stu-id="ec228-131">Authorization</span></span>  | <span data-ttu-id="ec228-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ec228-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ec228-134">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="ec228-134">Workbook-Session-Id</span></span>  | <span data-ttu-id="ec228-p104">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="ec228-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ec228-137">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ec228-137">Request body</span></span>
<span data-ttu-id="ec228-138">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ec228-138">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ec228-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="ec228-139">Response</span></span>

<span data-ttu-id="ec228-140">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [workbookRange](../resources/workbookrange.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ec228-140">If successful, this method returns `200 OK` response code and [workbookRange](../resources/workbookrange.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ec228-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ec228-141">Example</span></span>
<span data-ttu-id="ec228-142">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="ec228-142">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="ec228-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ec228-143">Request</span></span>
<span data-ttu-id="ec228-144">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ec228-144">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ec228-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="ec228-145">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "workbookrange_columnsafter"
}-->
```http
POST https://graph.microsoft.com/beta/drive/root/workbook/worksheets/{id}/range/columnsAfter(count=2)
```
# <a name="c"></a>[<span data-ttu-id="ec228-146">C#</span><span class="sxs-lookup"><span data-stu-id="ec228-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/workbookrange-columnsafter-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ec228-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ec228-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/workbookrange-columnsafter-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ec228-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ec228-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/workbookrange-columnsafter-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="ec228-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="ec228-149">Response</span></span>
<span data-ttu-id="ec228-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ec228-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
