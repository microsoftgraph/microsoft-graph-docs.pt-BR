---
title: Excluir taskTrigger
description: Excluir o gatilho de tarefa de uma impressora.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: c96edf3379e1d20e35070e4e131ffb08cce98d5f
ms.sourcegitcommit: 8a74c06be9c41390331ca1717efedc5b5a244db5
ms.translationtype: Auto
ms.contentlocale: pt-BR
ms.lasthandoff: 07/09/2020
ms.locfileid: "45091554"
---
# <a name="delete-tasktrigger"></a><span data-ttu-id="1e339-103">Excluir taskTrigger</span><span class="sxs-lookup"><span data-stu-id="1e339-103">Delete taskTrigger</span></span>

<span data-ttu-id="1e339-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1e339-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1e339-105">Exclua o [disparador de tarefa](../resources/printtasktrigger.md) de uma [impressora](../resources/printer.md)para impedir que eventos de impressão relacionados disparem tarefas na impressora especificada.</span><span class="sxs-lookup"><span data-stu-id="1e339-105">Delete a [printer](../resources/printer.md)'s [task trigger](../resources/printtasktrigger.md) to prevent related print events from triggering tasks on the specified printer.</span></span>

## <a name="permissions"></a><span data-ttu-id="1e339-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="1e339-106">Permissions</span></span>
<span data-ttu-id="1e339-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1e339-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="1e339-109">Além das permissões a seguir, o locatário do usuário deve ter uma assinatura universal de impressão.</span><span class="sxs-lookup"><span data-stu-id="1e339-109">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="1e339-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1e339-110">Permission type</span></span> | <span data-ttu-id="1e339-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1e339-111">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="1e339-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1e339-112">Delegated (work or school account)</span></span>| <span data-ttu-id="1e339-113">Printer. ReadWrite. All, Printer. FullControl. All</span><span class="sxs-lookup"><span data-stu-id="1e339-113">Printer.ReadWrite.All, Printer.FullControl.All</span></span> |
|<span data-ttu-id="1e339-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1e339-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1e339-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1e339-115">Not Supported.</span></span>|
|<span data-ttu-id="1e339-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1e339-116">Application</span></span>|<span data-ttu-id="1e339-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1e339-117">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1e339-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1e339-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /print/printers/{id}/taskTriggers/{id}
```
## <a name="request-headers"></a><span data-ttu-id="1e339-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1e339-119">Request headers</span></span>
| <span data-ttu-id="1e339-120">Nome</span><span class="sxs-lookup"><span data-stu-id="1e339-120">Name</span></span>          | <span data-ttu-id="1e339-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="1e339-121">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="1e339-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="1e339-122">Authorization</span></span> | <span data-ttu-id="1e339-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1e339-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1e339-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1e339-125">Request body</span></span>
<span data-ttu-id="1e339-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1e339-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1e339-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="1e339-127">Response</span></span>
<span data-ttu-id="1e339-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1e339-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1e339-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1e339-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1e339-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1e339-131">Request</span></span>
<span data-ttu-id="1e339-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="1e339-132">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_printer_tasktrigger"
}-->
```http
DELETE https://graph.microsoft.com/beta/print/printers/1a5f91a7-9bd1-4d5f-bb86-f43554cac51c/taskTriggers/25be207e-1154-491f-aa68-a9f7007d4bec
```

---

##### <a name="response"></a><span data-ttu-id="1e339-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="1e339-133">Response</span></span>
<span data-ttu-id="1e339-134">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="1e339-134">The following is an example of the response.</span></span>
><span data-ttu-id="1e339-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1e339-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
