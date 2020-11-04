---
title: Excluir conversationMember
description: Excluir conversationMember de um canal.
author: laujan
doc_type: apiPageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 05dd3377e5a3161a38d9db1d56de7bba7ccf9af4
ms.sourcegitcommit: d1e72c8d36aad78732133f9ecefaf66c433b8530
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/03/2020
ms.locfileid: "48848322"
---
# <a name="delete-conversationmember"></a><span data-ttu-id="de321-103">Excluir conversationMember</span><span class="sxs-lookup"><span data-stu-id="de321-103">Delete conversationMember</span></span>

<span data-ttu-id="de321-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="de321-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="de321-105">Excluir um [conversationMember](../resources/conversationmember.md) de um [canal](../resources/channel.md).</span><span class="sxs-lookup"><span data-stu-id="de321-105">Delete a [conversationMember](../resources/conversationmember.md) from a [channel](../resources/channel.md).</span></span>


## <a name="permissions"></a><span data-ttu-id="de321-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="de321-106">Permissions</span></span>

<span data-ttu-id="de321-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="de321-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="de321-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="de321-109">Permission Type</span></span>|<span data-ttu-id="de321-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="de321-110">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="de321-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="de321-111">Delegated (work or school account)</span></span>| <span data-ttu-id="de321-112">ChannelMember.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="de321-112">ChannelMember.ReadWrite.All</span></span> |
|<span data-ttu-id="de321-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="de321-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="de321-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="de321-114">Not supported.</span></span>|
|<span data-ttu-id="de321-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="de321-115">Application</span></span>| <span data-ttu-id="de321-116">ChannelMember.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="de321-116">ChannelMember.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="de321-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="de321-117">HTTP request</span></span>
<!-- { "blockType": "ignored"} -->
```http
DELETE /teams/{id}/channels/{id}/members/{id}
```

## <a name="request-headers"></a><span data-ttu-id="de321-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="de321-118">Request headers</span></span>

| <span data-ttu-id="de321-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="de321-119">Header</span></span>       | <span data-ttu-id="de321-120">Valor</span><span class="sxs-lookup"><span data-stu-id="de321-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="de321-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="de321-121">Authorization</span></span>  | <span data-ttu-id="de321-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="de321-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="de321-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="de321-124">Request body</span></span>

<span data-ttu-id="de321-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="de321-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="de321-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="de321-126">Response</span></span>

<span data-ttu-id="de321-127">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="de321-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="de321-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="de321-128">Example</span></span>

### <a name="request"></a><span data-ttu-id="de321-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="de321-129">Request</span></span>

<span data-ttu-id="de321-130">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="de321-130">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="de321-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="de321-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_conversation_member"
} -->
```http
DELETE https://graph.microsoft.com/V1.0/teams/{id}/channels/{id}/members/{id}
```
# <a name="c"></a>[<span data-ttu-id="de321-132">C#</span><span class="sxs-lookup"><span data-stu-id="de321-132">C#</span></span>](#tab/csharp)

# <a name="javascript"></a>[<span data-ttu-id="de321-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="de321-133">JavaScript</span></span>](#tab/javascript)

# <a name="objective-c"></a>[<span data-ttu-id="de321-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="de321-134">Objective-C</span></span>](#tab/objc)

---

### <a name="response"></a><span data-ttu-id="de321-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="de321-135">Response</span></span>

<span data-ttu-id="de321-136">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="de321-136">Here is an example of the response.</span></span>

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 204 No Content
```
