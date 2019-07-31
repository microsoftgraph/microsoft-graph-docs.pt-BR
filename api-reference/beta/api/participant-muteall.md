---
title: 'participante: muteAll'
description: Ative o mudo para todos os participantes em uma chamada.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 14f21180052579fe417544ebb08c8960d34d58b8
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35983527"
---
# <a name="participant-muteall"></a><span data-ttu-id="2993a-103">participante: muteAll</span><span class="sxs-lookup"><span data-stu-id="2993a-103">participant: muteAll</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2993a-104">Ative o mudo para todos os participantes em uma chamada.</span><span class="sxs-lookup"><span data-stu-id="2993a-104">Mute all participants in the call.</span></span>

## <a name="permissions"></a><span data-ttu-id="2993a-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="2993a-105">Permissions</span></span>
<span data-ttu-id="2993a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2993a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2993a-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2993a-108">Permission type</span></span>                        | <span data-ttu-id="2993a-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2993a-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="2993a-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2993a-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="2993a-111">Não suportado</span><span class="sxs-lookup"><span data-stu-id="2993a-111">Not Supported</span></span>                               |
| <span data-ttu-id="2993a-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2993a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2993a-113">Não suportado</span><span class="sxs-lookup"><span data-stu-id="2993a-113">Not Supported</span></span>                               |
| <span data-ttu-id="2993a-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2993a-114">Application</span></span>                            | <span data-ttu-id="2993a-115">Nenhum</span><span class="sxs-lookup"><span data-stu-id="2993a-115">None</span></span>                                        |

## <a name="http-request"></a><span data-ttu-id="2993a-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2993a-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/participants/muteAll
POST /applications/{id}/calls/{id}/participants/muteAll
```

## <a name="request-headers"></a><span data-ttu-id="2993a-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2993a-117">Request headers</span></span>
| <span data-ttu-id="2993a-118">Nome</span><span class="sxs-lookup"><span data-stu-id="2993a-118">Name</span></span>          | <span data-ttu-id="2993a-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="2993a-119">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="2993a-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="2993a-120">Authorization</span></span> | <span data-ttu-id="2993a-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2993a-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2993a-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2993a-123">Request body</span></span>
<span data-ttu-id="2993a-124">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2993a-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="2993a-125">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="2993a-125">Parameter</span></span>      | <span data-ttu-id="2993a-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="2993a-126">Type</span></span>    |<span data-ttu-id="2993a-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="2993a-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2993a-128">participants</span><span class="sxs-lookup"><span data-stu-id="2993a-128">participants</span></span>|<span data-ttu-id="2993a-129">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="2993a-129">String collection</span></span>|<span data-ttu-id="2993a-130">Os participantes a serem mudo.</span><span class="sxs-lookup"><span data-stu-id="2993a-130">The participants to be muted.</span></span>|
|<span data-ttu-id="2993a-131">clientContext</span><span class="sxs-lookup"><span data-stu-id="2993a-131">clientContext</span></span>|<span data-ttu-id="2993a-132">String</span><span class="sxs-lookup"><span data-stu-id="2993a-132">String</span></span>|<span data-ttu-id="2993a-133">O contexto do cliente.</span><span class="sxs-lookup"><span data-stu-id="2993a-133">The client context.</span></span>|

## <a name="response"></a><span data-ttu-id="2993a-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="2993a-134">Response</span></span>
<span data-ttu-id="2993a-135">Se bem-sucedido, este método retorna `200 OK` o código de resposta e o objeto [commsOperation](../resources/commsoperation.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2993a-135">If successful, this method returns `200 OK` response code and [commsOperation](../resources/commsoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2993a-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2993a-136">Example</span></span>
<span data-ttu-id="2993a-137">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="2993a-137">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="2993a-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2993a-138">Request</span></span>
<span data-ttu-id="2993a-139">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="2993a-139">The following example shows the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="2993a-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="2993a-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "participant-muteAll"
}-->
```http
POST https://graph.microsoft.com/beta/app/calls/{id}/participants/muteAll
Content-Type: application/json
Content-Length: 81

{
  "participants": [
    ""
  ],
  "clientContext": "clientContext-value"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="2993a-141">C#</span><span class="sxs-lookup"><span data-stu-id="2993a-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/participant-muteall-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="2993a-142">Javascript</span><span class="sxs-lookup"><span data-stu-id="2993a-142">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/participant-muteall-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="2993a-143">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="2993a-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/participant-muteall-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="2993a-144">Java</span><span class="sxs-lookup"><span data-stu-id="2993a-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/participant-muteall-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="2993a-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="2993a-145">Response</span></span>

> <span data-ttu-id="2993a-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2993a-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "description": "participant: muteAll",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
