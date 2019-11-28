---
title: 'Call: updateMetadata'
description: Atualize os metadados da aplicação associados a uma chamada.
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: e681ebf65ebed550d4180788eb5d534723981463
ms.sourcegitcommit: fce7ce328f0c88c6310af9cc85d12bcebc88a6c3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/28/2019
ms.locfileid: "39636684"
---
# <a name="call-updatemetadata"></a><span data-ttu-id="20e6a-103">Call: updateMetadata</span><span class="sxs-lookup"><span data-stu-id="20e6a-103">call: updateMetadata</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="20e6a-104">Atualize os metadados da aplicação associados a uma chamada.</span><span class="sxs-lookup"><span data-stu-id="20e6a-104">Update the appliation's metadata associated with a call.</span></span>

## <a name="permissions"></a><span data-ttu-id="20e6a-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="20e6a-105">Permissions</span></span>
<span data-ttu-id="20e6a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="20e6a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="20e6a-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="20e6a-108">Permission type</span></span>                        | <span data-ttu-id="20e6a-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="20e6a-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="20e6a-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="20e6a-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="20e6a-111">Não suportado</span><span class="sxs-lookup"><span data-stu-id="20e6a-111">Not Supported</span></span>                               |
| <span data-ttu-id="20e6a-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="20e6a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="20e6a-113">Não suportado</span><span class="sxs-lookup"><span data-stu-id="20e6a-113">Not Supported</span></span>                               |
| <span data-ttu-id="20e6a-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="20e6a-114">Application</span></span>     | <span data-ttu-id="20e6a-115">Calls. JoinGroupCallsasGuest. All, calls. JoinGroupCalls. All, calls. InitiateGroupCalls. All</span><span class="sxs-lookup"><span data-stu-id="20e6a-115">Calls.JoinGroupCallsasGuest.All, Calls.JoinGroupCalls.All, Calls.InitiateGroupCalls.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="20e6a-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="20e6a-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/updateMetadata
POST /communications/calls/{id}/updateMetadata
```
> <span data-ttu-id="20e6a-117">**Observação:** o caminho `/app` foi preterido.</span><span class="sxs-lookup"><span data-stu-id="20e6a-117">**Note:** The `/app` path is deprecated.</span></span> <span data-ttu-id="20e6a-118">Daqui em diante, use o caminho `/communications`.</span><span class="sxs-lookup"><span data-stu-id="20e6a-118">Going forward, use the `/communications` path.</span></span>

## <a name="request-headers"></a><span data-ttu-id="20e6a-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="20e6a-119">Request headers</span></span>
| <span data-ttu-id="20e6a-120">Nome</span><span class="sxs-lookup"><span data-stu-id="20e6a-120">Name</span></span>          | <span data-ttu-id="20e6a-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="20e6a-121">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="20e6a-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="20e6a-122">Authorization</span></span> | <span data-ttu-id="20e6a-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="20e6a-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="20e6a-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="20e6a-125">Request body</span></span>
<span data-ttu-id="20e6a-126">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="20e6a-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="20e6a-127">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="20e6a-127">Parameter</span></span>      | <span data-ttu-id="20e6a-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="20e6a-128">Type</span></span>    |<span data-ttu-id="20e6a-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="20e6a-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="20e6a-130">los</span><span class="sxs-lookup"><span data-stu-id="20e6a-130">metadata</span></span>|<span data-ttu-id="20e6a-131">String</span><span class="sxs-lookup"><span data-stu-id="20e6a-131">String</span></span>|<span data-ttu-id="20e6a-132">Um blob de dados fornecido pelo participante na lista.</span><span class="sxs-lookup"><span data-stu-id="20e6a-132">A blob of data provided by the participant in the roster.</span></span>|
|<span data-ttu-id="20e6a-133">clientContext</span><span class="sxs-lookup"><span data-stu-id="20e6a-133">clientContext</span></span>|<span data-ttu-id="20e6a-134">String</span><span class="sxs-lookup"><span data-stu-id="20e6a-134">String</span></span>|<span data-ttu-id="20e6a-135">O contexto do cliente.</span><span class="sxs-lookup"><span data-stu-id="20e6a-135">The client context.</span></span>|

## <a name="response"></a><span data-ttu-id="20e6a-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="20e6a-136">Response</span></span>
<span data-ttu-id="20e6a-137">Retorna `202 Accepted` o código de resposta e um cabeçalho de local com um URI para o [commsOperation](../resources/commsoperation.md) criado para essa solicitação.</span><span class="sxs-lookup"><span data-stu-id="20e6a-137">Returns `202 Accepted` response code and a Location header with a uri to the [commsOperation](../resources/commsoperation.md) created for this request.</span></span>

## <a name="example"></a><span data-ttu-id="20e6a-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="20e6a-138">Example</span></span>
<span data-ttu-id="20e6a-139">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="20e6a-139">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="20e6a-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="20e6a-140">Request</span></span>
<span data-ttu-id="20e6a-141">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="20e6a-141">The following example shows the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="20e6a-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="20e6a-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "call-updateMetadata"
}-->
```http
POST https://graph.microsoft.com/beta/communications/calls/{id}/updateMetadata
Content-Type: application/json
Content-Length: 79

{
  "metadata": "metadata-value",
  "clientContext": "clientContext-value"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="20e6a-143">C#</span><span class="sxs-lookup"><span data-stu-id="20e6a-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-updatemetadata-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="20e6a-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="20e6a-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-updatemetadata-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="20e6a-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="20e6a-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-updatemetadata-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="20e6a-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="20e6a-146">Response</span></span>

> <span data-ttu-id="20e6a-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="20e6a-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "name": "call-updateMetadata",
  "truncated": true,
  "@odata.type": "microsoft.graph.commsOperation"
} -->
```http
HTTP/1.1 200 OK
Location: https://graph.microsoft.com/beta/communications/calls/57dab8b1-894c-409a-b240-bd8beae78896/operations/0fe0623f-d628-42ed-b4bd-8ac290072cc5

{
  "@odata.type": "#microsoft.graph.commsOperation",
  "clientContext": "clientContext-value",
  "id": "0fe0623f-d628-42ed-b4bd-8ac290072cc5",
  "resultInfo": null,
  "status": "completed"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "call: updateMetadata",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
