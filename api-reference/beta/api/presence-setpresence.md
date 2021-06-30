---
title: 'presença: setPresence'
description: De definir as informações de presença para a sessão de presença do aplicativo do usuário.
author: jsandoval-msft
localization_priority: Normal
doc_type: apiPageType
ms.prod: cloud-communications
ms.openlocfilehash: 1e7e90b90ad92ca62327ad9c356fa1d870c7ecbd
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/30/2021
ms.locfileid: "53208271"
---
# <a name="presence-setpresence"></a><span data-ttu-id="c52ab-103">presença: setPresence</span><span class="sxs-lookup"><span data-stu-id="c52ab-103">presence: setPresence</span></span>

<span data-ttu-id="c52ab-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c52ab-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c52ab-105">De definir o estado da sessão de presença de um usuário como um aplicativo.</span><span class="sxs-lookup"><span data-stu-id="c52ab-105">Set the state of a user's presence session as an application.</span></span>

### <a name="presence-sessions"></a><span data-ttu-id="c52ab-106">Sessões de presença</span><span class="sxs-lookup"><span data-stu-id="c52ab-106">Presence sessions</span></span>
<span data-ttu-id="c52ab-107">Um usuário pode ter várias sessões de presença porque o usuário pode estar em vários Teams clientes (desktop, móvel e Web).</span><span class="sxs-lookup"><span data-stu-id="c52ab-107">A user can have multiple presence sessions because the user can be on multiple Teams clients (desktop, mobile, and web).</span></span> <span data-ttu-id="c52ab-108">Cada Teams cliente tem uma sessão de presença independente e a presença do usuário é um estado agregado de todas as sessões atrás.</span><span class="sxs-lookup"><span data-stu-id="c52ab-108">Each Teams client has an independent presence session and the user's presence is an aggregated state from all the sessions behind.</span></span>

<span data-ttu-id="c52ab-109">Da mesma forma, um aplicativo pode ter sua própria sessão de presença para um usuário e ser capaz de atualizar o estado.</span><span class="sxs-lookup"><span data-stu-id="c52ab-109">Similarly, an application can have its own presence session for a user and be able to update the state.</span></span>

<span data-ttu-id="c52ab-110">Veja a seguir a precedência de como os estados de sessão são agregados:</span><span class="sxs-lookup"><span data-stu-id="c52ab-110">The following is the precedence for how session states are aggregated:</span></span>
* <span data-ttu-id="c52ab-111">Configurada pelo usuário > configurada pelo aplicativo (o estado configurado pelo usuário substitui outras pessoas)</span><span class="sxs-lookup"><span data-stu-id="c52ab-111">User-configured > app-configured (user-configured state overrides others)</span></span>
* <span data-ttu-id="c52ab-112">Entre os aplicativos configurados: DoNotDisturb (atualmente sem suporte para a presença definida) > Ocupado > Disponível > Distância</span><span class="sxs-lookup"><span data-stu-id="c52ab-112">Among app-configured: DoNotDisturb (currently not supported for set presence) > Busy > Available > Away</span></span>

### <a name="timeout-expiration-and-keep-alive"></a><span data-ttu-id="c52ab-113">Tempo de expiração, expiração e manter-se vivo</span><span class="sxs-lookup"><span data-stu-id="c52ab-113">Timeout, expiration, and keep alive</span></span>
<span data-ttu-id="c52ab-114">Uma sessão de presença pode **expirar** e **expirar**, portanto, o aplicativo precisa chamar essa API antes do tempo de tempo, para manter o estado da sessão; ou antes da **expiração**, para manter a sessão viva.</span><span class="sxs-lookup"><span data-stu-id="c52ab-114">A presence session may **time out** and **expire**, so the application needs to call this API before the **timeout**, to maintain the state for the session; or before the **expiration**, to keep the session alive.</span></span>

<span data-ttu-id="c52ab-115">Uma sessão de presença pode ser limitada se a disponibilidade for `Available` e o tempo-de-tempo for de 5 minutos.</span><span class="sxs-lookup"><span data-stu-id="c52ab-115">A presence session can time out if the availability is `Available` and the timeout is 5 minutes.</span></span> <span data-ttu-id="c52ab-116">Quando o tempo passa, o estado de presença desaparece em estágios.</span><span class="sxs-lookup"><span data-stu-id="c52ab-116">When it times out, the presence state fades in stages.</span></span> <span data-ttu-id="c52ab-117">Por exemplo, se um aplicativo define a sessão de presença como , o estado será alternado para em 5 minutos com o primeiro tempo de tempo, em seguida, em outros 5 minutos com o `Available/Available` `Available/AvailableInactive` segundo `Away/Away` tempo.</span><span class="sxs-lookup"><span data-stu-id="c52ab-117">For example, if an application sets the presence session as `Available/Available`, the state would change to `Available/AvailableInactive` in 5 minutes with the first timeout, then `Away/Away` in another 5 minutes with the second timeout.</span></span>

