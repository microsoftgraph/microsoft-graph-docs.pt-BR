---
title: Obter chat entre usuário e teamsApp
description: Recupere o chat um-a-um entre o usuário especificado e o Teams aplicativo.
author: AkJo
doc_type: apiPageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: cde0931caf5509c9782e7da9fdb4691eafa4eb67
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52052576"
---
# <a name="get-chat-between-user-and-teamsapp"></a><span data-ttu-id="abc7f-103">Obter chat entre usuário e teamsApp</span><span class="sxs-lookup"><span data-stu-id="abc7f-103">Get chat between user and teamsApp</span></span>

<span data-ttu-id="abc7f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="abc7f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="abc7f-105">Recupere o [chat](../resources/chat.md) do usuário especificado [e](../resources/user.md) Teams [app](../resources/teamsapp.md).</span><span class="sxs-lookup"><span data-stu-id="abc7f-105">Retrieve the [chat](../resources/chat.md) of the specified [user](../resources/user.md) and [Teams app](../resources/teamsapp.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="abc7f-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="abc7f-106">Permissions</span></span>

<span data-ttu-id="abc7f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="abc7f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="abc7f-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="abc7f-109">Permission type</span></span>      | <span data-ttu-id="abc7f-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="abc7f-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="abc7f-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="abc7f-111">Delegated (work or school account)</span></span> | <span data-ttu-id="abc7f-112">TeamsAppInstallation.ReadForUser, TeamsAppInstallation.ReadWriteSelfForUser, TeamsAppInstallation.ReadWriteForUser</span><span class="sxs-lookup"><span data-stu-id="abc7f-112">TeamsAppInstallation.ReadForUser, TeamsAppInstallation.ReadWriteSelfForUser, TeamsAppInstallation.ReadWriteForUser</span></span> |
|<span data-ttu-id="abc7f-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="abc7f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="abc7f-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="abc7f-114">Not supported.</span></span>    |
|<span data-ttu-id="abc7f-115">Application</span><span class="sxs-lookup"><span data-stu-id="abc7f-115">Application</span></span> | <span data-ttu-id="abc7f-116">TeamsAppInstallation.ReadForUser.All, TeamsAppInstallation.ReadWriteSelfForUser.All, TeamsAppInstallation.ReadWriteForUser.All</span><span class="sxs-lookup"><span data-stu-id="abc7f-116">TeamsAppInstallation.ReadForUser.All, TeamsAppInstallation.ReadWriteSelfForUser.All, TeamsAppInstallation.ReadWriteForUser.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="abc7f-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="abc7f-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /users/{user-id}/teamwork/installedApps/{app-installation-id}/chat
```

## <a name="optional-query-parameters"></a><span data-ttu-id="abc7f-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="abc7f-118">Optional query parameters</span></span>

<span data-ttu-id="abc7f-119">Este método dá suporte ao `$select` [parâmetro de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="abc7f-119">This method supports the `$select` [OData query parameter](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="abc7f-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="abc7f-120">Request headers</span></span>

| <span data-ttu-id="abc7f-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="abc7f-121">Header</span></span>       | <span data-ttu-id="abc7f-122">Valor</span><span class="sxs-lookup"><span data-stu-id="abc7f-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="abc7f-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="abc7f-123">Authorization</span></span>  | <span data-ttu-id="abc7f-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="abc7f-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="abc7f-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="abc7f-126">Request body</span></span>

<span data-ttu-id="abc7f-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="abc7f-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="abc7f-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="abc7f-128">Response</span></span>

<span data-ttu-id="abc7f-129">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` instância de objeto de [chat](../resources/chat.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="abc7f-129">If successful, this method returns a `200 OK` response code and an instance of [chat](../resources/chat.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="abc7f-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="abc7f-130">Examples</span></span>

### <a name="example-1-list-one-on-one-chats-between-the-specified-user-and-the-teams-app"></a><span data-ttu-id="abc7f-131">Exemplo 1: Listar chats um-a-um entre o usuário especificado e o Teams aplicativo</span><span class="sxs-lookup"><span data-stu-id="abc7f-131">Example 1: List one-on-one chats between the specified user and the Teams app</span></span>

#### <a name="request"></a><span data-ttu-id="abc7f-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="abc7f-132">Request</span></span>

<span data-ttu-id="abc7f-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="abc7f-133">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="abc7f-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="abc7f-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_chat_teamsApps"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/f32b83bb-4fc8-4db7-b7f5-76cdbbb8aa1c/teamwork/installedApps/ZjMyYjgzYmItNGZjOC00ZGI3LWI3ZjUtNzZjZGJiYjhhYTFjIyMyMmY3M2JiZS1mNjdhLTRkZWEtYmQ1NC01NGNhYzcxOGNiMmI=/chat
```
# <a name="c"></a>[<span data-ttu-id="abc7f-135">C#</span><span class="sxs-lookup"><span data-stu-id="abc7f-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-chat-teamsapps-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="abc7f-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="abc7f-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-chat-teamsapps-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="abc7f-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="abc7f-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-chat-teamsapps-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="abc7f-138">Java</span><span class="sxs-lookup"><span data-stu-id="abc7f-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-chat-teamsapps-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="abc7f-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="abc7f-139">Response</span></span>

<span data-ttu-id="abc7f-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="abc7f-140">The following is an example of the response.</span></span>
><span data-ttu-id="abc7f-141">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="abc7f-141">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "name": "user_chat_teamsApps",
  "truncated": true,
  "@odata.type": "microsoft.graph.chat",
  "isCollection": false
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
   "@odata.context":"https://graph.microsoft.com/beta/$metadata#chats/$entity",
   "id":"19:0de69e5e-2da8-4cf2-821f-5e6585b2c65b_f32b83bb-4fc8-4db7-b7f5-76cdbbb8aa1c@unq.gbl.spaces"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "User chat teamsAppInstallations",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
