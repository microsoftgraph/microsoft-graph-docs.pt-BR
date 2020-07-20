---
title: Listar taskTriggers
description: Recupere uma lista de disparadores de tarefas associados à impressora.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 1278e84070bc78c6fb0ead350bd464e8a102ea98
ms.sourcegitcommit: 8a74c06be9c41390331ca1717efedc5b5a244db5
ms.translationtype: Auto
ms.contentlocale: pt-BR
ms.lasthandoff: 07/09/2020
ms.locfileid: "45091551"
---
# <a name="list-tasktriggers"></a><span data-ttu-id="64eb2-103">Listar taskTriggers</span><span class="sxs-lookup"><span data-stu-id="64eb2-103">List taskTriggers</span></span>

<span data-ttu-id="64eb2-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="64eb2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="64eb2-105">Recupere uma lista de [disparadores de tarefas](../resources/printtasktrigger.md) associados à [impressora](../resources/printer.md).</span><span class="sxs-lookup"><span data-stu-id="64eb2-105">Retrieve a list of [task triggers](../resources/printtasktrigger.md) associated with the [printer](../resources/printer.md).</span></span> <span data-ttu-id="64eb2-106">A lista de disparadores de tarefa define quais tarefas serão disparadas como resultado de eventos que ocorrem durante a impressão.</span><span class="sxs-lookup"><span data-stu-id="64eb2-106">The list of task triggers defines which tasks will be triggered as a result of events that occur during printing.</span></span>

<span data-ttu-id="64eb2-107">Para obter detalhes sobre como usar essa API para adicionar suporte à impressão pull à impressão universal, consulte [Estendeing universal print to support pull Printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span><span class="sxs-lookup"><span data-stu-id="64eb2-107">For details about how to use this API to add pull printing support to Universal Print, see [Extending Universal Print to support pull printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span></span>

## <a name="permissions"></a><span data-ttu-id="64eb2-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="64eb2-108">Permissions</span></span>
<span data-ttu-id="64eb2-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="64eb2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="64eb2-111">Além das permissões a seguir, o locatário do usuário deve ter uma assinatura universal de impressão.</span><span class="sxs-lookup"><span data-stu-id="64eb2-111">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="64eb2-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="64eb2-112">Permission type</span></span> | <span data-ttu-id="64eb2-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="64eb2-113">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="64eb2-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="64eb2-114">Delegated (work or school account)</span></span>| <span data-ttu-id="64eb2-115">Printer. Read. All, Printer. ReadWrite. All, Printer. FullControl. All</span><span class="sxs-lookup"><span data-stu-id="64eb2-115">Printer.Read.All, Printer.ReadWrite.All, Printer.FullControl.All</span></span> |
|<span data-ttu-id="64eb2-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="64eb2-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="64eb2-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="64eb2-117">Not Supported.</span></span>|
|<span data-ttu-id="64eb2-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="64eb2-118">Application</span></span>| <span data-ttu-id="64eb2-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="64eb2-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="64eb2-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="64eb2-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/printers/{id}/taskTriggers
```

## <a name="optional-query-parameters"></a><span data-ttu-id="64eb2-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="64eb2-121">Optional query parameters</span></span>
<span data-ttu-id="64eb2-122">Este método oferece suporte a alguns dos parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="64eb2-122">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="64eb2-123">Para obter informações gerais, confira [parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="64eb2-123">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

### <a name="exceptions"></a><span data-ttu-id="64eb2-124">Exceptions</span><span class="sxs-lookup"><span data-stu-id="64eb2-124">Exceptions</span></span>
<span data-ttu-id="64eb2-125">Não há suporte para alguns operadores: `$count` ,,,, `$format` `$search` `$select` `$skip` , `$top` .</span><span class="sxs-lookup"><span data-stu-id="64eb2-125">Some operators are not supported: `$count`, `$format`, `$search`, `$select`, `$skip`, `$top`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="64eb2-126">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="64eb2-126">Request headers</span></span>
| <span data-ttu-id="64eb2-127">Nome</span><span class="sxs-lookup"><span data-stu-id="64eb2-127">Name</span></span>      |<span data-ttu-id="64eb2-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="64eb2-128">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="64eb2-129">Autorização</span><span class="sxs-lookup"><span data-stu-id="64eb2-129">Authorization</span></span> | <span data-ttu-id="64eb2-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="64eb2-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="64eb2-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="64eb2-132">Request body</span></span>
<span data-ttu-id="64eb2-133">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="64eb2-133">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="64eb2-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="64eb2-134">Response</span></span>
<span data-ttu-id="64eb2-135">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [printTaskTrigger](../resources/printtasktrigger.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="64eb2-135">If successful, this method returns a `200 OK` response code and collection of [printTaskTrigger](../resources/printtasktrigger.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="64eb2-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="64eb2-136">Example</span></span>
### <a name="request"></a><span data-ttu-id="64eb2-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="64eb2-137">Request</span></span>
<span data-ttu-id="64eb2-138">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="64eb2-138">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_printer_tasktriggers"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/printers/{id}/taskTriggers
```

---

### <a name="response"></a><span data-ttu-id="64eb2-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="64eb2-139">Response</span></span>
<span data-ttu-id="64eb2-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="64eb2-140">The following is an example of the response.</span></span>
><span data-ttu-id="64eb2-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="64eb2-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
