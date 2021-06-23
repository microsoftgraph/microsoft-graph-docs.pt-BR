---
title: Excluir conversationMember
description: Excluir conversationMember de um canal.
author: akjo
doc_type: apiPageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 2b0489387f4822296788c417536332c2fef387ad
ms.sourcegitcommit: 456ec9510807d05623c0ed1dd049c9676f53f56b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/22/2021
ms.locfileid: "53060594"
---
# <a name="delete-conversationmember"></a><span data-ttu-id="ebd36-103">Excluir conversationMember</span><span class="sxs-lookup"><span data-stu-id="ebd36-103">Delete conversationMember</span></span>

<span data-ttu-id="ebd36-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ebd36-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ebd36-105">Excluir uma [conversaMember](../resources/conversationmember.md) de um [canal](../resources/channel.md).</span><span class="sxs-lookup"><span data-stu-id="ebd36-105">Delete a [conversationMember](../resources/conversationmember.md) from a [channel](../resources/channel.md).</span></span>


## <a name="permissions"></a><span data-ttu-id="ebd36-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="ebd36-106">Permissions</span></span>

<span data-ttu-id="ebd36-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ebd36-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ebd36-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ebd36-109">Permission Type</span></span>|<span data-ttu-id="ebd36-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ebd36-110">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="ebd36-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ebd36-111">Delegated (work or school account)</span></span>| <span data-ttu-id="ebd36-112">ChannelMember.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ebd36-112">ChannelMember.ReadWrite.All</span></span> |
|<span data-ttu-id="ebd36-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ebd36-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ebd36-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ebd36-114">Not supported.</span></span>|
|<span data-ttu-id="ebd36-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ebd36-115">Application</span></span>| <span data-ttu-id="ebd36-116">ChannelMember.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ebd36-116">ChannelMember.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ebd36-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ebd36-117">HTTP request</span></span>
<!-- { "blockType": "ignored"} -->
```http
DELETE /teams/{id}/channels/{id}/members/{id}
```

## <a name="request-headers"></a><span data-ttu-id="ebd36-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ebd36-118">Request headers</span></span>

| <span data-ttu-id="ebd36-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ebd36-119">Header</span></span>       | <span data-ttu-id="ebd36-120">Valor</span><span class="sxs-lookup"><span data-stu-id="ebd36-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="ebd36-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="ebd36-121">Authorization</span></span>  | <span data-ttu-id="ebd36-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ebd36-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="ebd36-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ebd36-124">Request body</span></span>

<span data-ttu-id="ebd36-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ebd36-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ebd36-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="ebd36-126">Response</span></span>

<span data-ttu-id="ebd36-127">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="ebd36-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="ebd36-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ebd36-128">Example</span></span>

### <a name="request"></a><span data-ttu-id="ebd36-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ebd36-129">Request</span></span>

<span data-ttu-id="ebd36-130">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ebd36-130">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ebd36-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="ebd36-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_conversation_member"
} -->
```http
DELETE https://graph.microsoft.com/V1.0/teams/{id}/channels/{id}/members/{id}
```
# <a name="c"></a>[<span data-ttu-id="ebd36-132">C#</span><span class="sxs-lookup"><span data-stu-id="ebd36-132">C#</span></span>](#tab/csharp)

# <a name="javascript"></a>[<span data-ttu-id="ebd36-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ebd36-133">JavaScript</span></span>](#tab/javascript)

# <a name="objective-c"></a>[<span data-ttu-id="ebd36-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ebd36-134">Objective-C</span></span>](#tab/objc)

---

### <a name="response"></a><span data-ttu-id="ebd36-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="ebd36-135">Response</span></span>

<span data-ttu-id="ebd36-136">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ebd36-136">Here is an example of the response.</span></span>

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 204 No Content
```
