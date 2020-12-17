---
title: Obter teamworkBot
description: Leia as propriedades e os relacionamentos de um objeto teamworkBot.
author: AkJo
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 33a6312474994ff65397f6d09b416d15560bb08c
ms.sourcegitcommit: ee9e594ad64bef5bc839cf813c0854d083c00aef
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/17/2020
ms.locfileid: "49706252"
---
# <a name="get-teamworkbot"></a><span data-ttu-id="ffa45-103">Obter teamworkBot</span><span class="sxs-lookup"><span data-stu-id="ffa45-103">Get teamworkBot</span></span>
<span data-ttu-id="ffa45-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ffa45-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ffa45-105">Obter o bot associado a uma [definição](../resources/teamsappdefinition.md) específica do  [TeamsApp](../resources/teamsapp.md).</span><span class="sxs-lookup"><span data-stu-id="ffa45-105">Get the bot associated with a specific [definition](../resources/teamsappdefinition.md) of the  [TeamsApp](../resources/teamsapp.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="ffa45-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="ffa45-106">Permissions</span></span>
<span data-ttu-id="ffa45-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ffa45-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ffa45-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ffa45-109">Permission type</span></span>|<span data-ttu-id="ffa45-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ffa45-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ffa45-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ffa45-111">Delegated (work or school account)</span></span>| <span data-ttu-id="ffa45-112">AppCatalog. Submit, AppCatalog. Read. All, AppCatalog. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="ffa45-112">AppCatalog.Submit, AppCatalog.Read.All, AppCatalog.ReadWrite.All</span></span> |
|<span data-ttu-id="ffa45-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ffa45-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="ffa45-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ffa45-114">Not supported.</span></span> |
|<span data-ttu-id="ffa45-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ffa45-115">Application</span></span>| <span data-ttu-id="ffa45-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ffa45-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ffa45-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ffa45-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /appCatalogs/teamsApps/{app-id}/appDefinitions/{app-definition-id}/bot
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ffa45-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="ffa45-118">Optional query parameters</span></span>
<span data-ttu-id="ffa45-119">Este método dá suporte a `$select` [Parâmetros de consulta OData](/graph/query-parameter) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="ffa45-119">This method supports the `$select` [OData query parameters](/graph/query-parameter) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ffa45-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ffa45-120">Request headers</span></span>
|<span data-ttu-id="ffa45-121">Nome</span><span class="sxs-lookup"><span data-stu-id="ffa45-121">Name</span></span>|<span data-ttu-id="ffa45-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="ffa45-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="ffa45-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="ffa45-123">Authorization</span></span>|<span data-ttu-id="ffa45-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ffa45-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ffa45-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ffa45-126">Request body</span></span>
<span data-ttu-id="ffa45-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ffa45-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ffa45-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="ffa45-128">Response</span></span>

<span data-ttu-id="ffa45-129">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [teamworkBot](../resources/teamworkbot.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ffa45-129">If successful, this method returns a `200 OK` response code and a [teamworkBot](../resources/teamworkbot.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ffa45-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="ffa45-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ffa45-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ffa45-131">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_teamworkbot"
}
-->
``` http
GET https://graph.microsoft.com/beta/appCatalogs/teamsApps/e4c5c249-bb4b-419e-b7c5-b1d98559368b/appDefinitions/ZTRjNWMyNDktYmI0Yi00MTllLWI3YzUtYjFkOTg1NTkzNjhiIyMyLjAuMSMjUHVibGlzaGVk/bot
```


### <a name="response"></a><span data-ttu-id="ffa45-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="ffa45-132">Response</span></span>
<span data-ttu-id="ffa45-133">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="ffa45-133">**Note:** The response object shown here might be shortened for readability.</span></span>
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
## <a name="see-also"></a><span data-ttu-id="ffa45-134">Confira também</span><span class="sxs-lookup"><span data-stu-id="ffa45-134">See also</span></span>

- <span data-ttu-id="ffa45-135">Para obter bots instalados em uma equipe, confira o exemplo 2 em [list apps in Team](team-list-installedapps.md).</span><span class="sxs-lookup"><span data-stu-id="ffa45-135">To get bots installed in a team, see example 2 in [List apps in team](team-list-installedapps.md).</span></span>
- <span data-ttu-id="ffa45-136">Para obter bots instalados em um chat, confira o exemplo 2 em [listar aplicativos no chat](chat-list-installedapps.md).</span><span class="sxs-lookup"><span data-stu-id="ffa45-136">To get bots installed in a chat, see example 2 in [List apps in chat](chat-list-installedapps.md).</span></span>
- <span data-ttu-id="ffa45-137">Para obter bots instalados no escopo pessoal de um usuário, confira o exemplo 2 em [listar aplicativos instalados para o usuário](userteamwork-list-installedapps.md).</span><span class="sxs-lookup"><span data-stu-id="ffa45-137">To get bots installed in the personal scope of a user, see example 2 in [List apps installed for user](userteamwork-list-installedapps.md).</span></span>


