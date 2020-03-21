---
title: Obter printJob
description: Recupere as propriedades e os relacionamentos de um trabalho de impressão.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 011ba76e161d01ab3d168840163e8cb4f7a3a240
ms.sourcegitcommit: 7baf4847486885edf08ead533c76503cd31a98a4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/21/2020
ms.locfileid: "42895540"
---
# <a name="get-printjob"></a><span data-ttu-id="31d3b-103">Obter printJob</span><span class="sxs-lookup"><span data-stu-id="31d3b-103">Get printJob</span></span>

<span data-ttu-id="31d3b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="31d3b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="31d3b-105">Recupere as propriedades e os relacionamentos de um trabalho de impressão.</span><span class="sxs-lookup"><span data-stu-id="31d3b-105">Retrieve the properties and relationships of a print job.</span></span>

## <a name="permissions"></a><span data-ttu-id="31d3b-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="31d3b-106">Permissions</span></span>
<span data-ttu-id="31d3b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="31d3b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="31d3b-109">Além das permissões a seguir, o locatário do usuário deve ter uma assinatura universal de impressão.</span><span class="sxs-lookup"><span data-stu-id="31d3b-109">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="31d3b-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="31d3b-110">Permission type</span></span> | <span data-ttu-id="31d3b-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="31d3b-111">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="31d3b-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="31d3b-112">Delegated (work or school account)</span></span>| <span data-ttu-id="31d3b-113">Users. Read. All</span><span class="sxs-lookup"><span data-stu-id="31d3b-113">Users.Read.All</span></span> |
|<span data-ttu-id="31d3b-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="31d3b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="31d3b-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="31d3b-115">Not Supported.</span></span>|
|<span data-ttu-id="31d3b-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="31d3b-116">Application</span></span>|<span data-ttu-id="31d3b-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="31d3b-117">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="31d3b-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="31d3b-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/printers/{id}/jobs/{id}
```

## <a name="request-headers"></a><span data-ttu-id="31d3b-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="31d3b-119">Request headers</span></span>
| <span data-ttu-id="31d3b-120">Nome</span><span class="sxs-lookup"><span data-stu-id="31d3b-120">Name</span></span>      |<span data-ttu-id="31d3b-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="31d3b-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="31d3b-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="31d3b-122">Authorization</span></span> | <span data-ttu-id="31d3b-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="31d3b-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="31d3b-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="31d3b-125">Request body</span></span>
<span data-ttu-id="31d3b-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="31d3b-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="31d3b-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="31d3b-127">Response</span></span>
<span data-ttu-id="31d3b-128">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [printJob](../resources/printjob.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="31d3b-128">If successful, this method returns a `200 OK` response code and a [printJob](../resources/printjob.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="31d3b-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="31d3b-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="31d3b-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="31d3b-130">Request</span></span>
<span data-ttu-id="31d3b-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="31d3b-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_printjob"
}-->
```http
GET https://graph.microsoft.com/beta/print/printers/{id}/jobs/{id}
```
##### <a name="response"></a><span data-ttu-id="31d3b-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="31d3b-132">Response</span></span>
<span data-ttu-id="31d3b-133">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="31d3b-133">The following is an example of the response.</span></span>
><span data-ttu-id="31d3b-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="31d3b-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printJob"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 408

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#print/printers('c05f3726-0d4b-4aa1-8fe9-2eb981bb26fb')/jobs/$entity",
  "id": "5182",
  "createdDateTime": "2020-02-04T00:00:00.0000000Z",
  "createdBy": {},
  "status": {
    "processingState": "completed",
    "processingStateDescription": "The print job has completed successfully and no further processing will take place."
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get printJob",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->