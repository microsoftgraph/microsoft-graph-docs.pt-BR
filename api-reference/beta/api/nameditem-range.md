---
title: 'NamedItem: Range'
description: Retorna o objeto Range associado ao nome. Gera uma exceção quando o tipo de item nomeado não é um intervalo.
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: 6938ab3e73e43ea2ffc9d3bac0a9f9101f0c2c0c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42456801"
---
# <a name="nameditem-range"></a><span data-ttu-id="81eb7-104">NamedItem: Range</span><span class="sxs-lookup"><span data-stu-id="81eb7-104">NamedItem: Range</span></span>

<span data-ttu-id="81eb7-105">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="81eb7-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="81eb7-p102">Retorna o objeto Range associado ao nome. Gera uma exceção quando o tipo de item nomeado não é um intervalo.</span><span class="sxs-lookup"><span data-stu-id="81eb7-p102">Returns the range object that is associated with the name. Throws an exception if the named item's type is not a range.</span></span>
## <a name="permissions"></a><span data-ttu-id="81eb7-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="81eb7-108">Permissions</span></span>
<span data-ttu-id="81eb7-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="81eb7-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="81eb7-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="81eb7-111">Permission type</span></span>      | <span data-ttu-id="81eb7-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="81eb7-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="81eb7-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="81eb7-113">Delegated (work or school account)</span></span> | <span data-ttu-id="81eb7-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="81eb7-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="81eb7-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="81eb7-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="81eb7-116">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="81eb7-116">Files.ReadWrite</span></span>    |
|<span data-ttu-id="81eb7-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="81eb7-117">Application</span></span> | <span data-ttu-id="81eb7-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="81eb7-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="81eb7-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="81eb7-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names/{name}/Range

```
## <a name="request-headers"></a><span data-ttu-id="81eb7-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="81eb7-120">Request headers</span></span>
| <span data-ttu-id="81eb7-121">Nome</span><span class="sxs-lookup"><span data-stu-id="81eb7-121">Name</span></span>       | <span data-ttu-id="81eb7-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="81eb7-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="81eb7-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="81eb7-123">Authorization</span></span>  | <span data-ttu-id="81eb7-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="81eb7-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="81eb7-126">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="81eb7-126">Workbook-Session-Id</span></span>  | <span data-ttu-id="81eb7-p105">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="81eb7-p105">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="81eb7-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="81eb7-129">Request body</span></span>

## <a name="response"></a><span data-ttu-id="81eb7-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="81eb7-130">Response</span></span>

<span data-ttu-id="81eb7-131">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [workbookRange](../resources/workbookrange.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="81eb7-131">If successful, this method returns `200 OK` response code and [workbookRange](../resources/workbookrange.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="81eb7-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="81eb7-132">Example</span></span>
<span data-ttu-id="81eb7-133">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="81eb7-133">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="81eb7-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="81eb7-134">Request</span></span>
<span data-ttu-id="81eb7-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="81eb7-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="81eb7-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="81eb7-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "nameditem_range"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names/{name}/Range
```
# <a name="c"></a>[<span data-ttu-id="81eb7-137">C#</span><span class="sxs-lookup"><span data-stu-id="81eb7-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/nameditem-range-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="81eb7-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="81eb7-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/nameditem-range-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="81eb7-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="81eb7-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/nameditem-range-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="81eb7-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="81eb7-140">Response</span></span>
<span data-ttu-id="81eb7-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="81eb7-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "NamedItem: Range",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
