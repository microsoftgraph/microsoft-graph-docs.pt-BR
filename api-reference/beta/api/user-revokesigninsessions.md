---
title: 'user: revokeSignInSessions'
description: Invalida todos os tokens de atualização do usuário emitidos para aplicativos (bem como cookies de sessão no navegador do usuário), redefinindo a propriedade de usuário **signInSessionsValidFromDateTime** para a data-hora atual.
localization_priority: Normal
author: jpettere
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: 53d194ac1058652c06e673beca1fdd6aeb876719
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50719728"
---
# <a name="user-revokesigninsessions"></a><span data-ttu-id="c1e28-103">user: revokeSignInSessions</span><span class="sxs-lookup"><span data-stu-id="c1e28-103">user: revokeSignInSessions</span></span>

<span data-ttu-id="c1e28-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c1e28-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c1e28-105">Invalida todos os tokens de atualização emitidos para aplicativos para um usuário (bem como cookies de sessão no navegador de um usuário), redefinindo a propriedade de usuário **signInSessionsValidFromDateTime** para a data-hora atual.</span><span class="sxs-lookup"><span data-stu-id="c1e28-105">Invalidates all the refresh tokens issued to applications for a user (as well as session cookies in a user's browser), by resetting the **signInSessionsValidFromDateTime** user property to the current date-time.</span></span> <span data-ttu-id="c1e28-106">Normalmente, essa operação é executada (pelo usuário ou por um administrador) se o usuário tiver um dispositivo perdido ou roubado.</span><span class="sxs-lookup"><span data-stu-id="c1e28-106">Typically, this operation is performed (by the user or an administrator) if the user has a lost or stolen device.</span></span> <span data-ttu-id="c1e28-107">Essa operação impede o acesso aos dados da organização por meio de aplicativos no dispositivo, exigindo que o usuário entre novamente em todos os aplicativos que eles consentiram anteriormente, independentemente do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="c1e28-107">This operation prevents access to the organization's data through applications on the device by requiring the user to sign in again to all applications that they have previously consented to, independent of device.</span></span>

<span data-ttu-id="c1e28-108">Se o aplicativo tentar resgatar um token de acesso delegado para esse usuário usando um token de atualização inválido, o aplicativo receberá um erro.</span><span class="sxs-lookup"><span data-stu-id="c1e28-108">If the application attempts to redeem a delegated access token for this user by using an invalidated refresh token, the application will get an error.</span></span> <span data-ttu-id="c1e28-109">Se isso acontecer, o aplicativo precisará adquirir um novo token de atualização fazendo uma solicitação ao ponto de extremidade de autorização, o que forçará o usuário a entrar.</span><span class="sxs-lookup"><span data-stu-id="c1e28-109">If this happens, the application will need to acquire a new refresh token by making a request to the authorize endpoint, which will force the user to sign in.</span></span>

>[!NOTE]
><span data-ttu-id="c1e28-110">Depois de **chamar revokeSignInSessions**, pode haver um pequeno atraso de alguns minutos antes que os tokens sejam revogados.</span><span class="sxs-lookup"><span data-stu-id="c1e28-110">After calling **revokeSignInSessions**, there might be a small delay of a few minutes before tokens are revoked.</span></span>

## <a name="permissions"></a><span data-ttu-id="c1e28-111">Permissões</span><span class="sxs-lookup"><span data-stu-id="c1e28-111">Permissions</span></span>

<span data-ttu-id="c1e28-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c1e28-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c1e28-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c1e28-114">Permission type</span></span>                        | <span data-ttu-id="c1e28-115">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c1e28-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="c1e28-116">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c1e28-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="c1e28-117">User.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="c1e28-117">User.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="c1e28-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c1e28-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c1e28-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c1e28-119">Not supported.</span></span> |
|<span data-ttu-id="c1e28-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c1e28-120">Application</span></span>                            | <span data-ttu-id="c1e28-121">User.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c1e28-121">User.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c1e28-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c1e28-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/revokeSignInSessions
POST /users/{id | userPrincipalName}/revokeSignInSessions
```

## <a name="request-headers"></a><span data-ttu-id="c1e28-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c1e28-123">Request headers</span></span>
| <span data-ttu-id="c1e28-124">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c1e28-124">Header</span></span>       | <span data-ttu-id="c1e28-125">Valor</span><span class="sxs-lookup"><span data-stu-id="c1e28-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="c1e28-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="c1e28-126">Authorization</span></span>  | <span data-ttu-id="c1e28-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c1e28-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="c1e28-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c1e28-129">Content-Type</span></span>  | <span data-ttu-id="c1e28-130">application/json</span><span class="sxs-lookup"><span data-stu-id="c1e28-130">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c1e28-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c1e28-131">Request body</span></span>
<span data-ttu-id="c1e28-132">Esta operação não tem conteúdo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="c1e28-132">This operation has no request content.</span></span>

## <a name="response"></a><span data-ttu-id="c1e28-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="c1e28-133">Response</span></span>

<span data-ttu-id="c1e28-134">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="c1e28-134">If successful, this method returns a `204 No Content` response code.</span></span>

>[!NOTE]
><span data-ttu-id="c1e28-135">Essa API tem um [problema conhecido](/graph/known-issues#revoke-sign-in-sessions-returns-wrong-HTTP-code).</span><span class="sxs-lookup"><span data-stu-id="c1e28-135">This API has a [known issue](/graph/known-issues#revoke-sign-in-sessions-returns-wrong-HTTP-code).</span></span> <span data-ttu-id="c1e28-136">Ele retorna um código de resposta HTTP diferente.</span><span class="sxs-lookup"><span data-stu-id="c1e28-136">It returns a different HTTP response code.</span></span>

## <a name="example"></a><span data-ttu-id="c1e28-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c1e28-137">Example</span></span>
<span data-ttu-id="c1e28-138">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="c1e28-138">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="c1e28-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c1e28-139">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="c1e28-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="c1e28-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_revokesigninsessionss"
}-->
```http
POST https://graph.microsoft.com/beta/me/revokeSignInSessions
```
# <a name="c"></a>[<span data-ttu-id="c1e28-141">C#</span><span class="sxs-lookup"><span data-stu-id="c1e28-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-revokesigninsessionss-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c1e28-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c1e28-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-revokesigninsessionss-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c1e28-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c1e28-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-revokesigninsessionss-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c1e28-144">Java</span><span class="sxs-lookup"><span data-stu-id="c1e28-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-revokesigninsessionss-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="c1e28-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="c1e28-145">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "user: revokeSignInSessions",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