<span data-ttu-id="c52ab-118">A expiração de uma sessão de presença é configurável com o `expirationDuration` parâmetro.</span><span class="sxs-lookup"><span data-stu-id="c52ab-118">The expiration of a presence session is configurable with the `expirationDuration` parameter.</span></span> <span data-ttu-id="c52ab-119">Quando uma sessão expira, ela se torna `Offline` .</span><span class="sxs-lookup"><span data-stu-id="c52ab-119">When a session expires it becomes `Offline`.</span></span>

## <a name="permissions"></a><span data-ttu-id="c52ab-120">Permissões</span><span class="sxs-lookup"><span data-stu-id="c52ab-120">Permissions</span></span>
<span data-ttu-id="c52ab-121">A permissão a seguir é necessária para chamar a API.</span><span class="sxs-lookup"><span data-stu-id="c52ab-121">The following permission is required to call the API.</span></span> <span data-ttu-id="c52ab-122">Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c52ab-122">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c52ab-123">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c52ab-123">Permission type</span></span>                        | <span data-ttu-id="c52ab-124">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c52ab-124">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="c52ab-125">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c52ab-125">Delegated (work or school account)</span></span>     | <span data-ttu-id="c52ab-126">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c52ab-126">Not Supported.</span></span>                              |
| <span data-ttu-id="c52ab-127">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c52ab-127">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c52ab-128">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c52ab-128">Not Supported.</span></span>                              |
| <span data-ttu-id="c52ab-129">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c52ab-129">Application</span></span>                            | <span data-ttu-id="c52ab-130">Presence.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c52ab-130">Presence.ReadWrite.All</span></span>                      |

