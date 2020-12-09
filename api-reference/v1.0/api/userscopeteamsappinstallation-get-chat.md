---
title: Obter o chat 1:1 entre o usuário especificado e o aplicativo de equipes
description: Recupere o chat de um em um entre o usuário especificado e o aplicativo Teams.
author: AkJo
doc_type: apiPageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 3a216a04d55dda0c87af497fadb3403f7a4b1055
ms.sourcegitcommit: 59e79cf2693cbb550da3e61eb4f68d9e0f57faf6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/09/2020
ms.locfileid: "49606992"
---
# <a name="get-one-on-one-chat-between-the-specified-user-and-teams-app"></a><span data-ttu-id="3dec4-103">Obter chat de um em um entre o usuário especificado e o aplicativo de equipes</span><span class="sxs-lookup"><span data-stu-id="3dec4-103">Get one-on-one chat between the specified user and Teams app</span></span>

<span data-ttu-id="3dec4-104">Namespace: Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="3dec4-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="3dec4-105">Recupere o [chat](../resources/chat.md) do [usuário](../resources/user.md) especificado e o [aplicativo Teams](../resources/teamsapp.md).</span><span class="sxs-lookup"><span data-stu-id="3dec4-105">Retrieve the [chat](../resources/chat.md) of the specified [user](../resources/user.md) and [Teams app](../resources/teamsapp.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="3dec4-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="3dec4-106">Permissions</span></span>

<span data-ttu-id="3dec4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3dec4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3dec4-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3dec4-109">Permission type</span></span>      | <span data-ttu-id="3dec4-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3dec4-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3dec4-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3dec4-111">Delegated (work or school account)</span></span> | <span data-ttu-id="3dec4-112">TeamsAppInstallation.ReadForUser, TeamsAppInstallation.ReadWriteSelfForUser, TeamsAppInstallation.ReadWriteForUser</span><span class="sxs-lookup"><span data-stu-id="3dec4-112">TeamsAppInstallation.ReadForUser, TeamsAppInstallation.ReadWriteSelfForUser, TeamsAppInstallation.ReadWriteForUser</span></span> |
|<span data-ttu-id="3dec4-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3dec4-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3dec4-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3dec4-114">Not supported.</span></span>    |
|<span data-ttu-id="3dec4-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3dec4-115">Application</span></span> | <span data-ttu-id="3dec4-116">TeamsAppInstallation. ReadForUser. All, TeamsAppInstallation. ReadWriteSelfForUser. All, TeamsAppInstallation. ReadWriteForUser. All</span><span class="sxs-lookup"><span data-stu-id="3dec4-116">TeamsAppInstallation.ReadForUser.All, TeamsAppInstallation.ReadWriteSelfForUser.All, TeamsAppInstallation.ReadWriteForUser.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3dec4-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3dec4-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /users/{user-id}/teamwork/installedApps/{app-installation-id}/chat
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3dec4-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="3dec4-118">Optional query parameters</span></span>

<span data-ttu-id="3dec4-119">Este método oferece suporte ao `$select` [parâmetro de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="3dec4-119">This method supports the `$select` [OData query parameter](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3dec4-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3dec4-120">Request headers</span></span>

| <span data-ttu-id="3dec4-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3dec4-121">Header</span></span>       | <span data-ttu-id="3dec4-122">Valor</span><span class="sxs-lookup"><span data-stu-id="3dec4-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="3dec4-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="3dec4-123">Authorization</span></span>  | <span data-ttu-id="3dec4-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3dec4-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="3dec4-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3dec4-126">Request body</span></span>

<span data-ttu-id="3dec4-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3dec4-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3dec4-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="3dec4-128">Response</span></span>

<span data-ttu-id="3dec4-129">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma instância do objeto [chat](../resources/chat.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3dec4-129">If successful, this method returns a `200 OK` response code and an instance of [chat](../resources/chat.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="3dec4-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="3dec4-130">Examples</span></span>

### <a name="example-1-list-one-on-one-chats-between-the-specified-user-and-the-teams-app"></a><span data-ttu-id="3dec4-131">Exemplo 1: listar chats um-on-one entre o usuário especificado e o aplicativo Teams</span><span class="sxs-lookup"><span data-stu-id="3dec4-131">Example 1: List one-on-one chats between the specified user and the Teams app</span></span>

#### <a name="request"></a><span data-ttu-id="3dec4-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3dec4-132">Request</span></span>

<span data-ttu-id="3dec4-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="3dec4-133">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "user_chat_teamsApps"
}-->
```http
GET https://graph.microsoft.com/beta/users/f32b83bb-4fc8-4db7-b7f5-76cdbbb8aa1c/teamwork/installedApps/ZjMyYjgzYmItNGZjOC00ZGI3LWI3ZjUtNzZjZGJiYjhhYTFjIyMyMmY3M2JiZS1mNjdhLTRkZWEtYmQ1NC01NGNhYzcxOGNiMmI=/chat
```

#### <a name="response"></a><span data-ttu-id="3dec4-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="3dec4-134">Response</span></span>

<span data-ttu-id="3dec4-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="3dec4-135">The following is an example of the response.</span></span>
><span data-ttu-id="3dec4-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3dec4-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
   "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#chats/$entity",
   "id": "19:0de69e5e-2da8-4cf2-821f-5e6585b2c65b_f32b83bb-4fc8-4db7-b7f5-76cdbbb8aa1c@unq.gbl.spaces"
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
