---
title: 'participante: muteAll'
description: Ative o mudo para todos os participantes em uma chamada.
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: a4f5157e4441269258ed578a26a6ea700b8e4e0a
ms.sourcegitcommit: d40d2a9266bd376d713382925323aefab285ed69
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/20/2019
ms.locfileid: "38747963"
---
# <a name="participant-muteall"></a><span data-ttu-id="f96b5-103">participante: muteAll</span><span class="sxs-lookup"><span data-stu-id="f96b5-103">participant: muteAll</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f96b5-104">Ative o mudo para todos os participantes em uma chamada.</span><span class="sxs-lookup"><span data-stu-id="f96b5-104">Mute all participants in the call.</span></span>

> <span data-ttu-id="f96b5-105">**Observação:** Esta API foi preterida e será removida até 15 de março de 2020.</span><span class="sxs-lookup"><span data-stu-id="f96b5-105">**Note:** This API is deprecated and will be removed by March 15th, 2020.</span></span> <span data-ttu-id="f96b5-106">Para fazer o mudo de um único participante, confira [participante: sem áudio](participant-mute.md).</span><span class="sxs-lookup"><span data-stu-id="f96b5-106">To mute a single participant, see [participant: mute](participant-mute.md).</span></span>


## <a name="permissions"></a><span data-ttu-id="f96b5-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="f96b5-107">Permissions</span></span>
<span data-ttu-id="f96b5-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f96b5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f96b5-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f96b5-110">Permission type</span></span>                        | <span data-ttu-id="f96b5-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f96b5-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="f96b5-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f96b5-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="f96b5-113">Não suportado</span><span class="sxs-lookup"><span data-stu-id="f96b5-113">Not Supported</span></span>                               |
| <span data-ttu-id="f96b5-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f96b5-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f96b5-115">Não suportado</span><span class="sxs-lookup"><span data-stu-id="f96b5-115">Not Supported</span></span>                               |
| <span data-ttu-id="f96b5-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f96b5-116">Application</span></span>                            | <span data-ttu-id="f96b5-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f96b5-117">None</span></span>                                        |

## <a name="http-request"></a><span data-ttu-id="f96b5-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f96b5-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/participants/muteAll
POST /communications/calls/{id}/participants/muteAll
```
> <span data-ttu-id="f96b5-119">**Observação:** o caminho `/app` foi preterido.</span><span class="sxs-lookup"><span data-stu-id="f96b5-119">**Note:** The `/app` path is deprecated.</span></span> <span data-ttu-id="f96b5-120">Daqui em diante, use o caminho `/communications`.</span><span class="sxs-lookup"><span data-stu-id="f96b5-120">Going forward, use the `/communications` path.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f96b5-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f96b5-121">Request headers</span></span>
| <span data-ttu-id="f96b5-122">Nome</span><span class="sxs-lookup"><span data-stu-id="f96b5-122">Name</span></span>          | <span data-ttu-id="f96b5-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="f96b5-123">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="f96b5-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="f96b5-124">Authorization</span></span> | <span data-ttu-id="f96b5-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f96b5-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f96b5-127">Content-type</span><span class="sxs-lookup"><span data-stu-id="f96b5-127">Content-type</span></span> | <span data-ttu-id="f96b5-p105">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f96b5-p105">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f96b5-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f96b5-130">Request body</span></span>
<span data-ttu-id="f96b5-131">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f96b5-131">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="f96b5-132">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="f96b5-132">Parameter</span></span>      | <span data-ttu-id="f96b5-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="f96b5-133">Type</span></span>    |<span data-ttu-id="f96b5-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="f96b5-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f96b5-135">participants</span><span class="sxs-lookup"><span data-stu-id="f96b5-135">participants</span></span>|<span data-ttu-id="f96b5-136">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="f96b5-136">String collection</span></span>|<span data-ttu-id="f96b5-137">Os participantes a serem mudo.</span><span class="sxs-lookup"><span data-stu-id="f96b5-137">The participants to be muted.</span></span>|
|<span data-ttu-id="f96b5-138">clientContext</span><span class="sxs-lookup"><span data-stu-id="f96b5-138">clientContext</span></span>|<span data-ttu-id="f96b5-139">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="f96b5-139">String</span></span>|<span data-ttu-id="f96b5-140">O contexto do cliente.</span><span class="sxs-lookup"><span data-stu-id="f96b5-140">The client context.</span></span>|

## <a name="response"></a><span data-ttu-id="f96b5-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="f96b5-141">Response</span></span>
<span data-ttu-id="f96b5-142">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [commsOperation](../resources/commsoperation.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f96b5-142">If successful, this method returns a `200 OK` response code and a [commsOperation](../resources/commsoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f96b5-143">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f96b5-143">Example</span></span>
<span data-ttu-id="f96b5-144">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="f96b5-144">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="f96b5-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f96b5-145">Request</span></span>
<span data-ttu-id="f96b5-146">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="f96b5-146">The following example shows the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="f96b5-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="f96b5-147">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="f96b5-148">C#</span><span class="sxs-lookup"><span data-stu-id="f96b5-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/participant-muteall-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f96b5-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f96b5-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/participant-muteall-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="f96b5-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f96b5-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/participant-muteall-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="f96b5-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="f96b5-151">Response</span></span>

> <span data-ttu-id="f96b5-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f96b5-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
