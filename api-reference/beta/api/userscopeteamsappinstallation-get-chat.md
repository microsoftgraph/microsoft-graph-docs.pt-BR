---
title: Obter chat entre o usuário e o teamsApp
description: Recupere o chat de um em um entre o usuário especificado e o aplicativo Teams.
author: AkJo
doc_type: apiPageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: cc0be0eb80b35c17b2f0ea6ba38b4dbf1673ac37
ms.sourcegitcommit: 59e79cf2693cbb550da3e61eb4f68d9e0f57faf6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/09/2020
ms.locfileid: "49607207"
---
# <a name="get-chat-between-user-and-teamsapp"></a><span data-ttu-id="6634d-103">Obter chat entre o usuário e o teamsApp</span><span class="sxs-lookup"><span data-stu-id="6634d-103">Get chat between user and teamsApp</span></span>

<span data-ttu-id="6634d-104">Namespace: Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="6634d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6634d-105">Recupere o [chat](../resources/chat.md) do [usuário](../resources/user.md) especificado e o [aplicativo Teams](../resources/teamsapp.md).</span><span class="sxs-lookup"><span data-stu-id="6634d-105">Retrieve the [chat](../resources/chat.md) of the specified [user](../resources/user.md) and [Teams app](../resources/teamsapp.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="6634d-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="6634d-106">Permissions</span></span>

<span data-ttu-id="6634d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6634d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6634d-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6634d-109">Permission type</span></span>      | <span data-ttu-id="6634d-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6634d-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6634d-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6634d-111">Delegated (work or school account)</span></span> | <span data-ttu-id="6634d-112">TeamsAppInstallation.ReadForUser, TeamsAppInstallation.ReadWriteSelfForUser, TeamsAppInstallation.ReadWriteForUser</span><span class="sxs-lookup"><span data-stu-id="6634d-112">TeamsAppInstallation.ReadForUser, TeamsAppInstallation.ReadWriteSelfForUser, TeamsAppInstallation.ReadWriteForUser</span></span> |
|<span data-ttu-id="6634d-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6634d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6634d-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6634d-114">Not supported.</span></span>    |
|<span data-ttu-id="6634d-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6634d-115">Application</span></span> | <span data-ttu-id="6634d-116">TeamsAppInstallation. ReadForUser. All, TeamsAppInstallation. ReadWriteSelfForUser. All, TeamsAppInstallation. ReadWriteForUser. All</span><span class="sxs-lookup"><span data-stu-id="6634d-116">TeamsAppInstallation.ReadForUser.All, TeamsAppInstallation.ReadWriteSelfForUser.All, TeamsAppInstallation.ReadWriteForUser.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6634d-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6634d-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /users/{user-id}/teamwork/installedApps/{app-installation-id}/chat
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6634d-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="6634d-118">Optional query parameters</span></span>

<span data-ttu-id="6634d-119">Este método oferece suporte ao `$select` [parâmetro de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="6634d-119">This method supports the `$select` [OData query parameter](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6634d-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6634d-120">Request headers</span></span>

| <span data-ttu-id="6634d-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6634d-121">Header</span></span>       | <span data-ttu-id="6634d-122">Valor</span><span class="sxs-lookup"><span data-stu-id="6634d-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="6634d-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="6634d-123">Authorization</span></span>  | <span data-ttu-id="6634d-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6634d-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="6634d-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6634d-126">Request body</span></span>

<span data-ttu-id="6634d-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="6634d-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6634d-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="6634d-128">Response</span></span>

<span data-ttu-id="6634d-129">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma instância do objeto [chat](../resources/chat.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6634d-129">If successful, this method returns a `200 OK` response code and an instance of [chat](../resources/chat.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6634d-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="6634d-130">Examples</span></span>

### <a name="example-1-list-one-on-one-chats-between-the-specified-user-and-the-teams-app"></a><span data-ttu-id="6634d-131">Exemplo 1: listar chats um-on-one entre o usuário especificado e o aplicativo Teams</span><span class="sxs-lookup"><span data-stu-id="6634d-131">Example 1: List one-on-one chats between the specified user and the Teams app</span></span>

#### <a name="request"></a><span data-ttu-id="6634d-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6634d-132">Request</span></span>

<span data-ttu-id="6634d-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="6634d-133">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "user_chat_teamsApps"
}-->
```http
GET https://graph.microsoft.com/beta/users/f32b83bb-4fc8-4db7-b7f5-76cdbbb8aa1c/teamwork/installedApps/ZjMyYjgzYmItNGZjOC00ZGI3LWI3ZjUtNzZjZGJiYjhhYTFjIyMyMmY3M2JiZS1mNjdhLTRkZWEtYmQ1NC01NGNhYzcxOGNiMmI=/chat
```

#### <a name="response"></a><span data-ttu-id="6634d-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="6634d-134">Response</span></span>

<span data-ttu-id="6634d-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="6634d-135">The following is an example of the response.</span></span>
><span data-ttu-id="6634d-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6634d-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
