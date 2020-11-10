---
title: List taskTriggers
description: Recupere uma lista de disparadores de tarefas associados à impressora.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 22d4d9b27117159b93c3913c54c2be9debb9fafe
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48979813"
---
# <a name="list-tasktriggers"></a><span data-ttu-id="dd507-103">List taskTriggers</span><span class="sxs-lookup"><span data-stu-id="dd507-103">List taskTriggers</span></span>

<span data-ttu-id="dd507-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dd507-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dd507-105">Recupere uma lista de [disparadores de tarefas](../resources/printtasktrigger.md) associados à [impressora](../resources/printer.md).</span><span class="sxs-lookup"><span data-stu-id="dd507-105">Retrieve a list of [task triggers](../resources/printtasktrigger.md) associated with the [printer](../resources/printer.md).</span></span> <span data-ttu-id="dd507-106">A lista de disparadores de tarefa define quais tarefas serão disparadas como resultado de eventos que ocorrem durante a impressão.</span><span class="sxs-lookup"><span data-stu-id="dd507-106">The list of task triggers defines which tasks will be triggered as a result of events that occur during printing.</span></span>

<span data-ttu-id="dd507-107">Para obter detalhes sobre como usar essa API para adicionar suporte à impressão pull à impressão universal, consulte [Estendeing universal print to support pull Printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span><span class="sxs-lookup"><span data-stu-id="dd507-107">For details about how to use this API to add pull printing support to Universal Print, see [Extending Universal Print to support pull printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span></span>

## <a name="permissions"></a><span data-ttu-id="dd507-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="dd507-108">Permissions</span></span>
<span data-ttu-id="dd507-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dd507-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="dd507-111">Além das permissões a seguir, o locatário do usuário deve ter uma assinatura universal de impressão.</span><span class="sxs-lookup"><span data-stu-id="dd507-111">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span> <span data-ttu-id="dd507-112">O usuário conectado deve ser um [administrador da impressora](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span><span class="sxs-lookup"><span data-stu-id="dd507-112">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="dd507-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="dd507-113">Permission type</span></span> | <span data-ttu-id="dd507-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="dd507-114">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="dd507-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="dd507-115">Delegated (work or school account)</span></span>| <span data-ttu-id="dd507-116">Printer. Read. All, Printer. ReadWrite. All, Printer. FullControl. All</span><span class="sxs-lookup"><span data-stu-id="dd507-116">Printer.Read.All, Printer.ReadWrite.All, Printer.FullControl.All</span></span> |
|<span data-ttu-id="dd507-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="dd507-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dd507-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dd507-118">Not Supported.</span></span>|
|<span data-ttu-id="dd507-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="dd507-119">Application</span></span>| <span data-ttu-id="dd507-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dd507-120">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="dd507-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="dd507-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/printers/{id}/taskTriggers
```

## <a name="optional-query-parameters"></a><span data-ttu-id="dd507-122">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="dd507-122">Optional query parameters</span></span>
<span data-ttu-id="dd507-123">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="dd507-123">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="dd507-124">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="dd507-124">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

### <a name="exceptions"></a><span data-ttu-id="dd507-125">Exceptions</span><span class="sxs-lookup"><span data-stu-id="dd507-125">Exceptions</span></span>
<span data-ttu-id="dd507-126">Não há suporte para alguns operadores: `$count` ,,,, `$format` `$search` `$select` `$skip` , `$top` .</span><span class="sxs-lookup"><span data-stu-id="dd507-126">Some operators are not supported: `$count`, `$format`, `$search`, `$select`, `$skip`, `$top`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="dd507-127">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="dd507-127">Request headers</span></span>
| <span data-ttu-id="dd507-128">Nome</span><span class="sxs-lookup"><span data-stu-id="dd507-128">Name</span></span>      |<span data-ttu-id="dd507-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="dd507-129">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="dd507-130">Autorização</span><span class="sxs-lookup"><span data-stu-id="dd507-130">Authorization</span></span> | <span data-ttu-id="dd507-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dd507-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="dd507-133">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="dd507-133">Request body</span></span>
<span data-ttu-id="dd507-134">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="dd507-134">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="dd507-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="dd507-135">Response</span></span>
<span data-ttu-id="dd507-136">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [printTaskTrigger](../resources/printtasktrigger.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="dd507-136">If successful, this method returns a `200 OK` response code and collection of [printTaskTrigger](../resources/printtasktrigger.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="dd507-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="dd507-137">Example</span></span>
### <a name="request"></a><span data-ttu-id="dd507-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dd507-138">Request</span></span>
<span data-ttu-id="dd507-139">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="dd507-139">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="dd507-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="dd507-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_printer_tasktriggers"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/printers/{id}/taskTriggers
```
# <a name="c"></a>[<span data-ttu-id="dd507-141">C#</span><span class="sxs-lookup"><span data-stu-id="dd507-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-printer-tasktriggers-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="dd507-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="dd507-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-printer-tasktriggers-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="dd507-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="dd507-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-printer-tasktriggers-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="dd507-144">Java</span><span class="sxs-lookup"><span data-stu-id="dd507-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-printer-tasktriggers-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

### <a name="response"></a><span data-ttu-id="dd507-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="dd507-145">Response</span></span>
<span data-ttu-id="dd507-146">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="dd507-146">The following is an example of the response.</span></span>
><span data-ttu-id="dd507-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="dd507-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
