---
title: Obter conversationMember
description: Recuperar um membro de um bate-papo.
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: a2c539b7240060a6434f5ece01dc242ae948a5f4
ms.sourcegitcommit: afea19508ad74a3583b11b5f7b544c53eafb3740
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/22/2019
ms.locfileid: "34379264"
---
# <a name="get-conversationmember"></a><span data-ttu-id="4d373-103">Obter conversationMember</span><span class="sxs-lookup"><span data-stu-id="4d373-103">Get conversationMember</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4d373-104">Recuperar um [conversationMember](../resources/conversationmember.md) de um [bate-papo](../resources/chat.md).</span><span class="sxs-lookup"><span data-stu-id="4d373-104">Retrieve a [conversationMember](../resources/conversationmember.md) from a [chat](../resources/chat.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="4d373-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="4d373-105">Permissions</span></span>

<span data-ttu-id="4d373-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4d373-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4d373-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4d373-108">Permission Type</span></span>|<span data-ttu-id="4d373-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4d373-109">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="4d373-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4d373-110">Delegated (work or school account)</span></span>|<span data-ttu-id="4d373-111">Chat.Read, Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4d373-111">Chat.Read, Chat.ReadWrite</span></span>|
|<span data-ttu-id="4d373-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4d373-112">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4d373-113">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="4d373-113">Not supported</span></span>|
|<span data-ttu-id="4d373-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4d373-114">Application</span></span> |<span data-ttu-id="4d373-115">Chat.Read.All, Chat.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4d373-115">Chat.Read.All, Chat.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4d373-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4d373-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /chats/{id}/members/{id}
GET /users/{id}/chats/{id}/members/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4d373-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="4d373-117">Optional query parameters</span></span>

<span data-ttu-id="4d373-118">Esta operação não é compatível com os [parâmetros de consulta OData](/graph/query-parameters) para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="4d373-118">This operation does not currently support [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4d373-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4d373-119">Request headers</span></span>

| <span data-ttu-id="4d373-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4d373-120">Header</span></span>       | <span data-ttu-id="4d373-121">Valor</span><span class="sxs-lookup"><span data-stu-id="4d373-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="4d373-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="4d373-122">Authorization</span></span>  | <span data-ttu-id="4d373-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4d373-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="4d373-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4d373-125">Request body</span></span>

<span data-ttu-id="4d373-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="4d373-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4d373-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="4d373-127">Response</span></span>

<span data-ttu-id="4d373-128">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [conversationMember](../resources/conversationmember.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4d373-128">If successful, this method returns a `200 OK` response code and a [chatmessage](../resources/conversationmember.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4d373-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4d373-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="4d373-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4d373-130">Request</span></span>

<span data-ttu-id="4d373-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4d373-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_conversation_member"
}-->
```http
GET https://graph.microsoft.com/beta/chats/{id}/members/{id}
```

##### <a name="response"></a><span data-ttu-id="4d373-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="4d373-132">Response</span></span>

<span data-ttu-id="4d373-133">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4d373-133">Here is an example of the response.</span></span> 

><span data-ttu-id="4d373-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4d373-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversationMember"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 201

{
  "id": "id-value",
  "displayName": "display-name-value"
}
```