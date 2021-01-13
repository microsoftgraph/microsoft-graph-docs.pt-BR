---
title: Obter teamworkBot
description: Leia as propriedades e os relacionamentos de um objeto teamworkBot.
author: AkJo
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: b0c0eaecb59140450d365c0eee931156b8b99e16
ms.sourcegitcommit: a9731e19589dcb5c0c6fe2e24b008c86573ef803
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/13/2021
ms.locfileid: "49844701"
---
# <a name="get-teamworkbot"></a><span data-ttu-id="30283-103">Obter teamworkBot</span><span class="sxs-lookup"><span data-stu-id="30283-103">Get teamworkBot</span></span>

<span data-ttu-id="30283-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="30283-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="30283-105">Obter o bot associado a uma definição [específica](../resources/teamsappdefinition.md) do  [TeamsApp](../resources/teamsapp.md).</span><span class="sxs-lookup"><span data-stu-id="30283-105">Get the bot associated with a specific [definition](../resources/teamsappdefinition.md) of the  [TeamsApp](../resources/teamsapp.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="30283-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="30283-106">Permissions</span></span>
<span data-ttu-id="30283-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="30283-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="30283-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="30283-109">Permission type</span></span>|<span data-ttu-id="30283-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="30283-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="30283-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="30283-111">Delegated (work or school account)</span></span>| <span data-ttu-id="30283-112">AppCatalog.Submit, AppCatalog.Read.All, AppCatalog.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="30283-112">AppCatalog.Submit, AppCatalog.Read.All, AppCatalog.ReadWrite.All</span></span> |
|<span data-ttu-id="30283-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="30283-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="30283-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="30283-114">Not supported.</span></span> |
|<span data-ttu-id="30283-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="30283-115">Application</span></span>| <span data-ttu-id="30283-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="30283-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="30283-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="30283-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /appCatalogs/teamsApps/{app-id}/appDefinitions/{app-definition-id}/bot
```

## <a name="optional-query-parameters"></a><span data-ttu-id="30283-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="30283-118">Optional query parameters</span></span>
<span data-ttu-id="30283-119">Este método dá suporte a `$select` [Parâmetros de consulta OData](/graph/query-parameter) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="30283-119">This method supports the `$select` [OData query parameters](/graph/query-parameter) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="30283-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="30283-120">Request headers</span></span>
|<span data-ttu-id="30283-121">Nome</span><span class="sxs-lookup"><span data-stu-id="30283-121">Name</span></span>|<span data-ttu-id="30283-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="30283-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="30283-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="30283-123">Authorization</span></span>|<span data-ttu-id="30283-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="30283-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="30283-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="30283-126">Request body</span></span>
<span data-ttu-id="30283-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="30283-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="30283-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="30283-128">Response</span></span>

<span data-ttu-id="30283-129">Se bem-sucedido, este método retorna um código de resposta e um objeto `200 OK` [teamworkBot](../resources/teamworkbot.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="30283-129">If successful, this method returns a `200 OK` response code and a [teamworkBot](../resources/teamworkbot.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="30283-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="30283-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="30283-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="30283-131">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="30283-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="30283-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_teamworkbot"
}
-->
``` http
GET https://graph.microsoft.com/beta/appCatalogs/teamsApps/e4c5c249-bb4b-419e-b7c5-b1d98559368b/appDefinitions/ZTRjNWMyNDktYmI0Yi00MTllLWI3YzUtYjFkOTg1NTkzNjhiIyMyLjAuMSMjUHVibGlzaGVk/bot
```
# <a name="c"></a>[<span data-ttu-id="30283-133">C#</span><span class="sxs-lookup"><span data-stu-id="30283-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-teamworkbot-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="30283-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="30283-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-teamworkbot-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="30283-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="30283-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-teamworkbot-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="30283-136">Java</span><span class="sxs-lookup"><span data-stu-id="30283-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-teamworkbot-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="30283-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="30283-137">Response</span></span>
<span data-ttu-id="30283-138">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="30283-138">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.teamworkBot"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.teamworkBot",
  "id": "1f81bb29-bb29-1f81-29bb-811f29bb811f"
}
```
## <a name="see-also"></a><span data-ttu-id="30283-139">Confira também</span><span class="sxs-lookup"><span data-stu-id="30283-139">See also</span></span>

- <span data-ttu-id="30283-140">Para instalar bots em uma equipe, confira o exemplo 2 em [Listar aplicativos em equipe.](team-list-installedapps.md)</span><span class="sxs-lookup"><span data-stu-id="30283-140">To get bots installed in a team, see example 2 in [List apps in team](team-list-installedapps.md).</span></span>
- <span data-ttu-id="30283-141">Para instalar bots em um chat, confira o exemplo 2 em Aplicativos [de lista no chat.](chat-list-installedapps.md)</span><span class="sxs-lookup"><span data-stu-id="30283-141">To get bots installed in a chat, see example 2 in [List apps in chat](chat-list-installedapps.md).</span></span>
- <span data-ttu-id="30283-142">Para instalar bots no escopo pessoal de um usuário, confira o exemplo 2 em Aplicativos de [lista instalados para o usuário.](userteamwork-list-installedapps.md)</span><span class="sxs-lookup"><span data-stu-id="30283-142">To get bots installed in the personal scope of a user, see example 2 in [List apps installed for user](userteamwork-list-installedapps.md).</span></span>


