---
title: Delete taskTrigger
description: Excluir o gatilho de tarefa de uma impressora.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: c63dad5a4367eb7cf196cf5a6aaf6e1350eef70f
ms.sourcegitcommit: 496410c1e256aa093eabf27f17e820d9ee91a293
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2020
ms.locfileid: "46566323"
---
# <a name="delete-tasktrigger"></a><span data-ttu-id="3d01a-103">Delete taskTrigger</span><span class="sxs-lookup"><span data-stu-id="3d01a-103">Delete taskTrigger</span></span>

<span data-ttu-id="3d01a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3d01a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3d01a-105">Exclua o [disparador de tarefa](../resources/printtasktrigger.md) de uma [impressora](../resources/printer.md)para impedir que eventos de impressão relacionados disparem tarefas na impressora especificada.</span><span class="sxs-lookup"><span data-stu-id="3d01a-105">Delete a [printer](../resources/printer.md)'s [task trigger](../resources/printtasktrigger.md) to prevent related print events from triggering tasks on the specified printer.</span></span>

## <a name="permissions"></a><span data-ttu-id="3d01a-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="3d01a-106">Permissions</span></span>
<span data-ttu-id="3d01a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3d01a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="3d01a-109">Além das permissões a seguir, o locatário do usuário deve ter uma assinatura universal de impressão.</span><span class="sxs-lookup"><span data-stu-id="3d01a-109">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="3d01a-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3d01a-110">Permission type</span></span> | <span data-ttu-id="3d01a-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3d01a-111">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="3d01a-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3d01a-112">Delegated (work or school account)</span></span>| <span data-ttu-id="3d01a-113">Printer. ReadWrite. All, Printer. FullControl. All</span><span class="sxs-lookup"><span data-stu-id="3d01a-113">Printer.ReadWrite.All, Printer.FullControl.All</span></span> |
|<span data-ttu-id="3d01a-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3d01a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3d01a-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3d01a-115">Not Supported.</span></span>|
|<span data-ttu-id="3d01a-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3d01a-116">Application</span></span>|<span data-ttu-id="3d01a-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3d01a-117">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3d01a-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3d01a-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /print/printers/{id}/taskTriggers/{id}
```
## <a name="request-headers"></a><span data-ttu-id="3d01a-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3d01a-119">Request headers</span></span>
| <span data-ttu-id="3d01a-120">Nome</span><span class="sxs-lookup"><span data-stu-id="3d01a-120">Name</span></span>          | <span data-ttu-id="3d01a-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="3d01a-121">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="3d01a-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="3d01a-122">Authorization</span></span> | <span data-ttu-id="3d01a-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3d01a-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3d01a-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3d01a-125">Request body</span></span>
<span data-ttu-id="3d01a-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3d01a-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3d01a-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="3d01a-127">Response</span></span>
<span data-ttu-id="3d01a-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3d01a-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3d01a-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3d01a-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3d01a-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3d01a-131">Request</span></span>
<span data-ttu-id="3d01a-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="3d01a-132">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="3d01a-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="3d01a-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_printer_tasktrigger"
}-->
```http
DELETE https://graph.microsoft.com/beta/print/printers/1a5f91a7-9bd1-4d5f-bb86-f43554cac51c/taskTriggers/25be207e-1154-491f-aa68-a9f7007d4bec
```
# <a name="c"></a>[<span data-ttu-id="3d01a-134">C#</span><span class="sxs-lookup"><span data-stu-id="3d01a-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-printer-tasktrigger-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3d01a-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3d01a-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-printer-tasktrigger-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3d01a-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3d01a-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-printer-tasktrigger-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

##### <a name="response"></a><span data-ttu-id="3d01a-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="3d01a-137">Response</span></span>
<span data-ttu-id="3d01a-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="3d01a-138">The following is an example of the response.</span></span>
><span data-ttu-id="3d01a-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3d01a-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
