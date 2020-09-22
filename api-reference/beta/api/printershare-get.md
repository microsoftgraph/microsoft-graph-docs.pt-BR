---
title: Get printerShare
description: Recupere as propriedades e os relacionamentos de um compartilhamento de impressora.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: c34a3a0c0e425035d71108c98aed7c2aa75c3333
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48035509"
---
# <a name="get-printershare"></a><span data-ttu-id="0cbf0-103">Get printerShare</span><span class="sxs-lookup"><span data-stu-id="0cbf0-103">Get printerShare</span></span>

<span data-ttu-id="0cbf0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0cbf0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0cbf0-105">Recupere as propriedades e os relacionamentos de um compartilhamento de impressora.</span><span class="sxs-lookup"><span data-stu-id="0cbf0-105">Retrieve the properties and relationships of a printer share.</span></span>

## <a name="permissions"></a><span data-ttu-id="0cbf0-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="0cbf0-106">Permissions</span></span>
<span data-ttu-id="0cbf0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0cbf0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="0cbf0-109">Além das permissões a seguir, o usuário ou o locatário do aplicativo deve ter uma assinatura universal de impressão ativa.</span><span class="sxs-lookup"><span data-stu-id="0cbf0-109">In addition to the following permissions, the user or app's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="0cbf0-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0cbf0-110">Permission type</span></span> | <span data-ttu-id="0cbf0-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0cbf0-111">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="0cbf0-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0cbf0-112">Delegated (work or school account)</span></span>| <span data-ttu-id="0cbf0-113">PrinterShare. Read. All, PrinterShare. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="0cbf0-113">PrinterShare.Read.All, PrinterShare.ReadWrite.All</span></span> |
|<span data-ttu-id="0cbf0-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0cbf0-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0cbf0-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0cbf0-115">Not Supported.</span></span>|
|<span data-ttu-id="0cbf0-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0cbf0-116">Application</span></span>|<span data-ttu-id="0cbf0-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0cbf0-117">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0cbf0-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0cbf0-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/shares/{id}
GET /print/printers/{id}/share
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0cbf0-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="0cbf0-119">Optional query parameters</span></span>
<span data-ttu-id="0cbf0-120">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="0cbf0-120">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="0cbf0-121">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="0cbf0-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

### <a name="exceptions"></a><span data-ttu-id="0cbf0-122">Exceptions</span><span class="sxs-lookup"><span data-stu-id="0cbf0-122">Exceptions</span></span>
* <span data-ttu-id="0cbf0-123">`$count`Não há suporte para o operador.</span><span class="sxs-lookup"><span data-stu-id="0cbf0-123">The `$count` operator is not supported.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0cbf0-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0cbf0-124">Request headers</span></span>
| <span data-ttu-id="0cbf0-125">Nome</span><span class="sxs-lookup"><span data-stu-id="0cbf0-125">Name</span></span>      |<span data-ttu-id="0cbf0-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="0cbf0-126">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="0cbf0-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="0cbf0-127">Authorization</span></span> | <span data-ttu-id="0cbf0-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0cbf0-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0cbf0-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0cbf0-130">Request body</span></span>
<span data-ttu-id="0cbf0-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="0cbf0-131">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="0cbf0-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="0cbf0-132">Response</span></span>
<span data-ttu-id="0cbf0-133">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [printerShare](../resources/printershare.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0cbf0-133">If successful, this method returns a `200 OK` response code and a [printerShare](../resources/printershare.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="0cbf0-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0cbf0-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0cbf0-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0cbf0-135">Request</span></span>
<span data-ttu-id="0cbf0-136">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="0cbf0-136">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="0cbf0-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="0cbf0-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_printershare"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/shares/{id}
```
# <a name="c"></a>[<span data-ttu-id="0cbf0-138">C#</span><span class="sxs-lookup"><span data-stu-id="0cbf0-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-printershare-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0cbf0-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0cbf0-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-printershare-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0cbf0-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0cbf0-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-printershare-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="0cbf0-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="0cbf0-141">Response</span></span>
<span data-ttu-id="0cbf0-142">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="0cbf0-142">The following is an example of the response.</span></span>
><span data-ttu-id="0cbf0-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0cbf0-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printerShare"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 225

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#print/shares/$entity",
  "id": "d837c17b-3296-4384-a053-828d56e10f50",
  "name": "ShareName",
  "createdDateTime": "2020-02-04T00:00:00.0000000Z"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get printerShare",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


