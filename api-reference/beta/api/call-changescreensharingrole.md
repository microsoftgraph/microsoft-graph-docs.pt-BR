---
title: 'Call: changeScreenSharingRole'
description: Inicie e interrompa a tela de compartilhamento na chamada. Essa API é usada para permitir que os aplicativos compartilhem conteúdo de tela com os participantes de uma chamada ou reunião.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 75d423e54309853d2fd6b39043a14e5bd5926daf
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35864839"
---
# <a name="call-changescreensharingrole"></a><span data-ttu-id="7875f-104">Call: changeScreenSharingRole</span><span class="sxs-lookup"><span data-stu-id="7875f-104">call: changeScreenSharingRole</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7875f-105">Inicie e interrompa a tela de compartilhamento na chamada.</span><span class="sxs-lookup"><span data-stu-id="7875f-105">Start and stop sharing screen in the call.</span></span> <span data-ttu-id="7875f-106">Essa API é usada para permitir que os aplicativos compartilhem conteúdo de tela com os participantes de uma chamada ou reunião.</span><span class="sxs-lookup"><span data-stu-id="7875f-106">This API is used to allow applications to share screen content with the participants of a call or meeting.</span></span>

## <a name="permissions"></a><span data-ttu-id="7875f-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="7875f-107">Permissions</span></span>
<span data-ttu-id="7875f-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7875f-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7875f-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7875f-110">Permission type</span></span>                        | <span data-ttu-id="7875f-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7875f-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="7875f-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7875f-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="7875f-113">Não suportado</span><span class="sxs-lookup"><span data-stu-id="7875f-113">Not Supported</span></span>                               |
| <span data-ttu-id="7875f-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7875f-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7875f-115">Não suportado</span><span class="sxs-lookup"><span data-stu-id="7875f-115">Not Supported</span></span>                               |
| <span data-ttu-id="7875f-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7875f-116">Application</span></span>                            | <span data-ttu-id="7875f-117">Calls.AccessMedia.All</span><span class="sxs-lookup"><span data-stu-id="7875f-117">Calls.AccessMedia.All</span></span>                       |

## <a name="http-request"></a><span data-ttu-id="7875f-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7875f-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/changeScreenSharingRole
POST /applications/{id}/calls/{id}/changeScreenSharingRole
```

## <a name="request-headers"></a><span data-ttu-id="7875f-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7875f-119">Request headers</span></span>
| <span data-ttu-id="7875f-120">Nome</span><span class="sxs-lookup"><span data-stu-id="7875f-120">Name</span></span>          | <span data-ttu-id="7875f-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="7875f-121">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="7875f-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="7875f-122">Authorization</span></span> | <span data-ttu-id="7875f-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7875f-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7875f-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7875f-125">Request body</span></span>
<span data-ttu-id="7875f-126">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7875f-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="7875f-127">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="7875f-127">Parameter</span></span>      | <span data-ttu-id="7875f-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="7875f-128">Type</span></span>    |<span data-ttu-id="7875f-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="7875f-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7875f-130">role</span><span class="sxs-lookup"><span data-stu-id="7875f-130">role</span></span>|<span data-ttu-id="7875f-131">String</span><span class="sxs-lookup"><span data-stu-id="7875f-131">String</span></span>|<span data-ttu-id="7875f-132">Os valores possíveis são: ' Visualizador ', ' participante '</span><span class="sxs-lookup"><span data-stu-id="7875f-132">Possible values are: 'Viewer', 'Sharer'</span></span>|

## <a name="response"></a><span data-ttu-id="7875f-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="7875f-133">Response</span></span>
<span data-ttu-id="7875f-134">Retorna `202 Accepted` o código de resposta.</span><span class="sxs-lookup"><span data-stu-id="7875f-134">Returns `202 Accepted` response code.</span></span>

## <a name="example"></a><span data-ttu-id="7875f-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7875f-135">Example</span></span>
<span data-ttu-id="7875f-136">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="7875f-136">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="7875f-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7875f-137">Request</span></span>
<span data-ttu-id="7875f-138">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="7875f-138">The following example shows the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="7875f-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="7875f-139">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="7875f-140">C#</span><span class="sxs-lookup"><span data-stu-id="7875f-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-changescreensharingrole-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7875f-141">Javascript</span><span class="sxs-lookup"><span data-stu-id="7875f-141">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-changescreensharingrole-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="7875f-142">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="7875f-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-changescreensharingrole-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="7875f-143">Java</span><span class="sxs-lookup"><span data-stu-id="7875f-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/call-changescreensharingrole-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="7875f-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="7875f-144">Response</span></span>
<span data-ttu-id="7875f-145">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7875f-145">Here is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 202 Accepted
```

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
  ]
}
-->
