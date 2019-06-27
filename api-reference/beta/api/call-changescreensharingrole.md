---
title: 'Call: changeScreenSharingRole'
description: Inicie e interrompa a tela de compartilhamento na chamada. Essa API é usada para permitir que os aplicativos compartilhem conteúdo de tela com os participantes de uma chamada ou reunião.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 87a2c56810d80af8f38e0a3b7ae84b5c6f787e22
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35262318"
---
# <a name="call-changescreensharingrole"></a><span data-ttu-id="b8196-104">Call: changeScreenSharingRole</span><span class="sxs-lookup"><span data-stu-id="b8196-104">call: changeScreenSharingRole</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b8196-105">Inicie e interrompa a tela de compartilhamento na chamada.</span><span class="sxs-lookup"><span data-stu-id="b8196-105">Start and stop sharing screen in the call.</span></span> <span data-ttu-id="b8196-106">Essa API é usada para permitir que os aplicativos compartilhem conteúdo de tela com os participantes de uma chamada ou reunião.</span><span class="sxs-lookup"><span data-stu-id="b8196-106">This API is used to allow applications to share screen content with the participants of a call or meeting.</span></span>

## <a name="permissions"></a><span data-ttu-id="b8196-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="b8196-107">Permissions</span></span>
<span data-ttu-id="b8196-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b8196-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b8196-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b8196-110">Permission type</span></span>                        | <span data-ttu-id="b8196-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b8196-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="b8196-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b8196-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="b8196-113">Não suportado</span><span class="sxs-lookup"><span data-stu-id="b8196-113">Not Supported</span></span>                               |
| <span data-ttu-id="b8196-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b8196-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b8196-115">Não suportado</span><span class="sxs-lookup"><span data-stu-id="b8196-115">Not Supported</span></span>                               |
| <span data-ttu-id="b8196-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b8196-116">Application</span></span>                            | <span data-ttu-id="b8196-117">Calls.AccessMedia.All</span><span class="sxs-lookup"><span data-stu-id="b8196-117">Calls.AccessMedia.All</span></span>                       |

## <a name="http-request"></a><span data-ttu-id="b8196-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b8196-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/changeScreenSharingRole
POST /applications/{id}/calls/{id}/changeScreenSharingRole
```

## <a name="request-headers"></a><span data-ttu-id="b8196-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b8196-119">Request headers</span></span>
| <span data-ttu-id="b8196-120">Nome</span><span class="sxs-lookup"><span data-stu-id="b8196-120">Name</span></span>          | <span data-ttu-id="b8196-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="b8196-121">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="b8196-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="b8196-122">Authorization</span></span> | <span data-ttu-id="b8196-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b8196-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b8196-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b8196-125">Request body</span></span>
<span data-ttu-id="b8196-126">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b8196-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="b8196-127">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="b8196-127">Parameter</span></span>      | <span data-ttu-id="b8196-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="b8196-128">Type</span></span>    |<span data-ttu-id="b8196-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="b8196-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b8196-130">role</span><span class="sxs-lookup"><span data-stu-id="b8196-130">role</span></span>|<span data-ttu-id="b8196-131">String</span><span class="sxs-lookup"><span data-stu-id="b8196-131">String</span></span>|<span data-ttu-id="b8196-132">Os valores possíveis são: ' Visualizador ', ' participante '</span><span class="sxs-lookup"><span data-stu-id="b8196-132">Possible values are: 'Viewer', 'Sharer'</span></span>|

## <a name="response"></a><span data-ttu-id="b8196-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="b8196-133">Response</span></span>
<span data-ttu-id="b8196-134">Retorna `202 Accepted` o código de resposta.</span><span class="sxs-lookup"><span data-stu-id="b8196-134">Returns `202 Accepted` response code.</span></span>

## <a name="example"></a><span data-ttu-id="b8196-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b8196-135">Example</span></span>
<span data-ttu-id="b8196-136">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="b8196-136">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="b8196-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b8196-137">Request</span></span>
<span data-ttu-id="b8196-138">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="b8196-138">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "call-changeScreenSharingRole"
}-->
```http
POST https://graph.microsoft.com/beta/app/calls/{id}/changeScreenSharingRole
Content-Type: application/json
Content-Length: 24

{
  "role": "viewer"
}
```

##### <a name="response"></a><span data-ttu-id="b8196-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="b8196-139">Response</span></span>
<span data-ttu-id="b8196-140">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b8196-140">Here is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 202 Accepted
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="b8196-141">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="b8196-141">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="b8196-142">C#</span><span class="sxs-lookup"><span data-stu-id="b8196-142">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/call-changeScreenSharingRole-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b8196-143">Javascript</span><span class="sxs-lookup"><span data-stu-id="b8196-143">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/call-changeScreenSharingRole-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="b8196-144">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="b8196-144">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/call-changeScreenSharingRole-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "call: changeScreenSharingRole",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/call-changescreensharingrole.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/call-changescreensharingrole.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/call-changescreensharingrole.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
