---
title: Listar trabalhos
description: Recupere uma lista de trabalhos de impressão associados à impressora.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 1f09e91c88e83127e86d441b2c6537d85729b4b6
ms.sourcegitcommit: 94c8985a3956622ea90f7e641f894d57b0982eb9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44251097"
---
# <a name="list-jobs"></a><span data-ttu-id="0adcd-103">Listar trabalhos</span><span class="sxs-lookup"><span data-stu-id="0adcd-103">List jobs</span></span>

<span data-ttu-id="0adcd-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0adcd-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0adcd-105">Recupere uma lista de trabalhos de impressão associados à [impressora](../resources/printer.md).</span><span class="sxs-lookup"><span data-stu-id="0adcd-105">Retrieve a list of print jobs associated with the [printer](../resources/printer.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="0adcd-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="0adcd-106">Permissions</span></span>
<span data-ttu-id="0adcd-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0adcd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="0adcd-109">Além das permissões a seguir, o locatário do usuário deve ter uma assinatura universal de impressão.</span><span class="sxs-lookup"><span data-stu-id="0adcd-109">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="0adcd-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0adcd-110">Permission type</span></span> | <span data-ttu-id="0adcd-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0adcd-111">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="0adcd-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0adcd-112">Delegated (work or school account)</span></span>| <span data-ttu-id="0adcd-113">Users. Read. All</span><span class="sxs-lookup"><span data-stu-id="0adcd-113">Users.Read.All</span></span> |
|<span data-ttu-id="0adcd-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0adcd-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0adcd-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0adcd-115">Not Supported.</span></span>|
|<span data-ttu-id="0adcd-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0adcd-116">Application</span></span>|<span data-ttu-id="0adcd-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0adcd-117">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0adcd-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0adcd-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/printers/{id}/jobs
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0adcd-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="0adcd-119">Optional query parameters</span></span>
<span data-ttu-id="0adcd-120">Este método oferece suporte a alguns dos parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="0adcd-120">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="0adcd-121">Para obter informações gerais, confira [parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="0adcd-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

### <a name="exceptions"></a><span data-ttu-id="0adcd-122">Exceções</span><span class="sxs-lookup"><span data-stu-id="0adcd-122">Exceptions</span></span>
<span data-ttu-id="0adcd-123">Não há suporte para alguns operadores: `$count` , `$search` , `$filter` .</span><span class="sxs-lookup"><span data-stu-id="0adcd-123">Some operators are not supported: `$count`, `$search`, `$filter`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0adcd-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0adcd-124">Request headers</span></span>
| <span data-ttu-id="0adcd-125">Nome</span><span class="sxs-lookup"><span data-stu-id="0adcd-125">Name</span></span>      |<span data-ttu-id="0adcd-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="0adcd-126">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="0adcd-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="0adcd-127">Authorization</span></span> | <span data-ttu-id="0adcd-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0adcd-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0adcd-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0adcd-130">Request body</span></span>
<span data-ttu-id="0adcd-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="0adcd-131">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="0adcd-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="0adcd-132">Response</span></span>
<span data-ttu-id="0adcd-133">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [printJob](../resources/printjob.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0adcd-133">If successful, this method returns a `200 OK` response code and collection of [printJob](../resources/printjob.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="0adcd-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0adcd-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0adcd-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0adcd-135">Request</span></span>
<span data-ttu-id="0adcd-136">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="0adcd-136">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="0adcd-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="0adcd-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_jobs"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/printers/{id}/jobs
```
# <a name="c"></a>[<span data-ttu-id="0adcd-138">C#</span><span class="sxs-lookup"><span data-stu-id="0adcd-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-jobs-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0adcd-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0adcd-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-jobs-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0adcd-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0adcd-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-jobs-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="0adcd-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="0adcd-141">Response</span></span>
<span data-ttu-id="0adcd-142">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="0adcd-142">The following is an example of the response.</span></span>
><span data-ttu-id="0adcd-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0adcd-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
