---
title: 'impressora: resetDefaults'
description: Redefinir as configurações padrão de uma impressora.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: d3e2f28e15d12e2a332f995b5b6d8d3e94856228
ms.sourcegitcommit: 33ffed5b785abf36b1a7786856c9266958830d25
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/25/2020
ms.locfileid: "42947747"
---
# <a name="printer-resetdefaults"></a><span data-ttu-id="b0780-103">impressora: resetDefaults</span><span class="sxs-lookup"><span data-stu-id="b0780-103">printer: resetDefaults</span></span>

<span data-ttu-id="b0780-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b0780-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b0780-105">Redefinir as configurações padrão de uma [impressora](../resources/printer.md).</span><span class="sxs-lookup"><span data-stu-id="b0780-105">Reset a [printer](../resources/printer.md)'s default settings.</span></span>

## <a name="permissions"></a><span data-ttu-id="b0780-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="b0780-106">Permissions</span></span>
<span data-ttu-id="b0780-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b0780-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="b0780-109">Além das permissões a seguir, o locatário do usuário deve ter uma assinatura universal de impressão.</span><span class="sxs-lookup"><span data-stu-id="b0780-109">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="b0780-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b0780-110">Permission type</span></span> | <span data-ttu-id="b0780-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b0780-111">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="b0780-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b0780-112">Delegated (work or school account)</span></span>| <span data-ttu-id="b0780-113">Users. Read. All</span><span class="sxs-lookup"><span data-stu-id="b0780-113">Users.Read.All</span></span> |
|<span data-ttu-id="b0780-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b0780-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b0780-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b0780-115">Not Supported.</span></span>|
|<span data-ttu-id="b0780-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b0780-116">Application</span></span>|<span data-ttu-id="b0780-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b0780-117">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b0780-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b0780-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /print/printers/{id}/resetDefaults
```
## <a name="request-headers"></a><span data-ttu-id="b0780-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b0780-119">Request headers</span></span>
| <span data-ttu-id="b0780-120">Nome</span><span class="sxs-lookup"><span data-stu-id="b0780-120">Name</span></span>          | <span data-ttu-id="b0780-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="b0780-121">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="b0780-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="b0780-122">Authorization</span></span> | <span data-ttu-id="b0780-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b0780-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b0780-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b0780-125">Request body</span></span>

## <a name="response"></a><span data-ttu-id="b0780-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="b0780-126">Response</span></span>
<span data-ttu-id="b0780-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b0780-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b0780-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b0780-129">Example</span></span>
<span data-ttu-id="b0780-130">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="b0780-130">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="b0780-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b0780-131">Request</span></span>
<span data-ttu-id="b0780-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="b0780-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b0780-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="b0780-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "printer-resetdefaults"
}-->
```http
POST https://graph.microsoft.com/beta/print/printers/{id}/resetDefaults
```
# <a name="c"></a>[<span data-ttu-id="b0780-134">C#</span><span class="sxs-lookup"><span data-stu-id="b0780-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/printer-resetdefaults-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b0780-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b0780-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/printer-resetdefaults-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b0780-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b0780-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/printer-resetdefaults-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="b0780-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="b0780-137">Response</span></span>
<span data-ttu-id="b0780-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="b0780-138">The following is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "printer: resetDefaults",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
