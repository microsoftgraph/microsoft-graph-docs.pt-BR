---
title: Obter chat entre o usuário e o teamsApp
description: Recupere o chat de um em um entre o usuário especificado e o aplicativo Teams.
author: AkJo
doc_type: apiPageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 0e9776b48fcfc64d3a3b1a1f9c5eb49f704adfc2
ms.sourcegitcommit: 958b540f118ef3ce64d4d4e96b29264e2b56d703
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2020
ms.locfileid: "49564145"
---
# <a name="get-chat-between-user-and-teamsapp"></a><span data-ttu-id="9e9e2-103">Obter chat entre o usuário e o teamsApp</span><span class="sxs-lookup"><span data-stu-id="9e9e2-103">Get chat between user and teamsApp</span></span>

<span data-ttu-id="9e9e2-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9e9e2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9e9e2-105">Recupere o [chat](../resources/chat.md) do [usuário](../resources/user.md) especificado e o [aplicativo Teams](../resources/teamsapp.md).</span><span class="sxs-lookup"><span data-stu-id="9e9e2-105">Retrieve the [chat](../resources/chat.md) of the specified [user](../resources/user.md) and [Teams app](../resources/teamsapp.md).</span></span>

## <a name="http-request"></a><span data-ttu-id="9e9e2-106">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9e9e2-106">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /users/{id}/teamwork/installedApps/{id}/chat
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9e9e2-107">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="9e9e2-107">Optional query parameters</span></span>

<span data-ttu-id="9e9e2-108">Este método oferece suporte ao `$select` [parâmetro de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="9e9e2-108">This method supports the `$select` [OData query parameter](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9e9e2-109">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9e9e2-109">Request headers</span></span>

| <span data-ttu-id="9e9e2-110">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9e9e2-110">Header</span></span>       | <span data-ttu-id="9e9e2-111">Valor</span><span class="sxs-lookup"><span data-stu-id="9e9e2-111">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="9e9e2-112">Autorização</span><span class="sxs-lookup"><span data-stu-id="9e9e2-112">Authorization</span></span>  | <span data-ttu-id="9e9e2-p101">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9e9e2-p101">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="9e9e2-115">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9e9e2-115">Request body</span></span>

<span data-ttu-id="9e9e2-116">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="9e9e2-116">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9e9e2-117">Resposta</span><span class="sxs-lookup"><span data-stu-id="9e9e2-117">Response</span></span>

<span data-ttu-id="9e9e2-118">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma instância do objeto [chat](../resources/chat.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9e9e2-118">If successful, this method returns a `200 OK` response code and an instance of [chat](../resources/chat.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="9e9e2-119">Exemplos</span><span class="sxs-lookup"><span data-stu-id="9e9e2-119">Examples</span></span>

### <a name="example-1-list-one-on-one-chats-between-the-specified-user-and-the-teams-app"></a><span data-ttu-id="9e9e2-120">Exemplo 1: listar chats um-on-one entre o usuário especificado e o aplicativo Teams</span><span class="sxs-lookup"><span data-stu-id="9e9e2-120">Example 1: List one-on-one chats between the specified user and the Teams app</span></span>

#### <a name="request"></a><span data-ttu-id="9e9e2-121">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9e9e2-121">Request</span></span>

<span data-ttu-id="9e9e2-122">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="9e9e2-122">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "user_chat_teamsApps"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/{id}/teamwork/installedApps/{id}/chat
```

#### <a name="response"></a><span data-ttu-id="9e9e2-123">Resposta</span><span class="sxs-lookup"><span data-stu-id="9e9e2-123">Response</span></span>

<span data-ttu-id="9e9e2-124">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="9e9e2-124">The following is an example of the response.</span></span>
><span data-ttu-id="9e9e2-p102">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9e9e2-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
   "@odata.context": "https://graph.microsoft.com/beta/$metadata#chats/$entity",
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
