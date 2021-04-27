---
title: Delete taskTrigger
description: Exclua o gatilho de tarefas de uma impressora.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: f98e73a7cf6d1da759ba933d685f72fbf11f2035
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52051085"
---
# <a name="delete-tasktrigger"></a><span data-ttu-id="78cdc-103">Delete taskTrigger</span><span class="sxs-lookup"><span data-stu-id="78cdc-103">Delete taskTrigger</span></span>

<span data-ttu-id="78cdc-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="78cdc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="78cdc-105">Exclua [o gatilho](../resources/printer.md)de tarefas de uma [impressora para](../resources/printtasktrigger.md) impedir que eventos de impressão relacionados acionem tarefas na impressora especificada.</span><span class="sxs-lookup"><span data-stu-id="78cdc-105">Delete a [printer](../resources/printer.md)'s [task trigger](../resources/printtasktrigger.md) to prevent related print events from triggering tasks on the specified printer.</span></span>

## <a name="permissions"></a><span data-ttu-id="78cdc-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="78cdc-106">Permissions</span></span>
<span data-ttu-id="78cdc-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="78cdc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="78cdc-109">Além das permissões a seguir, o locatário do usuário deve ter uma assinatura de Impressão Universal ativa.</span><span class="sxs-lookup"><span data-stu-id="78cdc-109">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="78cdc-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="78cdc-110">Permission type</span></span> | <span data-ttu-id="78cdc-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="78cdc-111">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="78cdc-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="78cdc-112">Delegated (work or school account)</span></span>| <span data-ttu-id="78cdc-113">Printer.ReadWrite.All, Printer.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="78cdc-113">Printer.ReadWrite.All, Printer.FullControl.All</span></span> |
|<span data-ttu-id="78cdc-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="78cdc-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="78cdc-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="78cdc-115">Not Supported.</span></span>|
|<span data-ttu-id="78cdc-116">Application</span><span class="sxs-lookup"><span data-stu-id="78cdc-116">Application</span></span>|<span data-ttu-id="78cdc-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="78cdc-117">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="78cdc-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="78cdc-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /print/printers/{id}/taskTriggers/{id}
```
## <a name="request-headers"></a><span data-ttu-id="78cdc-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="78cdc-119">Request headers</span></span>
| <span data-ttu-id="78cdc-120">Nome</span><span class="sxs-lookup"><span data-stu-id="78cdc-120">Name</span></span>          | <span data-ttu-id="78cdc-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="78cdc-121">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="78cdc-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="78cdc-122">Authorization</span></span> | <span data-ttu-id="78cdc-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="78cdc-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="78cdc-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="78cdc-125">Request body</span></span>
<span data-ttu-id="78cdc-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="78cdc-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="78cdc-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="78cdc-127">Response</span></span>
<span data-ttu-id="78cdc-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="78cdc-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="78cdc-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="78cdc-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="78cdc-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="78cdc-131">Request</span></span>
<span data-ttu-id="78cdc-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="78cdc-132">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="78cdc-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="78cdc-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_printer_tasktrigger"
}-->
```http
DELETE https://graph.microsoft.com/beta/print/printers/1a5f91a7-9bd1-4d5f-bb86-f43554cac51c/taskTriggers/25be207e-1154-491f-aa68-a9f7007d4bec
```
# <a name="c"></a>[<span data-ttu-id="78cdc-134">C#</span><span class="sxs-lookup"><span data-stu-id="78cdc-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-printer-tasktrigger-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="78cdc-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="78cdc-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-printer-tasktrigger-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="78cdc-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="78cdc-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-printer-tasktrigger-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="78cdc-137">Java</span><span class="sxs-lookup"><span data-stu-id="78cdc-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-printer-tasktrigger-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

##### <a name="response"></a><span data-ttu-id="78cdc-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="78cdc-138">Response</span></span>
<span data-ttu-id="78cdc-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="78cdc-139">The following is an example of the response.</span></span>
><span data-ttu-id="78cdc-140">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="78cdc-140">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete taskTrigger",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


