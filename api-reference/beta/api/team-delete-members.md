---
title: Remover membro da equipe
description: Remover um conversationMember de uma equipe.
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 97e6b940abd02e409531f9872393583320f88eba
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/15/2021
ms.locfileid: "49873007"
---
# <a name="remove-member-from-team"></a><span data-ttu-id="20916-103">Remover membro da equipe</span><span class="sxs-lookup"><span data-stu-id="20916-103">Remove member from team</span></span>
<span data-ttu-id="20916-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="20916-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="20916-105">Remover um [conversationMember](../resources/conversationmember.md) de uma [equipe](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="20916-105">Remove a [conversationMember](../resources/conversationmember.md) from a [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="20916-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="20916-106">Permissions</span></span>
<span data-ttu-id="20916-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="20916-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="20916-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="20916-109">Permission type</span></span>|<span data-ttu-id="20916-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="20916-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="20916-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="20916-111">Delegated (work or school account)</span></span>| <span data-ttu-id="20916-112">TeamMember.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="20916-112">TeamMember.ReadWrite.All</span></span> |
|<span data-ttu-id="20916-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="20916-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="20916-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="20916-114">Not supported.</span></span>    |
|<span data-ttu-id="20916-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="20916-115">Application</span></span>| <span data-ttu-id="20916-116">TeamMember.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="20916-116">TeamMember.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="20916-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="20916-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /teams/{team-id}/members/{membership-id}
```

## <a name="request-headers"></a><span data-ttu-id="20916-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="20916-118">Request headers</span></span>
|<span data-ttu-id="20916-119">Nome</span><span class="sxs-lookup"><span data-stu-id="20916-119">Name</span></span>|<span data-ttu-id="20916-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="20916-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="20916-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="20916-121">Authorization</span></span>|<span data-ttu-id="20916-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="20916-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="20916-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="20916-124">Request body</span></span>
<span data-ttu-id="20916-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="20916-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="20916-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="20916-126">Response</span></span>

<span data-ttu-id="20916-127">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="20916-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="20916-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="20916-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="20916-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="20916-129">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="20916-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="20916-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_members_from_team"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/teams/ee0f5ae2-8bc6-4ae5-8466-7daeebbfa062/members/ZWUwZjVhZTItOGJjNi00YWU1LTg0NjYtN2RhZWViYmZhMDYyIyM3Mzc2MWYwNi0yYWM5LTQ2OWMtOWYxMC0yNzlhOGNjMjY3Zjk=
```
# <a name="c"></a>[<span data-ttu-id="20916-131">C#</span><span class="sxs-lookup"><span data-stu-id="20916-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-members-from-team-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="20916-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="20916-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-members-from-team-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="20916-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="20916-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-members-from-team-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="20916-134">Java</span><span class="sxs-lookup"><span data-stu-id="20916-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-members-from-team-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="20916-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="20916-135">Response</span></span>
<span data-ttu-id="20916-136">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="20916-136">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

## <a name="see-also"></a><span data-ttu-id="20916-137">Confira também</span><span class="sxs-lookup"><span data-stu-id="20916-137">See also</span></span>

- [<span data-ttu-id="20916-138">Remover membro do canal</span><span class="sxs-lookup"><span data-stu-id="20916-138">Remove member from channel</span></span>](channel-delete-members.md)

