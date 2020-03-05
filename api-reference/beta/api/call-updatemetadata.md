---
title: 'Call: updateMetadata'
description: Atualize os metadados da aplicação associados a uma chamada.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 793639bed1288dd6873a6f2b4afba53efba9e533
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42440700"
---
# <a name="call-updatemetadata"></a><span data-ttu-id="967ff-103">Call: updateMetadata</span><span class="sxs-lookup"><span data-stu-id="967ff-103">call: updateMetadata</span></span>

<span data-ttu-id="967ff-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="967ff-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="967ff-105">Atualize os metadados da aplicação associados a uma chamada.</span><span class="sxs-lookup"><span data-stu-id="967ff-105">Update the appliation's metadata associated with a call.</span></span>

## <a name="permissions"></a><span data-ttu-id="967ff-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="967ff-106">Permissions</span></span>
<span data-ttu-id="967ff-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="967ff-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="967ff-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="967ff-109">Permission type</span></span>                        | <span data-ttu-id="967ff-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="967ff-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="967ff-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="967ff-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="967ff-112">Não suportado</span><span class="sxs-lookup"><span data-stu-id="967ff-112">Not Supported</span></span>                               |
| <span data-ttu-id="967ff-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="967ff-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="967ff-114">Não suportado</span><span class="sxs-lookup"><span data-stu-id="967ff-114">Not Supported</span></span>                               |
| <span data-ttu-id="967ff-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="967ff-115">Application</span></span>     | <span data-ttu-id="967ff-116">Calls. JoinGroupCallsasGuest. All, calls. JoinGroupCalls. All, calls. InitiateGroupCalls. All</span><span class="sxs-lookup"><span data-stu-id="967ff-116">Calls.JoinGroupCallsasGuest.All, Calls.JoinGroupCalls.All, Calls.InitiateGroupCalls.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="967ff-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="967ff-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/updateMetadata
POST /communications/calls/{id}/updateMetadata
```
> <span data-ttu-id="967ff-118">**Observação:** o caminho `/app` foi preterido.</span><span class="sxs-lookup"><span data-stu-id="967ff-118">**Note:** The `/app` path is deprecated.</span></span> <span data-ttu-id="967ff-119">Daqui em diante, use o caminho `/communications`.</span><span class="sxs-lookup"><span data-stu-id="967ff-119">Going forward, use the `/communications` path.</span></span>

## <a name="request-headers"></a><span data-ttu-id="967ff-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="967ff-120">Request headers</span></span>
| <span data-ttu-id="967ff-121">Nome</span><span class="sxs-lookup"><span data-stu-id="967ff-121">Name</span></span>          | <span data-ttu-id="967ff-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="967ff-122">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="967ff-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="967ff-123">Authorization</span></span> | <span data-ttu-id="967ff-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="967ff-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="967ff-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="967ff-126">Request body</span></span>
<span data-ttu-id="967ff-127">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="967ff-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="967ff-128">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="967ff-128">Parameter</span></span>      | <span data-ttu-id="967ff-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="967ff-129">Type</span></span>    |<span data-ttu-id="967ff-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="967ff-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="967ff-131">los</span><span class="sxs-lookup"><span data-stu-id="967ff-131">metadata</span></span>|<span data-ttu-id="967ff-132">String</span><span class="sxs-lookup"><span data-stu-id="967ff-132">String</span></span>|<span data-ttu-id="967ff-133">Um blob de dados fornecido pelo participante na lista.</span><span class="sxs-lookup"><span data-stu-id="967ff-133">A blob of data provided by the participant in the roster.</span></span>|
|<span data-ttu-id="967ff-134">clientContext</span><span class="sxs-lookup"><span data-stu-id="967ff-134">clientContext</span></span>|<span data-ttu-id="967ff-135">String</span><span class="sxs-lookup"><span data-stu-id="967ff-135">String</span></span>|<span data-ttu-id="967ff-136">O contexto do cliente.</span><span class="sxs-lookup"><span data-stu-id="967ff-136">The client context.</span></span>|

## <a name="response"></a><span data-ttu-id="967ff-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="967ff-137">Response</span></span>
<span data-ttu-id="967ff-138">Retorna `202 Accepted` o código de resposta e um cabeçalho de local com um URI para o [commsOperation](../resources/commsoperation.md) criado para essa solicitação.</span><span class="sxs-lookup"><span data-stu-id="967ff-138">Returns `202 Accepted` response code and a Location header with a uri to the [commsOperation](../resources/commsoperation.md) created for this request.</span></span>

## <a name="example"></a><span data-ttu-id="967ff-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="967ff-139">Example</span></span>
<span data-ttu-id="967ff-140">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="967ff-140">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="967ff-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="967ff-141">Request</span></span>
<span data-ttu-id="967ff-142">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="967ff-142">The following example shows the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="967ff-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="967ff-143">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="967ff-144">C#</span><span class="sxs-lookup"><span data-stu-id="967ff-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-updatemetadata-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="967ff-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="967ff-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-updatemetadata-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="967ff-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="967ff-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-updatemetadata-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="967ff-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="967ff-147">Response</span></span>

> <span data-ttu-id="967ff-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="967ff-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
