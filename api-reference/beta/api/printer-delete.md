---
title: Eliminar impressora
description: Excluir (não registro) uma impressora.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: d31efb889442ded8f8bfa48e8674279602a16024
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52051078"
---
# <a name="delete-printer"></a><span data-ttu-id="81fcb-103">Eliminar impressora</span><span class="sxs-lookup"><span data-stu-id="81fcb-103">Delete printer</span></span>

<span data-ttu-id="81fcb-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="81fcb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="81fcb-105">Excluir (não registro) uma [impressora](../resources/printer.md).</span><span class="sxs-lookup"><span data-stu-id="81fcb-105">Delete (unregister) a [printer](../resources/printer.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="81fcb-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="81fcb-106">Permissions</span></span>
<span data-ttu-id="81fcb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="81fcb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="81fcb-109">Para usar o serviço Impressão Universal, o usuário ou locatário do aplicativo deve ter uma assinatura de Impressão Universal ativa, além das permissões listadas na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="81fcb-109">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, in addition to the permissions listed in the following table.</span></span> <span data-ttu-id="81fcb-110">O usuário inscreveu deve ser um [Administrador de Impressora.](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)</span><span class="sxs-lookup"><span data-stu-id="81fcb-110">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="81fcb-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="81fcb-111">Permission type</span></span> | <span data-ttu-id="81fcb-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="81fcb-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="81fcb-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="81fcb-113">Delegated (work or school account)</span></span>| <span data-ttu-id="81fcb-114">Printer.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="81fcb-114">Printer.FullControl.All</span></span> |
|<span data-ttu-id="81fcb-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="81fcb-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="81fcb-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="81fcb-116">Not Supported.</span></span>|
|<span data-ttu-id="81fcb-117">Application</span><span class="sxs-lookup"><span data-stu-id="81fcb-117">Application</span></span>|<span data-ttu-id="81fcb-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="81fcb-118">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="81fcb-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="81fcb-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /print/printers/{id}
```
## <a name="request-headers"></a><span data-ttu-id="81fcb-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="81fcb-120">Request headers</span></span>
| <span data-ttu-id="81fcb-121">Nome</span><span class="sxs-lookup"><span data-stu-id="81fcb-121">Name</span></span>          | <span data-ttu-id="81fcb-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="81fcb-122">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="81fcb-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="81fcb-123">Authorization</span></span> | <span data-ttu-id="81fcb-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="81fcb-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="81fcb-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="81fcb-126">Request body</span></span>
<span data-ttu-id="81fcb-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="81fcb-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="81fcb-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="81fcb-128">Response</span></span>
<span data-ttu-id="81fcb-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="81fcb-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="81fcb-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="81fcb-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="81fcb-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="81fcb-132">Request</span></span>
<span data-ttu-id="81fcb-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="81fcb-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="81fcb-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="81fcb-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_printer"
}-->
```http
DELETE https://graph.microsoft.com/beta/print/printers/{id}
```
# <a name="c"></a>[<span data-ttu-id="81fcb-135">C#</span><span class="sxs-lookup"><span data-stu-id="81fcb-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-printer-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="81fcb-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="81fcb-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-printer-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="81fcb-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="81fcb-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-printer-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="81fcb-138">Java</span><span class="sxs-lookup"><span data-stu-id="81fcb-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-printer-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="81fcb-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="81fcb-139">Response</span></span>
<span data-ttu-id="81fcb-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="81fcb-140">The following is an example of the response.</span></span>
><span data-ttu-id="81fcb-141">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="81fcb-141">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete printer",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
