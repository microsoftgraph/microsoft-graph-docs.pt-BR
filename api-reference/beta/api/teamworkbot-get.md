---
title: Obter teamworkBot
description: Leia as propriedades e os relacionamentos de um objeto teamworkBot.
author: AkJo
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 05cb2e8e4d6a41028a9f35b82561b4f5b5d80251
ms.sourcegitcommit: de175a11806f9e9ba3c916384e897aee1cc7f75c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/09/2021
ms.locfileid: "49790584"
---
# <a name="get-teamworkbot"></a><span data-ttu-id="bb1fb-103">Obter teamworkBot</span><span class="sxs-lookup"><span data-stu-id="bb1fb-103">Get teamworkBot</span></span>

<span data-ttu-id="bb1fb-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bb1fb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bb1fb-105">Obter o bot associado a uma definição [específica](../resources/teamsappdefinition.md) do  [TeamsApp](../resources/teamsapp.md).</span><span class="sxs-lookup"><span data-stu-id="bb1fb-105">Get the bot associated with a specific [definition](../resources/teamsappdefinition.md) of the  [TeamsApp](../resources/teamsapp.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="bb1fb-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="bb1fb-106">Permissions</span></span>
<span data-ttu-id="bb1fb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bb1fb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bb1fb-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bb1fb-109">Permission type</span></span>|<span data-ttu-id="bb1fb-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="bb1fb-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bb1fb-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bb1fb-111">Delegated (work or school account)</span></span>| <span data-ttu-id="bb1fb-112">AppCatalog.Submit, AppCatalog.Read.All, AppCatalog.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bb1fb-112">AppCatalog.Submit, AppCatalog.Read.All, AppCatalog.ReadWrite.All</span></span> |
|<span data-ttu-id="bb1fb-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bb1fb-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="bb1fb-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bb1fb-114">Not supported.</span></span> |
|<span data-ttu-id="bb1fb-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bb1fb-115">Application</span></span>| <span data-ttu-id="bb1fb-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bb1fb-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bb1fb-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bb1fb-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /appCatalogs/teamsApps/{app-id}/appDefinitions/{app-definition-id}/bot
```

## <a name="optional-query-parameters"></a><span data-ttu-id="bb1fb-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="bb1fb-118">Optional query parameters</span></span>
<span data-ttu-id="bb1fb-119">Esse método dá suporte aos parâmetros de `$select` [consulta OData](/graph/query-parameter) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="bb1fb-119">This method supports the `$select` [OData query parameters](/graph/query-parameter) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="bb1fb-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bb1fb-120">Request headers</span></span>
|<span data-ttu-id="bb1fb-121">Nome</span><span class="sxs-lookup"><span data-stu-id="bb1fb-121">Name</span></span>|<span data-ttu-id="bb1fb-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="bb1fb-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="bb1fb-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="bb1fb-123">Authorization</span></span>|<span data-ttu-id="bb1fb-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bb1fb-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="bb1fb-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bb1fb-126">Request body</span></span>
<span data-ttu-id="bb1fb-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="bb1fb-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bb1fb-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="bb1fb-128">Response</span></span>

<span data-ttu-id="bb1fb-129">Se bem-sucedido, este método retorna um código de resposta e um objeto `200 OK` [teamworkBot](../resources/teamworkbot.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bb1fb-129">If successful, this method returns a `200 OK` response code and a [teamworkBot](../resources/teamworkbot.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="bb1fb-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="bb1fb-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="bb1fb-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bb1fb-131">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_teamworkbot"
}
-->
``` http
GET https://graph.microsoft.com/beta/appCatalogs/teamsApps/e4c5c249-bb4b-419e-b7c5-b1d98559368b/appDefinitions/ZTRjNWMyNDktYmI0Yi00MTllLWI3YzUtYjFkOTg1NTkzNjhiIyMyLjAuMSMjUHVibGlzaGVk/bot
```


### <a name="response"></a><span data-ttu-id="bb1fb-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="bb1fb-132">Response</span></span>
<span data-ttu-id="bb1fb-133">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="bb1fb-133">**Note:** The response object shown here might be shortened for readability.</span></span>
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
## <a name="see-also"></a><span data-ttu-id="bb1fb-134">Confira também</span><span class="sxs-lookup"><span data-stu-id="bb1fb-134">See also</span></span>

- <span data-ttu-id="bb1fb-135">Para instalar bots em uma equipe, confira o exemplo 2 em [Listar aplicativos em equipe.](team-list-installedapps.md)</span><span class="sxs-lookup"><span data-stu-id="bb1fb-135">To get bots installed in a team, see example 2 in [List apps in team](team-list-installedapps.md).</span></span>
- <span data-ttu-id="bb1fb-136">Para instalar bots em um chat, confira o exemplo 2 em Aplicativos [de lista no chat.](chat-list-installedapps.md)</span><span class="sxs-lookup"><span data-stu-id="bb1fb-136">To get bots installed in a chat, see example 2 in [List apps in chat](chat-list-installedapps.md).</span></span>
- <span data-ttu-id="bb1fb-137">Para instalar bots no escopo pessoal de um usuário, confira o exemplo 2 em Aplicativos de [lista instalados para o usuário.](userteamwork-list-installedapps.md)</span><span class="sxs-lookup"><span data-stu-id="bb1fb-137">To get bots installed in the personal scope of a user, see example 2 in [List apps installed for user](userteamwork-list-installedapps.md).</span></span>


