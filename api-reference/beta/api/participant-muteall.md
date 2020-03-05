---
title: 'participante: muteAll'
description: Ative o mudo para todos os participantes em uma chamada.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 5bddd241226d0e583c7c5871c8da291edc486ff6
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42455958"
---
# <a name="participant-muteall"></a><span data-ttu-id="403ab-103">participante: muteAll</span><span class="sxs-lookup"><span data-stu-id="403ab-103">participant: muteAll</span></span>

<span data-ttu-id="403ab-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="403ab-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="403ab-105">Ative o mudo para todos os participantes em uma chamada.</span><span class="sxs-lookup"><span data-stu-id="403ab-105">Mute all participants in the call.</span></span>

> <span data-ttu-id="403ab-106">**Observação:** Esta API foi preterida e será removida até 15 de março de 2020.</span><span class="sxs-lookup"><span data-stu-id="403ab-106">**Note:** This API is deprecated and will be removed by March 15th, 2020.</span></span> <span data-ttu-id="403ab-107">Para fazer o mudo de um único participante, confira [participante: sem áudio](participant-mute.md).</span><span class="sxs-lookup"><span data-stu-id="403ab-107">To mute a single participant, see [participant: mute](participant-mute.md).</span></span>


## <a name="permissions"></a><span data-ttu-id="403ab-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="403ab-108">Permissions</span></span>
<span data-ttu-id="403ab-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="403ab-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="403ab-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="403ab-111">Permission type</span></span>                        | <span data-ttu-id="403ab-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="403ab-112">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="403ab-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="403ab-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="403ab-114">Não suportado</span><span class="sxs-lookup"><span data-stu-id="403ab-114">Not Supported</span></span>                               |
| <span data-ttu-id="403ab-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="403ab-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="403ab-116">Não suportado</span><span class="sxs-lookup"><span data-stu-id="403ab-116">Not Supported</span></span>                               |
| <span data-ttu-id="403ab-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="403ab-117">Application</span></span>                            | <span data-ttu-id="403ab-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="403ab-118">None</span></span>                                        |

## <a name="http-request"></a><span data-ttu-id="403ab-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="403ab-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/participants/muteAll
POST /communications/calls/{id}/participants/muteAll
```
> <span data-ttu-id="403ab-120">**Observação:** o caminho `/app` foi preterido.</span><span class="sxs-lookup"><span data-stu-id="403ab-120">**Note:** The `/app` path is deprecated.</span></span> <span data-ttu-id="403ab-121">Daqui em diante, use o caminho `/communications`.</span><span class="sxs-lookup"><span data-stu-id="403ab-121">Going forward, use the `/communications` path.</span></span>

## <a name="request-headers"></a><span data-ttu-id="403ab-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="403ab-122">Request headers</span></span>
| <span data-ttu-id="403ab-123">Nome</span><span class="sxs-lookup"><span data-stu-id="403ab-123">Name</span></span>          | <span data-ttu-id="403ab-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="403ab-124">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="403ab-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="403ab-125">Authorization</span></span> | <span data-ttu-id="403ab-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="403ab-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="403ab-128">Content-type</span><span class="sxs-lookup"><span data-stu-id="403ab-128">Content-type</span></span> | <span data-ttu-id="403ab-p105">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="403ab-p105">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="403ab-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="403ab-131">Request body</span></span>
<span data-ttu-id="403ab-132">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="403ab-132">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="403ab-133">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="403ab-133">Parameter</span></span>      | <span data-ttu-id="403ab-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="403ab-134">Type</span></span>    |<span data-ttu-id="403ab-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="403ab-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="403ab-136">participantes</span><span class="sxs-lookup"><span data-stu-id="403ab-136">participants</span></span>|<span data-ttu-id="403ab-137">String collection</span><span class="sxs-lookup"><span data-stu-id="403ab-137">String collection</span></span>|<span data-ttu-id="403ab-138">Os participantes a serem mudo.</span><span class="sxs-lookup"><span data-stu-id="403ab-138">The participants to be muted.</span></span>|
|<span data-ttu-id="403ab-139">clientContext</span><span class="sxs-lookup"><span data-stu-id="403ab-139">clientContext</span></span>|<span data-ttu-id="403ab-140">String</span><span class="sxs-lookup"><span data-stu-id="403ab-140">String</span></span>|<span data-ttu-id="403ab-141">O contexto do cliente.</span><span class="sxs-lookup"><span data-stu-id="403ab-141">The client context.</span></span>|

## <a name="response"></a><span data-ttu-id="403ab-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="403ab-142">Response</span></span>
<span data-ttu-id="403ab-143">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [commsOperation](../resources/commsoperation.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="403ab-143">If successful, this method returns a `200 OK` response code and a [commsOperation](../resources/commsoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="403ab-144">Exemplo</span><span class="sxs-lookup"><span data-stu-id="403ab-144">Example</span></span>
<span data-ttu-id="403ab-145">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="403ab-145">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="403ab-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="403ab-146">Request</span></span>
<span data-ttu-id="403ab-147">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="403ab-147">The following example shows the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="403ab-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="403ab-148">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="403ab-149">C#</span><span class="sxs-lookup"><span data-stu-id="403ab-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/participant-muteall-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="403ab-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="403ab-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/participant-muteall-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="403ab-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="403ab-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/participant-muteall-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="403ab-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="403ab-152">Response</span></span>

> <span data-ttu-id="403ab-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="403ab-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "name": "participant-muteAll",
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
  "description": "participant: muteAll",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
