---
title: 'chamada: ativar mudo'
description: Permite que o aplicativo se desative sozinho.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 161daadfc42213ed5b15c0de4e80e2f722ef8115
ms.sourcegitcommit: c68a83d28fa4bfca6e0618467934813a9ae17b12
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/07/2019
ms.locfileid: "36792531"
---
# <a name="call-unmute"></a><span data-ttu-id="8dd79-103">chamada: ativar mudo</span><span class="sxs-lookup"><span data-stu-id="8dd79-103">call: unmute</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8dd79-104">Permite que o aplicativo se desative sozinho.</span><span class="sxs-lookup"><span data-stu-id="8dd79-104">Allows the application to unmute itself.</span></span>

## <a name="permissions"></a><span data-ttu-id="8dd79-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="8dd79-105">Permissions</span></span>
<span data-ttu-id="8dd79-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8dd79-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8dd79-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8dd79-108">Permission type</span></span>                        | <span data-ttu-id="8dd79-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8dd79-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="8dd79-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8dd79-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="8dd79-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8dd79-111">Not supported.</span></span>                               |
| <span data-ttu-id="8dd79-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8dd79-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8dd79-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8dd79-113">Not supported.</span></span>                               |
| <span data-ttu-id="8dd79-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8dd79-114">Application</span></span>                            | <span data-ttu-id="8dd79-115">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="8dd79-115">None.</span></span>                                        |

## <a name="http-request"></a><span data-ttu-id="8dd79-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8dd79-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/unmute
```

## <a name="request-headers"></a><span data-ttu-id="8dd79-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8dd79-117">Request headers</span></span>
| <span data-ttu-id="8dd79-118">Nome</span><span class="sxs-lookup"><span data-stu-id="8dd79-118">Name</span></span>          | <span data-ttu-id="8dd79-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="8dd79-119">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="8dd79-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="8dd79-120">Authorization</span></span> | <span data-ttu-id="8dd79-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8dd79-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8dd79-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8dd79-123">Request body</span></span>
<span data-ttu-id="8dd79-124">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8dd79-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="8dd79-125">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="8dd79-125">Parameter</span></span>      | <span data-ttu-id="8dd79-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="8dd79-126">Type</span></span>    |<span data-ttu-id="8dd79-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="8dd79-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8dd79-128">clientContext</span><span class="sxs-lookup"><span data-stu-id="8dd79-128">clientContext</span></span>|<span data-ttu-id="8dd79-129">String</span><span class="sxs-lookup"><span data-stu-id="8dd79-129">String</span></span>|<span data-ttu-id="8dd79-130">O contexto do cliente.</span><span class="sxs-lookup"><span data-stu-id="8dd79-130">The client context.</span></span>|

## <a name="response"></a><span data-ttu-id="8dd79-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="8dd79-131">Response</span></span>
<span data-ttu-id="8dd79-132">Se bem-sucedido, este método retorna `200 OK` o código de resposta e o objeto [commsOperation](../resources/commsoperation.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8dd79-132">If successful, this method returns `200 OK` response code and [commsOperation](../resources/commsoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8dd79-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8dd79-133">Example</span></span>
<span data-ttu-id="8dd79-134">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="8dd79-134">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="8dd79-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8dd79-135">Request</span></span>
<span data-ttu-id="8dd79-136">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="8dd79-136">The following example shows the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="8dd79-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="8dd79-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "call-unmute"
}-->
```http
POST https://graph.microsoft.com/beta/app/calls/{id}/unmute
Content-Type: application/json
Content-Length: 46

{
  "clientContext": "clientContext-value"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="8dd79-138">C#</span><span class="sxs-lookup"><span data-stu-id="8dd79-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-unmute-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8dd79-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8dd79-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-unmute-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="8dd79-140">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="8dd79-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-unmute-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="8dd79-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="8dd79-141">Response</span></span>

> <span data-ttu-id="8dd79-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8dd79-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.commsOperation"
} -->
```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 259

{
  "id": "17e3b46c-f61d-4f4d-9635-c626ef18e6ad",
  "status": "completed",
  "createdDateTime": "2018-09-06T15:58:41Z",
  "lastActionDateTime": "2018-09-06T15:58:41Z",
  "clientContext": "d45324c1-fcb5-430a-902c-f20af696537c"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "call: unmute",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