## <a name="http-request"></a><span data-ttu-id="c52ab-131">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c52ab-131">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{userId}/presence/setPresence
```
## <a name="request-headers"></a><span data-ttu-id="c52ab-132">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c52ab-132">Request headers</span></span>
| <span data-ttu-id="c52ab-133">Nome</span><span class="sxs-lookup"><span data-stu-id="c52ab-133">Name</span></span>          | <span data-ttu-id="c52ab-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="c52ab-134">Description</span></span>                 |
| :------------ | :-------------------------- |
| <span data-ttu-id="c52ab-135">Autorização</span><span class="sxs-lookup"><span data-stu-id="c52ab-135">Authorization</span></span> | <span data-ttu-id="c52ab-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c52ab-p105">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="c52ab-138">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c52ab-138">Content-Type</span></span>  | <span data-ttu-id="c52ab-p106">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c52ab-p106">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c52ab-141">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c52ab-141">Request body</span></span>

<span data-ttu-id="c52ab-142">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c52ab-142">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="c52ab-143">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="c52ab-143">Parameter</span></span>          | <span data-ttu-id="c52ab-144">Tipo</span><span class="sxs-lookup"><span data-stu-id="c52ab-144">Type</span></span>     | <span data-ttu-id="c52ab-145">Descrição</span><span class="sxs-lookup"><span data-stu-id="c52ab-145">Description</span></span>                                                                                            |
| :----------------- | :------- | :----------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="c52ab-146">sessionId</span><span class="sxs-lookup"><span data-stu-id="c52ab-146">sessionId</span></span>          | <span data-ttu-id="c52ab-147">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c52ab-147">string</span></span>   | <span data-ttu-id="c52ab-148">A ID da sessão de presença do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="c52ab-148">The ID of the application's presence session.</span></span>                                                          |
| <span data-ttu-id="c52ab-149">availability</span><span class="sxs-lookup"><span data-stu-id="c52ab-149">availability</span></span>       | <span data-ttu-id="c52ab-150">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c52ab-150">string</span></span>   | <span data-ttu-id="c52ab-151">As informações de presença base.</span><span class="sxs-lookup"><span data-stu-id="c52ab-151">The base presence information.</span></span>                                                                         |
| <span data-ttu-id="c52ab-152">atividade</span><span class="sxs-lookup"><span data-stu-id="c52ab-152">activity</span></span>           | <span data-ttu-id="c52ab-153">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c52ab-153">string</span></span>   | <span data-ttu-id="c52ab-154">As informações complementares à disponibilidade.</span><span class="sxs-lookup"><span data-stu-id="c52ab-154">The supplemental information to availability.</span></span>                                                          |
| <span data-ttu-id="c52ab-155">expirationDuration</span><span class="sxs-lookup"><span data-stu-id="c52ab-155">expirationDuration</span></span> | <span data-ttu-id="c52ab-156">duração</span><span class="sxs-lookup"><span data-stu-id="c52ab-156">duration</span></span> | <span data-ttu-id="c52ab-157">A expiração da sessão de presença do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="c52ab-157">The expiration of the app presence session.</span></span> <span data-ttu-id="c52ab-158">O valor é representado no formato ISO 8601 por durações.</span><span class="sxs-lookup"><span data-stu-id="c52ab-158">The value is represented in ISO 8601 format for durations.</span></span> |

> [!IMPORTANT]
>
> <span data-ttu-id="c52ab-159">Forneça a ID do aplicativo como `sessionId` na solicitação.</span><span class="sxs-lookup"><span data-stu-id="c52ab-159">Provide the ID of the application as `sessionId` in the request.</span></span>

<span data-ttu-id="c52ab-160">Combinações com suporte de `availability` e `activity` são:</span><span class="sxs-lookup"><span data-stu-id="c52ab-160">Supported combinations of `availability` and `activity` are:</span></span>

| <span data-ttu-id="c52ab-161">availability</span><span class="sxs-lookup"><span data-stu-id="c52ab-161">availability</span></span> | <span data-ttu-id="c52ab-162">atividade</span><span class="sxs-lookup"><span data-stu-id="c52ab-162">activity</span></span>          | <span data-ttu-id="c52ab-163">Descrição</span><span class="sxs-lookup"><span data-stu-id="c52ab-163">Description</span></span>                                              |
| :----------- | :---------------- | :------------------------------------------------------- |
| <span data-ttu-id="c52ab-164">Disponível</span><span class="sxs-lookup"><span data-stu-id="c52ab-164">Available</span></span>    | <span data-ttu-id="c52ab-165">Disponível</span><span class="sxs-lookup"><span data-stu-id="c52ab-165">Available</span></span>         | <span data-ttu-id="c52ab-166">Atualiza a sessão de presença como Disponível.</span><span class="sxs-lookup"><span data-stu-id="c52ab-166">Updates the presence session as Available.</span></span>               |
| <span data-ttu-id="c52ab-167">Ocupado</span><span class="sxs-lookup"><span data-stu-id="c52ab-167">Busy</span></span>         | <span data-ttu-id="c52ab-168">InACall</span><span class="sxs-lookup"><span data-stu-id="c52ab-168">InACall</span></span>           | <span data-ttu-id="c52ab-169">Atualiza a sessão de presença como Ocupado, InACall.</span><span class="sxs-lookup"><span data-stu-id="c52ab-169">Updates the presence session as Busy, InACall.</span></span>           |
| <span data-ttu-id="c52ab-170">Ocupado</span><span class="sxs-lookup"><span data-stu-id="c52ab-170">Busy</span></span>         | <span data-ttu-id="c52ab-171">InAConferenceCall</span><span class="sxs-lookup"><span data-stu-id="c52ab-171">InAConferenceCall</span></span> | <span data-ttu-id="c52ab-172">Atualiza a sessão de presença como Busy, InAConferenceCall.</span><span class="sxs-lookup"><span data-stu-id="c52ab-172">Updates the presence session as Busy, InAConferenceCall.</span></span> |
| <span data-ttu-id="c52ab-173">Away</span><span class="sxs-lookup"><span data-stu-id="c52ab-173">Away</span></span>         | <span data-ttu-id="c52ab-174">Away</span><span class="sxs-lookup"><span data-stu-id="c52ab-174">Away</span></span>              | <span data-ttu-id="c52ab-175">Atualiza a sessão de presença como Distante.</span><span class="sxs-lookup"><span data-stu-id="c52ab-175">Updates the presence session as Away.</span></span>                    |

## <a name="response"></a><span data-ttu-id="c52ab-176">Resposta</span><span class="sxs-lookup"><span data-stu-id="c52ab-176">Response</span></span>
<span data-ttu-id="c52ab-177">Se tiver êxito, este método retornará um código de resposta `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="c52ab-177">If successful, this method returns a `200 OK` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="c52ab-178">Exemplos</span><span class="sxs-lookup"><span data-stu-id="c52ab-178">Examples</span></span>
<span data-ttu-id="c52ab-179">A solicitação a seguir mostra o aplicativo com ID `22553876-f5ab-4529-bffb-cfe50aa89f87` que define sua sessão de presença para o usuário `fa8bf3dc-eca7-46b7-bad1-db199b62afc3` .</span><span class="sxs-lookup"><span data-stu-id="c52ab-179">The following request shows the application with ID `22553876-f5ab-4529-bffb-cfe50aa89f87` that sets its presence session for user `fa8bf3dc-eca7-46b7-bad1-db199b62afc3`.</span></span>

### <a name="request"></a><span data-ttu-id="c52ab-180">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c52ab-180">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="c52ab-181">HTTP</span><span class="sxs-lookup"><span data-stu-id="c52ab-181">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "set-presence"
}-->

```msgraph-interactive
POST https://graph.microsoft.com/beta/users/fa8bf3dc-eca7-46b7-bad1-db199b62afc3/presence/setPresence
Content-Type: application/json

{
  "sessionId": "22553876-f5ab-4529-bffb-cfe50aa89f87",
  "availability": "Available",
  "activity": "Available",
  "expirationDuration": "PT1H"
}
```
# <a name="c"></a>[<span data-ttu-id="c52ab-182">C#</span><span class="sxs-lookup"><span data-stu-id="c52ab-182">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/set-presence-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c52ab-183">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c52ab-183">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/set-presence-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c52ab-184">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c52ab-184">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/set-presence-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c52ab-185">Java</span><span class="sxs-lookup"><span data-stu-id="c52ab-185">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/set-presence-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="c52ab-186">Resposta</span><span class="sxs-lookup"><span data-stu-id="c52ab-186">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
```
