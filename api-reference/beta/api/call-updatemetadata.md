---
title: 'Call: updateMetadata'
description: Atualize os metadados da aplicação associados a uma chamada.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: fa2b92118b6a1e0862044427dd73a2a0d2bf3a35
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35864652"
---
# <a name="call-updatemetadata"></a><span data-ttu-id="2a4c9-103">Call: updateMetadata</span><span class="sxs-lookup"><span data-stu-id="2a4c9-103">call: updateMetadata</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2a4c9-104">Atualize os metadados da aplicação associados a uma chamada.</span><span class="sxs-lookup"><span data-stu-id="2a4c9-104">Update the appliation's metadata associated with a call.</span></span>

## <a name="permissions"></a><span data-ttu-id="2a4c9-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="2a4c9-105">Permissions</span></span>
<span data-ttu-id="2a4c9-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2a4c9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2a4c9-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2a4c9-108">Permission type</span></span>                        | <span data-ttu-id="2a4c9-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2a4c9-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="2a4c9-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2a4c9-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="2a4c9-111">Não suportado</span><span class="sxs-lookup"><span data-stu-id="2a4c9-111">Not Supported</span></span>                               |
| <span data-ttu-id="2a4c9-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2a4c9-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2a4c9-113">Não suportado</span><span class="sxs-lookup"><span data-stu-id="2a4c9-113">Not Supported</span></span>                               |
| <span data-ttu-id="2a4c9-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2a4c9-114">Application</span></span>     | <span data-ttu-id="2a4c9-115">Calls. JoinGroupCallsasGuest. All, calls. JoinGroupCalls. All, calls. InitiateGroupCalls. All</span><span class="sxs-lookup"><span data-stu-id="2a4c9-115">Calls.JoinGroupCallsasGuest.All, Calls.JoinGroupCalls.All, Calls.InitiateGroupCalls.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2a4c9-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2a4c9-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/updateMetadata
POST /applications/{id}/calls/{id}/updateMetadata
```

## <a name="request-headers"></a><span data-ttu-id="2a4c9-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2a4c9-117">Request headers</span></span>
| <span data-ttu-id="2a4c9-118">Nome</span><span class="sxs-lookup"><span data-stu-id="2a4c9-118">Name</span></span>          | <span data-ttu-id="2a4c9-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="2a4c9-119">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="2a4c9-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="2a4c9-120">Authorization</span></span> | <span data-ttu-id="2a4c9-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2a4c9-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2a4c9-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2a4c9-123">Request body</span></span>
<span data-ttu-id="2a4c9-124">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2a4c9-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="2a4c9-125">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="2a4c9-125">Parameter</span></span>      | <span data-ttu-id="2a4c9-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="2a4c9-126">Type</span></span>    |<span data-ttu-id="2a4c9-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="2a4c9-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2a4c9-128">los</span><span class="sxs-lookup"><span data-stu-id="2a4c9-128">metadata</span></span>|<span data-ttu-id="2a4c9-129">String</span><span class="sxs-lookup"><span data-stu-id="2a4c9-129">String</span></span>|<span data-ttu-id="2a4c9-130">Um blob de dados fornecido pelo participante na lista.</span><span class="sxs-lookup"><span data-stu-id="2a4c9-130">A blob of data provided by the participant in the roster.</span></span>|
|<span data-ttu-id="2a4c9-131">clientContext</span><span class="sxs-lookup"><span data-stu-id="2a4c9-131">clientContext</span></span>|<span data-ttu-id="2a4c9-132">String</span><span class="sxs-lookup"><span data-stu-id="2a4c9-132">String</span></span>|<span data-ttu-id="2a4c9-133">O contexto do cliente.</span><span class="sxs-lookup"><span data-stu-id="2a4c9-133">The client context.</span></span>|

## <a name="response"></a><span data-ttu-id="2a4c9-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="2a4c9-134">Response</span></span>
<span data-ttu-id="2a4c9-135">Retorna `202 Accepted` o código de resposta e um cabeçalho de local com um URI para o [commsOperation](../resources/commsoperation.md) criado para essa solicitação.</span><span class="sxs-lookup"><span data-stu-id="2a4c9-135">Returns `202 Accepted` response code and a Location header with a uri to the [commsOperation](../resources/commsoperation.md) created for this request.</span></span>

## <a name="example"></a><span data-ttu-id="2a4c9-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2a4c9-136">Example</span></span>
<span data-ttu-id="2a4c9-137">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="2a4c9-137">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="2a4c9-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2a4c9-138">Request</span></span>
<span data-ttu-id="2a4c9-139">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="2a4c9-139">The following example shows the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="2a4c9-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="2a4c9-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "call-updateMetadata"
}-->
```http
POST https://graph.microsoft.com/beta/app/calls/{id}/updateMetadata
Content-Type: application/json
Content-Length: 79

{
  "metadata": "metadata-value",
  "clientContext": "clientContext-value"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="2a4c9-141">C#</span><span class="sxs-lookup"><span data-stu-id="2a4c9-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-updatemetadata-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="2a4c9-142">Javascript</span><span class="sxs-lookup"><span data-stu-id="2a4c9-142">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-updatemetadata-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="2a4c9-143">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="2a4c9-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-updatemetadata-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="2a4c9-144">Java</span><span class="sxs-lookup"><span data-stu-id="2a4c9-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/call-updatemetadata-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="2a4c9-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="2a4c9-145">Response</span></span>

> <span data-ttu-id="2a4c9-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2a4c9-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.commsOperation"
} -->
```http
HTTP/1.1 202 Accepted
Location: https://graph.microsoft.com/beta/app/calls/57dab8b1-894c-409a-b240-bd8beae78896/operations/0fe0623f-d628-42ed-b4bd-8ac290072cc5
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
