---
title: Obter compartilhamentos
description: Recupere uma lista de compartilhamentos de impressora.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 897c6b6acc8faed07564068d9a12d1d4193ef219
ms.sourcegitcommit: 5c3f4a3e2620d1d9e635e09231bbaa73cb0c3cdd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/14/2020
ms.locfileid: "46674482"
---
# <a name="list-shares"></a><span data-ttu-id="82883-103">Lista de compartilhamentos</span><span class="sxs-lookup"><span data-stu-id="82883-103">List shares</span></span>

<span data-ttu-id="82883-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="82883-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="82883-105">Recupere uma lista de **printerShares**.</span><span class="sxs-lookup"><span data-stu-id="82883-105">Retrieve a list of **printerShares**.</span></span>

## <a name="permissions"></a><span data-ttu-id="82883-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="82883-106">Permissions</span></span>
<span data-ttu-id="82883-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="82883-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="82883-109">Para usar o serviço de impressão universal, o usuário ou o locatário do aplicativo deve ter uma assinatura de impressão universal ativa, além das permissões listadas na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="82883-109">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, in addition to the permissions listed in the following table.</span></span>

|<span data-ttu-id="82883-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="82883-110">Permission type</span></span> | <span data-ttu-id="82883-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="82883-111">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="82883-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="82883-112">Delegated (work or school account)</span></span>| <span data-ttu-id="82883-113">PrinterShare. Read. All, PrinterShare. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="82883-113">PrinterShare.Read.All, PrinterShare.ReadWrite.All</span></span> |
|<span data-ttu-id="82883-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="82883-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="82883-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="82883-115">Not Supported.</span></span>|
|<span data-ttu-id="82883-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="82883-116">Application</span></span>|<span data-ttu-id="82883-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="82883-117">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="82883-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="82883-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/shares
```

## <a name="optional-query-parameters"></a><span data-ttu-id="82883-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="82883-119">Optional query parameters</span></span>
<span data-ttu-id="82883-120">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="82883-120">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="82883-121">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="82883-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

<span data-ttu-id="82883-122">Para ver uma lista de recursos de cada compartilhamento de impressora, inclua o `$select=capabilities` parâmetro de consulta opcional.</span><span class="sxs-lookup"><span data-stu-id="82883-122">To see a list of each printer share's capabilities, include the optional `$select=capabilities` query parameter.</span></span>

### <a name="exceptions"></a><span data-ttu-id="82883-123">Exceptions</span><span class="sxs-lookup"><span data-stu-id="82883-123">Exceptions</span></span>
<span data-ttu-id="82883-124">Não há suporte para alguns operadores: `$count` , `$orderby` , `$search` .</span><span class="sxs-lookup"><span data-stu-id="82883-124">Some operators are not supported: `$count`, `$orderby`, `$search`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="82883-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="82883-125">Request headers</span></span>
| <span data-ttu-id="82883-126">Nome</span><span class="sxs-lookup"><span data-stu-id="82883-126">Name</span></span>      |<span data-ttu-id="82883-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="82883-127">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="82883-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="82883-128">Authorization</span></span> | <span data-ttu-id="82883-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="82883-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="82883-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="82883-131">Request body</span></span>
<span data-ttu-id="82883-132">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="82883-132">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="82883-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="82883-133">Response</span></span>
<span data-ttu-id="82883-134">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [printerShare](../resources/printershare.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="82883-134">If successful, this method returns a `200 OK` response code and a collection of [printerShare](../resources/printershare.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="82883-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="82883-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="82883-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="82883-136">Request</span></span>
<span data-ttu-id="82883-137">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="82883-137">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="82883-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="82883-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_shares"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/shares
```
# <a name="c"></a>[<span data-ttu-id="82883-139">C#</span><span class="sxs-lookup"><span data-stu-id="82883-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-shares-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="82883-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="82883-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-shares-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="82883-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="82883-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-shares-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="82883-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="82883-142">Response</span></span>
<span data-ttu-id="82883-143">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="82883-143">The following is an example of the response.</span></span>
><span data-ttu-id="82883-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="82883-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printerShare",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 269

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#print/shares",
  "value": [
    {
      "id": "016b5565-3bbf-4067-b9ff-4d68167eb1a6",
      "name": "PrinterShareName",
      "createdDateTime": "2020-02-04T00:00:00.0000000Z"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List shares",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
