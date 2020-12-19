---
title: Obter o chat 1:1 entre o usuário especificado e o aplicativo de equipes
description: Recupere o chat de um em um entre o usuário especificado e o aplicativo Teams.
author: AkJo
doc_type: apiPageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 29c13e3c58cd7285146ffc80845496540146c6d1
ms.sourcegitcommit: ee9e594ad64bef5bc839cf813c0854d083c00aef
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/17/2020
ms.locfileid: "49706154"
---
# <a name="get-one-on-one-chat-between-the-specified-user-and-teams-app"></a><span data-ttu-id="0de88-103">Obter chat de um em um entre o usuário especificado e o aplicativo de equipes</span><span class="sxs-lookup"><span data-stu-id="0de88-103">Get one-on-one chat between the specified user and Teams app</span></span>

<span data-ttu-id="0de88-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0de88-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="0de88-105">Recupere o [chat](../resources/chat.md) do [usuário](../resources/user.md) especificado e o [aplicativo Teams](../resources/teamsapp.md).</span><span class="sxs-lookup"><span data-stu-id="0de88-105">Retrieve the [chat](../resources/chat.md) of the specified [user](../resources/user.md) and [Teams app](../resources/teamsapp.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="0de88-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="0de88-106">Permissions</span></span>

<span data-ttu-id="0de88-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0de88-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0de88-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0de88-109">Permission type</span></span>      | <span data-ttu-id="0de88-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0de88-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0de88-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0de88-111">Delegated (work or school account)</span></span> | <span data-ttu-id="0de88-112">TeamsAppInstallation.ReadForUser, TeamsAppInstallation.ReadWriteSelfForUser, TeamsAppInstallation.ReadWriteForUser</span><span class="sxs-lookup"><span data-stu-id="0de88-112">TeamsAppInstallation.ReadForUser, TeamsAppInstallation.ReadWriteSelfForUser, TeamsAppInstallation.ReadWriteForUser</span></span> |
|<span data-ttu-id="0de88-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0de88-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0de88-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0de88-114">Not supported.</span></span>    |
|<span data-ttu-id="0de88-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0de88-115">Application</span></span> | <span data-ttu-id="0de88-116">TeamsAppInstallation. ReadForUser. All, TeamsAppInstallation. ReadWriteSelfForUser. All, TeamsAppInstallation. ReadWriteForUser. All</span><span class="sxs-lookup"><span data-stu-id="0de88-116">TeamsAppInstallation.ReadForUser.All, TeamsAppInstallation.ReadWriteSelfForUser.All, TeamsAppInstallation.ReadWriteForUser.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0de88-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0de88-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /users/{user-id}/teamwork/installedApps/{app-installation-id}/chat
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0de88-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="0de88-118">Optional query parameters</span></span>

<span data-ttu-id="0de88-119">Este método oferece suporte ao `$select` [parâmetro de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="0de88-119">This method supports the `$select` [OData query parameter](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0de88-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0de88-120">Request headers</span></span>

| <span data-ttu-id="0de88-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0de88-121">Header</span></span>       | <span data-ttu-id="0de88-122">Valor</span><span class="sxs-lookup"><span data-stu-id="0de88-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="0de88-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="0de88-123">Authorization</span></span>  | <span data-ttu-id="0de88-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0de88-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="0de88-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0de88-126">Request body</span></span>

<span data-ttu-id="0de88-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="0de88-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0de88-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="0de88-128">Response</span></span>

<span data-ttu-id="0de88-129">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma instância do objeto [chat](../resources/chat.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0de88-129">If successful, this method returns a `200 OK` response code and an instance of [chat](../resources/chat.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="0de88-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="0de88-130">Examples</span></span>

### <a name="example-1-list-one-on-one-chats-between-the-specified-user-and-the-teams-app"></a><span data-ttu-id="0de88-131">Exemplo 1: listar chats um-on-one entre o usuário especificado e o aplicativo Teams</span><span class="sxs-lookup"><span data-stu-id="0de88-131">Example 1: List one-on-one chats between the specified user and the Teams app</span></span>

#### <a name="request"></a><span data-ttu-id="0de88-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0de88-132">Request</span></span>

<span data-ttu-id="0de88-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="0de88-133">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="0de88-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="0de88-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_chat_teamsApps"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/f32b83bb-4fc8-4db7-b7f5-76cdbbb8aa1c/teamwork/installedApps/ZjMyYjgzYmItNGZjOC00ZGI3LWI3ZjUtNzZjZGJiYjhhYTFjIyMyMmY3M2JiZS1mNjdhLTRkZWEtYmQ1NC01NGNhYzcxOGNiMmI=/chat
```
# <a name="c"></a>[<span data-ttu-id="0de88-135">C#</span><span class="sxs-lookup"><span data-stu-id="0de88-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-chat-teamsapps-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0de88-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0de88-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-chat-teamsapps-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0de88-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0de88-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-chat-teamsapps-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0de88-138">Java</span><span class="sxs-lookup"><span data-stu-id="0de88-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-chat-teamsapps-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="0de88-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="0de88-139">Response</span></span>

<span data-ttu-id="0de88-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="0de88-140">The following is an example of the response.</span></span>
><span data-ttu-id="0de88-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0de88-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
   "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#chats/$entity",
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
