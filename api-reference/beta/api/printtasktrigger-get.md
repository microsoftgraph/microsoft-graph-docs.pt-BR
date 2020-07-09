---
title: Obter taskTrigger
description: Obter um gatilho de tarefa de uma impressora.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: aeb7d5481a550ac3e9223023aaef92ed009eb85e
ms.sourcegitcommit: 8a74c06be9c41390331ca1717efedc5b5a244db5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/09/2020
ms.locfileid: "45091536"
---
# <a name="get-tasktrigger"></a><span data-ttu-id="88444-103">Obter taskTrigger</span><span class="sxs-lookup"><span data-stu-id="88444-103">Get taskTrigger</span></span>

<span data-ttu-id="88444-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="88444-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="88444-105">Obter um [gatilho de tarefa](../resources/printtasktrigger.md) de uma [impressora](../resources/printer.md).</span><span class="sxs-lookup"><span data-stu-id="88444-105">Get a [task trigger](../resources/printtasktrigger.md) from a [printer](../resources/printer.md).</span></span>

<span data-ttu-id="88444-106">Para obter detalhes sobre como usar essa API para adicionar suporte à impressão pull à impressão universal, consulte [Estendeing universal print to support pull Printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span><span class="sxs-lookup"><span data-stu-id="88444-106">For details about how to use this API to add pull printing support to Universal Print, see [Extending Universal Print to support pull printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span></span>

## <a name="permissions"></a><span data-ttu-id="88444-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="88444-107">Permissions</span></span>
<span data-ttu-id="88444-108">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="88444-108">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="88444-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="88444-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="88444-110">Além das permissões a seguir, o locatário do usuário deve ter uma assinatura universal de impressão.</span><span class="sxs-lookup"><span data-stu-id="88444-110">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="88444-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="88444-111">Permission type</span></span> | <span data-ttu-id="88444-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="88444-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="88444-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="88444-113">Delegated (work or school account)</span></span>| <span data-ttu-id="88444-114">Printer. Read. All, Printer. ReadWrite. All, Printer. FullControl. All</span><span class="sxs-lookup"><span data-stu-id="88444-114">Printer.Read.All, Printer.ReadWrite.All, Printer.FullControl.All</span></span> |
|<span data-ttu-id="88444-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="88444-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="88444-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="88444-116">Not Supported.</span></span>|
|<span data-ttu-id="88444-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="88444-117">Application</span></span>|<span data-ttu-id="88444-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="88444-118">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="88444-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="88444-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/printers/{id}/taskTriggers/{id}
```

## <a name="request-headers"></a><span data-ttu-id="88444-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="88444-120">Request headers</span></span>
| <span data-ttu-id="88444-121">Nome</span><span class="sxs-lookup"><span data-stu-id="88444-121">Name</span></span>      |<span data-ttu-id="88444-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="88444-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="88444-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="88444-123">Authorization</span></span> | <span data-ttu-id="88444-124">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="88444-124">Bearer {token}.</span></span> <span data-ttu-id="88444-125">Required.</span><span class="sxs-lookup"><span data-stu-id="88444-125">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="88444-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="88444-126">Request body</span></span>
<span data-ttu-id="88444-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="88444-127">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="88444-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="88444-128">Response</span></span>
<span data-ttu-id="88444-129">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [printTaskTrigger](../resources/printtasktrigger.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="88444-129">If successful, this method returns a `200 OK` response code and [printTaskTrigger](../resources/printtasktrigger.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="88444-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="88444-130">Example</span></span>
### <a name="request"></a><span data-ttu-id="88444-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="88444-131">Request</span></span>
<span data-ttu-id="88444-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="88444-132">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_printer_tasktrigger"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/printers/{printerId}/taskTriggers/{taskTriggerId}
```

---

### <a name="response"></a><span data-ttu-id="88444-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="88444-133">Response</span></span>
<span data-ttu-id="88444-134">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="88444-134">The following is an example of the response.</span></span>
><span data-ttu-id="88444-135">**Note:** The response object shown here might be shortened for readability.</span><span class="sxs-lookup"><span data-stu-id="88444-135">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="88444-136">All the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="88444-136">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printTaskTrigger"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 181

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#print/printers/taskTriggers/$entity",
  "id": "b6a843ca-e60e-4e20-a222-a58d85eead6d",
  "event": "jobStarted"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get taskTrigger",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
