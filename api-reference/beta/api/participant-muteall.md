---
title: 'participante: muteAll'
description: Ative o mudo para todos os participantes em uma chamada.
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 00ace588a763a9e6d1df64830820be1ad6308567
ms.sourcegitcommit: 9bddc0b7746383e8d05ce50d163af3f4196f12a6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/06/2019
ms.locfileid: "38006463"
---
# <a name="participant-muteall"></a><span data-ttu-id="3f206-103">participante: muteAll</span><span class="sxs-lookup"><span data-stu-id="3f206-103">participant: muteAll</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3f206-104">Ative o mudo para todos os participantes em uma chamada.</span><span class="sxs-lookup"><span data-stu-id="3f206-104">Mute all participants in the call.</span></span>

## <a name="permissions"></a><span data-ttu-id="3f206-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="3f206-105">Permissions</span></span>
<span data-ttu-id="3f206-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3f206-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="3f206-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3f206-108">Permission type</span></span>                        | <span data-ttu-id="3f206-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3f206-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="3f206-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3f206-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="3f206-111">Não suportado</span><span class="sxs-lookup"><span data-stu-id="3f206-111">Not Supported</span></span>                               |
| <span data-ttu-id="3f206-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3f206-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3f206-113">Não suportado</span><span class="sxs-lookup"><span data-stu-id="3f206-113">Not Supported</span></span>                               |
| <span data-ttu-id="3f206-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3f206-114">Application</span></span>                            | <span data-ttu-id="3f206-115">Nenhum</span><span class="sxs-lookup"><span data-stu-id="3f206-115">None</span></span>                                        |

## <a name="http-request"></a><span data-ttu-id="3f206-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3f206-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/participants/muteAll
POST /communications/calls/{id}/participants/muteAll
```
> <span data-ttu-id="3f206-117">**Observação:** o caminho `/app` foi preterido.</span><span class="sxs-lookup"><span data-stu-id="3f206-117">**Note:** The `/app` path is deprecated.</span></span> <span data-ttu-id="3f206-118">Daqui em diante, use o caminho `/communications`.</span><span class="sxs-lookup"><span data-stu-id="3f206-118">Going forward, use the `/communications` path.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3f206-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3f206-119">Request headers</span></span>
| <span data-ttu-id="3f206-120">Nome</span><span class="sxs-lookup"><span data-stu-id="3f206-120">Name</span></span>          | <span data-ttu-id="3f206-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="3f206-121">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="3f206-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="3f206-122">Authorization</span></span> | <span data-ttu-id="3f206-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3f206-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3f206-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3f206-125">Request body</span></span>
<span data-ttu-id="3f206-126">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3f206-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="3f206-127">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="3f206-127">Parameter</span></span>      | <span data-ttu-id="3f206-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="3f206-128">Type</span></span>    |<span data-ttu-id="3f206-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="3f206-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3f206-130">participants</span><span class="sxs-lookup"><span data-stu-id="3f206-130">participants</span></span>|<span data-ttu-id="3f206-131">String collection</span><span class="sxs-lookup"><span data-stu-id="3f206-131">String collection</span></span>|<span data-ttu-id="3f206-132">Os participantes a serem mudo.</span><span class="sxs-lookup"><span data-stu-id="3f206-132">The participants to be muted.</span></span>|
|<span data-ttu-id="3f206-133">clientContext</span><span class="sxs-lookup"><span data-stu-id="3f206-133">clientContext</span></span>|<span data-ttu-id="3f206-134">String</span><span class="sxs-lookup"><span data-stu-id="3f206-134">String</span></span>|<span data-ttu-id="3f206-135">O contexto do cliente.</span><span class="sxs-lookup"><span data-stu-id="3f206-135">The client context.</span></span>|

## <a name="response"></a><span data-ttu-id="3f206-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="3f206-136">Response</span></span>
<span data-ttu-id="3f206-137">Se bem-sucedido, este método retorna `200 OK` o código de resposta e o objeto [commsOperation](../resources/commsoperation.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3f206-137">If successful, this method returns `200 OK` response code and [commsOperation](../resources/commsoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3f206-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3f206-138">Example</span></span>
<span data-ttu-id="3f206-139">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="3f206-139">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="3f206-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3f206-140">Request</span></span>
<span data-ttu-id="3f206-141">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="3f206-141">The following example shows the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="3f206-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="3f206-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "participant-muteAll"
}-->
```http
POST https://graph.microsoft.com/beta/communications/calls/{id}/participants/muteAll
Content-Type: application/json
Content-Length: 81

{
  "participants": [
    ""
  ],
  "clientContext": "clientContext-value"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="3f206-143">C#</span><span class="sxs-lookup"><span data-stu-id="3f206-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/participant-muteall-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3f206-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3f206-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/participant-muteall-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="3f206-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3f206-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/participant-muteall-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="3f206-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="3f206-146">Response</span></span>

> <span data-ttu-id="3f206-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3f206-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.commsOperation"
} -->
```http
HTTP/1.1 200 OK
Location: https://graph.microsoft.com/beta/communications/calls/57dab8b1-894c-409a-b240-bd8beae78896/operations/17e3b46c-f61d-4f4d-9635-c626ef18e6ad
Content-Type: application/json
Content-Length: 259

{
  "id": "17e3b46c-f61d-4f4d-9635-c626ef18e6ad",
  "status": "completed",
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
