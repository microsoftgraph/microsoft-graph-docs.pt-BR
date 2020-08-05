---
title: List taskTriggers
description: Recupere uma lista de disparadores de tarefas associados à impressora.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 189830fb76de676163a24a8166cff6017cceffc5
ms.sourcegitcommit: 496410c1e256aa093eabf27f17e820d9ee91a293
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2020
ms.locfileid: "46565889"
---
# <a name="list-tasktriggers"></a><span data-ttu-id="61a3d-103">List taskTriggers</span><span class="sxs-lookup"><span data-stu-id="61a3d-103">List taskTriggers</span></span>

<span data-ttu-id="61a3d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="61a3d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="61a3d-105">Recupere uma lista de [disparadores de tarefas](../resources/printtasktrigger.md) associados à [impressora](../resources/printer.md).</span><span class="sxs-lookup"><span data-stu-id="61a3d-105">Retrieve a list of [task triggers](../resources/printtasktrigger.md) associated with the [printer](../resources/printer.md).</span></span> <span data-ttu-id="61a3d-106">A lista de disparadores de tarefa define quais tarefas serão disparadas como resultado de eventos que ocorrem durante a impressão.</span><span class="sxs-lookup"><span data-stu-id="61a3d-106">The list of task triggers defines which tasks will be triggered as a result of events that occur during printing.</span></span>

<span data-ttu-id="61a3d-107">Para obter detalhes sobre como usar essa API para adicionar suporte à impressão pull à impressão universal, consulte [Estendeing universal print to support pull Printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span><span class="sxs-lookup"><span data-stu-id="61a3d-107">For details about how to use this API to add pull printing support to Universal Print, see [Extending Universal Print to support pull printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span></span>

## <a name="permissions"></a><span data-ttu-id="61a3d-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="61a3d-108">Permissions</span></span>
<span data-ttu-id="61a3d-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="61a3d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="61a3d-111">Além das permissões a seguir, o locatário do usuário deve ter uma assinatura universal de impressão.</span><span class="sxs-lookup"><span data-stu-id="61a3d-111">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="61a3d-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="61a3d-112">Permission type</span></span> | <span data-ttu-id="61a3d-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="61a3d-113">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="61a3d-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="61a3d-114">Delegated (work or school account)</span></span>| <span data-ttu-id="61a3d-115">Printer. Read. All, Printer. ReadWrite. All, Printer. FullControl. All</span><span class="sxs-lookup"><span data-stu-id="61a3d-115">Printer.Read.All, Printer.ReadWrite.All, Printer.FullControl.All</span></span> |
|<span data-ttu-id="61a3d-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="61a3d-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="61a3d-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="61a3d-117">Not Supported.</span></span>|
|<span data-ttu-id="61a3d-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="61a3d-118">Application</span></span>| <span data-ttu-id="61a3d-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="61a3d-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="61a3d-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="61a3d-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/printers/{id}/taskTriggers
```

## <a name="optional-query-parameters"></a><span data-ttu-id="61a3d-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="61a3d-121">Optional query parameters</span></span>
<span data-ttu-id="61a3d-122">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="61a3d-122">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="61a3d-123">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="61a3d-123">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

### <a name="exceptions"></a><span data-ttu-id="61a3d-124">Exceptions</span><span class="sxs-lookup"><span data-stu-id="61a3d-124">Exceptions</span></span>
<span data-ttu-id="61a3d-125">Não há suporte para alguns operadores: `$count` ,,,, `$format` `$search` `$select` `$skip` , `$top` .</span><span class="sxs-lookup"><span data-stu-id="61a3d-125">Some operators are not supported: `$count`, `$format`, `$search`, `$select`, `$skip`, `$top`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="61a3d-126">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="61a3d-126">Request headers</span></span>
| <span data-ttu-id="61a3d-127">Nome</span><span class="sxs-lookup"><span data-stu-id="61a3d-127">Name</span></span>      |<span data-ttu-id="61a3d-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="61a3d-128">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="61a3d-129">Autorização</span><span class="sxs-lookup"><span data-stu-id="61a3d-129">Authorization</span></span> | <span data-ttu-id="61a3d-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="61a3d-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="61a3d-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="61a3d-132">Request body</span></span>
<span data-ttu-id="61a3d-133">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="61a3d-133">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="61a3d-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="61a3d-134">Response</span></span>
<span data-ttu-id="61a3d-135">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [printTaskTrigger](../resources/printtasktrigger.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="61a3d-135">If successful, this method returns a `200 OK` response code and collection of [printTaskTrigger](../resources/printtasktrigger.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="61a3d-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="61a3d-136">Example</span></span>
### <a name="request"></a><span data-ttu-id="61a3d-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="61a3d-137">Request</span></span>
<span data-ttu-id="61a3d-138">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="61a3d-138">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="61a3d-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="61a3d-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_printer_tasktriggers"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/printers/{id}/taskTriggers
```
# <a name="c"></a>[<span data-ttu-id="61a3d-140">C#</span><span class="sxs-lookup"><span data-stu-id="61a3d-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-printer-tasktriggers-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="61a3d-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="61a3d-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-printer-tasktriggers-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="61a3d-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="61a3d-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-printer-tasktriggers-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

### <a name="response"></a><span data-ttu-id="61a3d-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="61a3d-143">Response</span></span>
<span data-ttu-id="61a3d-144">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="61a3d-144">The following is an example of the response.</span></span>
><span data-ttu-id="61a3d-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="61a3d-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printTaskTrigger",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 254

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#print/printers('fcc7fe6a-5ba7-4059-8017-702f3a41c8a4')/taskTriggers",
  "value": [
    {
      "id": "b6a843ca-e60e-4e20-a222-a58d85eead6d",
      "event": "jobStarted"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List taskTriggers",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
