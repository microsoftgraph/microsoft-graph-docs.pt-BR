---
title: Obter printerShare
description: Recupere as propriedades e os relacionamentos de um compartilhamento de impressora.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: c7799d4b712323cf2ad1b40ba2bd6ded7158dbfd
ms.sourcegitcommit: 7baf4847486885edf08ead533c76503cd31a98a4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/21/2020
ms.locfileid: "42895545"
---
# <a name="get-printershare"></a><span data-ttu-id="6a692-103">Obter printerShare</span><span class="sxs-lookup"><span data-stu-id="6a692-103">Get printerShare</span></span>

<span data-ttu-id="6a692-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6a692-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6a692-105">Recupere as propriedades e os relacionamentos de um compartilhamento de impressora.</span><span class="sxs-lookup"><span data-stu-id="6a692-105">Retrieve the properties and relationships of a printer share.</span></span>

## <a name="permissions"></a><span data-ttu-id="6a692-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="6a692-106">Permissions</span></span>
<span data-ttu-id="6a692-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6a692-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="6a692-109">Além das permissões a seguir, o locatário do usuário deve ter uma assinatura universal de impressão.</span><span class="sxs-lookup"><span data-stu-id="6a692-109">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="6a692-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6a692-110">Permission type</span></span> | <span data-ttu-id="6a692-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6a692-111">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="6a692-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6a692-112">Delegated (work or school account)</span></span>| <span data-ttu-id="6a692-113">Users. Read. All</span><span class="sxs-lookup"><span data-stu-id="6a692-113">Users.Read.All</span></span> |
|<span data-ttu-id="6a692-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6a692-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6a692-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6a692-115">Not Supported.</span></span>|
|<span data-ttu-id="6a692-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6a692-116">Application</span></span>|<span data-ttu-id="6a692-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6a692-117">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6a692-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6a692-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/printerShares/{id}
GET /print/printers/{id}/share
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6a692-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="6a692-119">Optional query parameters</span></span>
<span data-ttu-id="6a692-120">Este método oferece suporte a alguns dos parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="6a692-120">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="6a692-121">Para obter informações gerais, confira [parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="6a692-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

### <a name="exceptions"></a><span data-ttu-id="6a692-122">Exceções</span><span class="sxs-lookup"><span data-stu-id="6a692-122">Exceptions</span></span>
* <span data-ttu-id="6a692-123">Não `$count` há suporte para o operador.</span><span class="sxs-lookup"><span data-stu-id="6a692-123">The `$count` operator is not supported.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6a692-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6a692-124">Request headers</span></span>
| <span data-ttu-id="6a692-125">Nome</span><span class="sxs-lookup"><span data-stu-id="6a692-125">Name</span></span>      |<span data-ttu-id="6a692-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="6a692-126">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="6a692-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="6a692-127">Authorization</span></span> | <span data-ttu-id="6a692-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6a692-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6a692-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6a692-130">Request body</span></span>
<span data-ttu-id="6a692-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="6a692-131">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="6a692-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="6a692-132">Response</span></span>
<span data-ttu-id="6a692-133">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [printerShare](../resources/printershare.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6a692-133">If successful, this method returns a `200 OK` response code and a [printerShare](../resources/printershare.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="6a692-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6a692-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6a692-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6a692-135">Request</span></span>
<span data-ttu-id="6a692-136">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="6a692-136">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_printershare"
}-->
```http
GET https://graph.microsoft.com/beta/print/printerShares/{id}
```
##### <a name="response"></a><span data-ttu-id="6a692-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="6a692-137">Response</span></span>
<span data-ttu-id="6a692-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="6a692-138">The following is an example of the response.</span></span>
><span data-ttu-id="6a692-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6a692-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#print/printerShares/$entity",
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