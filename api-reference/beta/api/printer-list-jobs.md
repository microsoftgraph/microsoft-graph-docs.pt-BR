---
title: Listar trabalhos
description: Recupere uma lista de trabalhos de impressão associados à impressora.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 2f0f539f902bd1b83c8efd046af35b0deb28ed05
ms.sourcegitcommit: e20c113409836115f338dcfe3162342ef3bd6a4a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/01/2020
ms.locfileid: "45006699"
---
# <a name="list-jobs"></a><span data-ttu-id="f920c-103">Listar trabalhos</span><span class="sxs-lookup"><span data-stu-id="f920c-103">List jobs</span></span>

<span data-ttu-id="f920c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f920c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f920c-105">Recupere uma lista de trabalhos de impressão associados à [impressora](../resources/printer.md).</span><span class="sxs-lookup"><span data-stu-id="f920c-105">Retrieve a list of print jobs associated with the [printer](../resources/printer.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="f920c-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="f920c-106">Permissions</span></span>
<span data-ttu-id="f920c-107">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="f920c-107">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="f920c-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f920c-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="f920c-109">Para usar o serviço de impressão universal, o usuário ou o locatário do aplicativo deve ter uma assinatura universal de impressão ativa, uma permissão que conceda obter acesso à [impressora](printer-get.md) e uma das permissões listadas na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="f920c-109">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, a permission that grants [Get printer](printer-get.md) access, and one of the permissions listed in the following table.</span></span>

|<span data-ttu-id="f920c-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f920c-110">Permission type</span></span> | <span data-ttu-id="f920c-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f920c-111">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="f920c-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f920c-112">Delegated (work or school account)</span></span>| <span data-ttu-id="f920c-113">Users. Read. All</span><span class="sxs-lookup"><span data-stu-id="f920c-113">Users.Read.All</span></span> |
|<span data-ttu-id="f920c-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f920c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f920c-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f920c-115">Not Supported.</span></span>|
|<span data-ttu-id="f920c-116">Application</span><span class="sxs-lookup"><span data-stu-id="f920c-116">Application</span></span>| <span data-ttu-id="f920c-117">PrintJob. ReadBasic. All, PrintJob. Read. All, PrintJob. ReadWriteBasic. All, PrintJob. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="f920c-117">PrintJob.ReadBasic.All, PrintJob.Read.All, PrintJob.ReadWriteBasic.All, PrintJob.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f920c-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f920c-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/printers/{id}/jobs
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f920c-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="f920c-119">Optional query parameters</span></span>
<span data-ttu-id="f920c-120">Este método oferece suporte a alguns dos parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="f920c-120">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="f920c-121">Para obter informações gerais, confira [parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="f920c-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

### <a name="exceptions"></a><span data-ttu-id="f920c-122">Exceptions</span><span class="sxs-lookup"><span data-stu-id="f920c-122">Exceptions</span></span>
<span data-ttu-id="f920c-123">Não há suporte para alguns operadores: `$count` , `$search` , `$filter` .</span><span class="sxs-lookup"><span data-stu-id="f920c-123">Some operators are not supported: `$count`, `$search`, `$filter`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f920c-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f920c-124">Request headers</span></span>
| <span data-ttu-id="f920c-125">Nome</span><span class="sxs-lookup"><span data-stu-id="f920c-125">Name</span></span>      |<span data-ttu-id="f920c-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="f920c-126">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="f920c-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="f920c-127">Authorization</span></span> | <span data-ttu-id="f920c-128">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="f920c-128">Bearer {token}.</span></span> <span data-ttu-id="f920c-129">Required.</span><span class="sxs-lookup"><span data-stu-id="f920c-129">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f920c-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f920c-130">Request body</span></span>
<span data-ttu-id="f920c-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f920c-131">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="f920c-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="f920c-132">Response</span></span>
<span data-ttu-id="f920c-133">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [printJob](../resources/printjob.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f920c-133">If successful, this method returns a `200 OK` response code and collection of [printJob](../resources/printjob.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f920c-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f920c-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f920c-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f920c-135">Request</span></span>
<span data-ttu-id="f920c-136">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="f920c-136">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="f920c-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="f920c-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_jobs"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/printers/{id}/jobs
```
# <a name="c"></a>[<span data-ttu-id="f920c-138">C#</span><span class="sxs-lookup"><span data-stu-id="f920c-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-jobs-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f920c-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f920c-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-jobs-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f920c-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f920c-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-jobs-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="f920c-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="f920c-141">Response</span></span>
<span data-ttu-id="f920c-142">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="f920c-142">The following is an example of the response.</span></span>
><span data-ttu-id="f920c-143">**Note:** The response object shown here might be shortened for readability.</span><span class="sxs-lookup"><span data-stu-id="f920c-143">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="f920c-144">All the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="f920c-144">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printJob",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 461

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#print/printers('c05f3726-0d4b-4aa1-8fe9-2eb981bb26fb')/jobs",
  "value": [
    {
      "id": "5182",
      "createdDateTime": "2020-02-04T00:00:00.0000000Z",
      "createdBy": {},
      "status": {
        "processingState": "completed",
        "processingStateDescription": "The print job has completed successfully and no further processing will take place."
      }
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List jobs",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
