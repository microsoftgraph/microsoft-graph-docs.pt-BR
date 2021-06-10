---
title: 'channel: removeEmail'
description: Remova o email provisionado de um canal.
author: anandab-msft
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 66efdd201217d34ba367df4ae1f30713cd939df4
ms.sourcegitcommit: 503c72036c376a30e08c29df8e7730a7afcab66e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/10/2021
ms.locfileid: "52869586"
---
# <a name="channel-removeemail"></a><span data-ttu-id="5bfa0-103">channel: removeEmail</span><span class="sxs-lookup"><span data-stu-id="5bfa0-103">channel: removeEmail</span></span>

<span data-ttu-id="5bfa0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5bfa0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5bfa0-105">Remova o endereço de email provisionado de um [canal](../resources/channel.md).</span><span class="sxs-lookup"><span data-stu-id="5bfa0-105">Remove the provisioned email address of a [channel](../resources/channel.md).</span></span>

<span data-ttu-id="5bfa0-106">Você só poderá remover um endereço de email se ele tiver sido provisionado usando o [método provisionEmail](channel-provisionemail.md) ou por meio do Microsoft Teams cliente.</span><span class="sxs-lookup"><span data-stu-id="5bfa0-106">You can remove an email address only if it was provisioned using the [provisionEmail](channel-provisionemail.md) method or through the Microsoft Teams client.</span></span>

## <a name="permissions"></a><span data-ttu-id="5bfa0-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="5bfa0-107">Permissions</span></span>

<span data-ttu-id="5bfa0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5bfa0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5bfa0-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5bfa0-110">Permission type</span></span>                        | <span data-ttu-id="5bfa0-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5bfa0-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="5bfa0-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5bfa0-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="5bfa0-113">ChannelSettings.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5bfa0-113">ChannelSettings.ReadWrite.All</span></span>               |
| <span data-ttu-id="5bfa0-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5bfa0-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5bfa0-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5bfa0-115">Not supported.</span></span>                              |
| <span data-ttu-id="5bfa0-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5bfa0-116">Application</span></span>                            | <span data-ttu-id="5bfa0-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5bfa0-117">Not supported.</span></span>                              |

## <a name="http-request"></a><span data-ttu-id="5bfa0-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5bfa0-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{team-id}/channels/{channel-id}/removeEmail
```
## <a name="request-headers"></a><span data-ttu-id="5bfa0-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5bfa0-119">Request headers</span></span>
| <span data-ttu-id="5bfa0-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5bfa0-120">Header</span></span>        | <span data-ttu-id="5bfa0-121">Valor</span><span class="sxs-lookup"><span data-stu-id="5bfa0-121">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="5bfa0-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="5bfa0-122">Authorization</span></span> | <span data-ttu-id="5bfa0-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5bfa0-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5bfa0-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5bfa0-125">Request body</span></span>

<span data-ttu-id="5bfa0-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5bfa0-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5bfa0-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="5bfa0-127">Response</span></span>

<span data-ttu-id="5bfa0-128">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="5bfa0-128">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="5bfa0-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5bfa0-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="5bfa0-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5bfa0-130">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="5bfa0-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="5bfa0-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["893075dd-2487-4122-925f-022c42e20265", "19:561fbdbbfca848a484f0a6f00ce9dbbd@thread.tacv2"],
  "name": "channel_removeemail"
}
-->
```http
POST https://graph.microsoft.com/beta/teams/893075dd-2487-4122-925f-022c42e20265/channels/19:561fbdbbfca848a484f0a6f00ce9dbbd@thread.tacv2/removeEmail
```
# <a name="c"></a>[<span data-ttu-id="5bfa0-132">C#</span><span class="sxs-lookup"><span data-stu-id="5bfa0-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/channel-removeemail-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5bfa0-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5bfa0-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/channel-removeemail-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5bfa0-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5bfa0-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/channel-removeemail-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5bfa0-135">Java</span><span class="sxs-lookup"><span data-stu-id="5bfa0-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/channel-removeemail-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="5bfa0-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="5bfa0-136">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```
<!-- uuid: e848414b-4669-4484-ac36-1504c58a3fb8
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Remove channel email",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


