---
title: 'NamedItem: Range'
description: Retorna o objeto Range associado ao nome. Gera uma exceção quando o tipo de item nomeado não é um intervalo.
localization_priority: Normal
ms.openlocfilehash: a77a34659540dbfbea101a1a88e258d5ad20a5fb
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35460655"
---
# <a name="nameditem-range"></a><span data-ttu-id="2fa5c-104">NamedItem: Range</span><span class="sxs-lookup"><span data-stu-id="2fa5c-104">NamedItem: Range</span></span>

<span data-ttu-id="2fa5c-p102">Retorna o objeto Range associado ao nome. Gera uma exceção quando o tipo de item nomeado não é um intervalo.</span><span class="sxs-lookup"><span data-stu-id="2fa5c-p102">Returns the range object that is associated with the name. Throws an exception if the named item's type is not a range.</span></span>
## <a name="permissions"></a><span data-ttu-id="2fa5c-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="2fa5c-107">Permissions</span></span>
<span data-ttu-id="2fa5c-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2fa5c-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2fa5c-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2fa5c-110">Permission type</span></span>      | <span data-ttu-id="2fa5c-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2fa5c-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2fa5c-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2fa5c-112">Delegated (work or school account)</span></span> | <span data-ttu-id="2fa5c-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2fa5c-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="2fa5c-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2fa5c-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2fa5c-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2fa5c-115">Not supported.</span></span>    |
|<span data-ttu-id="2fa5c-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2fa5c-116">Application</span></span> | <span data-ttu-id="2fa5c-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2fa5c-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="2fa5c-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2fa5c-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names/{name}/range

```
## <a name="request-headers"></a><span data-ttu-id="2fa5c-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2fa5c-119">Request headers</span></span>
| <span data-ttu-id="2fa5c-120">Nome</span><span class="sxs-lookup"><span data-stu-id="2fa5c-120">Name</span></span>       | <span data-ttu-id="2fa5c-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="2fa5c-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="2fa5c-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="2fa5c-122">Authorization</span></span>  | <span data-ttu-id="2fa5c-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2fa5c-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="2fa5c-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="2fa5c-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="2fa5c-p105">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="2fa5c-p105">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="2fa5c-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2fa5c-128">Request body</span></span>

## <a name="response"></a><span data-ttu-id="2fa5c-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="2fa5c-129">Response</span></span>

<span data-ttu-id="2fa5c-130">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [Range](../resources/range.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2fa5c-130">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2fa5c-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2fa5c-131">Example</span></span>
<span data-ttu-id="2fa5c-132">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="2fa5c-132">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="2fa5c-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2fa5c-133">Request</span></span>
<span data-ttu-id="2fa5c-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2fa5c-134">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="2fa5c-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="2fa5c-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "idempotent": true,
  "name": "nameditem_range"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="2fa5c-136">C#</span><span class="sxs-lookup"><span data-stu-id="2fa5c-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/nameditem-range-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="2fa5c-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="2fa5c-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/nameditem-range-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="2fa5c-138">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="2fa5c-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/nameditem-range-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="2fa5c-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="2fa5c-139">Response</span></span>
<span data-ttu-id="2fa5c-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2fa5c-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "NamedItem: Range",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
