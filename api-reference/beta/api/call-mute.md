---
title: 'chamada: sem áudio'
description: Permite que o aplicativo se desative.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 40edbab3f97fd7a98a8687a0950c854fb7bf1f44
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35438689"
---
# <a name="call-mute"></a><span data-ttu-id="729fc-103">chamada: sem áudio</span><span class="sxs-lookup"><span data-stu-id="729fc-103">call: mute</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="729fc-104">Permite que o aplicativo se desative.</span><span class="sxs-lookup"><span data-stu-id="729fc-104">Allows the application to mute itself.</span></span>

## <a name="permissions"></a><span data-ttu-id="729fc-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="729fc-105">Permissions</span></span>
<span data-ttu-id="729fc-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="729fc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="729fc-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="729fc-108">Permission type</span></span>                        | <span data-ttu-id="729fc-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="729fc-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="729fc-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="729fc-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="729fc-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="729fc-111">Not Supported.</span></span>                               |
| <span data-ttu-id="729fc-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="729fc-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="729fc-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="729fc-113">Not Supported.</span></span>                               |
| <span data-ttu-id="729fc-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="729fc-114">Application</span></span>                            | <span data-ttu-id="729fc-115">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="729fc-115">None.</span></span>                                        |

## <a name="http-request"></a><span data-ttu-id="729fc-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="729fc-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/mute
POST /applications/{id}/calls/{id}/mute
```

## <a name="request-headers"></a><span data-ttu-id="729fc-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="729fc-117">Request headers</span></span>
| <span data-ttu-id="729fc-118">Nome</span><span class="sxs-lookup"><span data-stu-id="729fc-118">Name</span></span>          | <span data-ttu-id="729fc-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="729fc-119">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="729fc-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="729fc-120">Authorization</span></span> | <span data-ttu-id="729fc-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="729fc-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="729fc-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="729fc-123">Request body</span></span>
<span data-ttu-id="729fc-124">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="729fc-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="729fc-125">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="729fc-125">Parameter</span></span>      | <span data-ttu-id="729fc-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="729fc-126">Type</span></span>    |<span data-ttu-id="729fc-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="729fc-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="729fc-128">clientContext</span><span class="sxs-lookup"><span data-stu-id="729fc-128">clientContext</span></span>|<span data-ttu-id="729fc-129">String</span><span class="sxs-lookup"><span data-stu-id="729fc-129">String</span></span>|<span data-ttu-id="729fc-130">O contexto do cliente.</span><span class="sxs-lookup"><span data-stu-id="729fc-130">The client context.</span></span>|

## <a name="response"></a><span data-ttu-id="729fc-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="729fc-131">Response</span></span>
<span data-ttu-id="729fc-132">Se bem-sucedido, este método retorna `200 OK` um código de resposta e um objeto [commsOperation](../resources/commsoperation.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="729fc-132">If successful, this method returns `200 OK` response code and a [commsOperation](../resources/commsoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="729fc-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="729fc-133">Example</span></span>
<span data-ttu-id="729fc-134">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="729fc-134">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="729fc-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="729fc-135">Request</span></span>
<span data-ttu-id="729fc-136">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="729fc-136">The following example shows the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="729fc-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="729fc-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "call-mute"
}-->
```http
POST https://graph.microsoft.com/beta/app/calls/{id}/mute
Content-Type: application/json
Content-Length: 46

{
  "clientContext": "clientContext-value"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="729fc-138">C#</span><span class="sxs-lookup"><span data-stu-id="729fc-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-mute-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="729fc-139">Javascript</span><span class="sxs-lookup"><span data-stu-id="729fc-139">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-mute-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="729fc-140">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="729fc-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-mute-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="729fc-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="729fc-141">Response</span></span>

> <span data-ttu-id="729fc-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="729fc-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "description": "call: mute",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
