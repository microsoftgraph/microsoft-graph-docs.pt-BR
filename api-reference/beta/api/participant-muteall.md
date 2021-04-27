---
title: 'participante: muteAll'
description: Ative o mudo para todos os participantes em uma chamada.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: a0cf9da4b6903931b813c0c2b2bd1aed3681434d
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52049181"
---
# <a name="participant-muteall"></a><span data-ttu-id="9705a-103">participante: muteAll</span><span class="sxs-lookup"><span data-stu-id="9705a-103">participant: muteAll</span></span>

<span data-ttu-id="9705a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9705a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9705a-105">Ative o mudo para todos os participantes em uma chamada.</span><span class="sxs-lookup"><span data-stu-id="9705a-105">Mute all participants in the call.</span></span>

> <span data-ttu-id="9705a-106">**Observação:** Essa API foi preterida e será removida até 15 de março de 2020.</span><span class="sxs-lookup"><span data-stu-id="9705a-106">**Note:** This API is deprecated and will be removed by March 15th, 2020.</span></span> <span data-ttu-id="9705a-107">Para silenciar um único participante, consulte [participante: mute](participant-mute.md).</span><span class="sxs-lookup"><span data-stu-id="9705a-107">To mute a single participant, see [participant: mute](participant-mute.md).</span></span>


## <a name="permissions"></a><span data-ttu-id="9705a-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="9705a-108">Permissions</span></span>
<span data-ttu-id="9705a-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9705a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="9705a-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9705a-111">Permission type</span></span>                        | <span data-ttu-id="9705a-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9705a-112">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="9705a-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9705a-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="9705a-114">Não suportado</span><span class="sxs-lookup"><span data-stu-id="9705a-114">Not Supported</span></span>                               |
| <span data-ttu-id="9705a-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9705a-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9705a-116">Não suportado</span><span class="sxs-lookup"><span data-stu-id="9705a-116">Not Supported</span></span>                               |
| <span data-ttu-id="9705a-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9705a-117">Application</span></span>                            | <span data-ttu-id="9705a-118">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="9705a-118">None</span></span>                                        |

## <a name="http-request"></a><span data-ttu-id="9705a-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9705a-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/participants/muteAll
POST /communications/calls/{id}/participants/muteAll
```
> <span data-ttu-id="9705a-120">**Observação:** o caminho `/app` foi preterido.</span><span class="sxs-lookup"><span data-stu-id="9705a-120">**Note:** The `/app` path is deprecated.</span></span> <span data-ttu-id="9705a-121">Daqui em diante, use o caminho `/communications`.</span><span class="sxs-lookup"><span data-stu-id="9705a-121">Going forward, use the `/communications` path.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9705a-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9705a-122">Request headers</span></span>
| <span data-ttu-id="9705a-123">Nome</span><span class="sxs-lookup"><span data-stu-id="9705a-123">Name</span></span>          | <span data-ttu-id="9705a-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="9705a-124">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="9705a-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="9705a-125">Authorization</span></span> | <span data-ttu-id="9705a-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9705a-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="9705a-128">Content-type</span><span class="sxs-lookup"><span data-stu-id="9705a-128">Content-type</span></span> | <span data-ttu-id="9705a-p105">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9705a-p105">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9705a-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9705a-131">Request body</span></span>
<span data-ttu-id="9705a-132">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9705a-132">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="9705a-133">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="9705a-133">Parameter</span></span>      | <span data-ttu-id="9705a-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="9705a-134">Type</span></span>    |<span data-ttu-id="9705a-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="9705a-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9705a-136">participants</span><span class="sxs-lookup"><span data-stu-id="9705a-136">participants</span></span>|<span data-ttu-id="9705a-137">Conjunto de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="9705a-137">String collection</span></span>|<span data-ttu-id="9705a-138">Os participantes a serem mudos.</span><span class="sxs-lookup"><span data-stu-id="9705a-138">The participants to be muted.</span></span>|
|<span data-ttu-id="9705a-139">clientContext</span><span class="sxs-lookup"><span data-stu-id="9705a-139">clientContext</span></span>|<span data-ttu-id="9705a-140">String</span><span class="sxs-lookup"><span data-stu-id="9705a-140">String</span></span>|<span data-ttu-id="9705a-141">O contexto do cliente.</span><span class="sxs-lookup"><span data-stu-id="9705a-141">The client context.</span></span>|

## <a name="response"></a><span data-ttu-id="9705a-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="9705a-142">Response</span></span>
<span data-ttu-id="9705a-143">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto commsOperation](../resources/commsoperation.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9705a-143">If successful, this method returns a `200 OK` response code and a [commsOperation](../resources/commsoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9705a-144">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9705a-144">Example</span></span>
<span data-ttu-id="9705a-145">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="9705a-145">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="9705a-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9705a-146">Request</span></span>
<span data-ttu-id="9705a-147">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="9705a-147">The following example shows the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="9705a-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="9705a-148">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="9705a-149">C#</span><span class="sxs-lookup"><span data-stu-id="9705a-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/participant-muteall-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9705a-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9705a-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/participant-muteall-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9705a-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9705a-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/participant-muteall-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9705a-152">Java</span><span class="sxs-lookup"><span data-stu-id="9705a-152">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/participant-muteall-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="9705a-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="9705a-153">Response</span></span>

> <span data-ttu-id="9705a-154">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="9705a-154">**Note:** The response object shown here might be shortened for readability.</span></span>

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


