---
title: 'user: invalidateAllRefreshTokens'
description: Invalida todos os tokens de atualização do usuário emitidos para aplicativos e cookies de sessão no navegador do usuário.
localization_priority: Normal
author: jpettere
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: a13982cb924c5c9b82c3248aefc13a54ec44bb2e
ms.sourcegitcommit: 4888ac7504533344c4fc6828e2a06a002a1d72d3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/09/2021
ms.locfileid: "53351045"
---
# <a name="user-invalidateallrefreshtokens"></a><span data-ttu-id="35bcd-103">user: invalidateAllRefreshTokens</span><span class="sxs-lookup"><span data-stu-id="35bcd-103">user: invalidateAllRefreshTokens</span></span>

<span data-ttu-id="35bcd-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="35bcd-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="35bcd-105">Invalida todos os tokens de atualização do usuário emitidos para aplicativos (bem como cookies de sessão no navegador de um usuário), redefinindo a propriedade de usuário **refreshTokensValidFromDateTime** para a data-hora atual.</span><span class="sxs-lookup"><span data-stu-id="35bcd-105">Invalidates all of the user's refresh tokens issued to applications (as well as session cookies in a user's browser), by resetting the **refreshTokensValidFromDateTime** user property to the current date-time.</span></span> <span data-ttu-id="35bcd-106">Normalmente, essa operação é executada (pelo usuário ou por um administrador) se o usuário tiver um dispositivo perdido ou roubado.</span><span class="sxs-lookup"><span data-stu-id="35bcd-106">Typically, this operation is performed (by the user or an administrator) if the user has a lost or stolen device.</span></span>  <span data-ttu-id="35bcd-107">Essa operação impediria o acesso a qualquer um dos dados da organização acessados por meio de aplicativos no dispositivo sem que o usuário seja obrigado a entrar novamente.</span><span class="sxs-lookup"><span data-stu-id="35bcd-107">This operation would prevent access to any of the organization's data accessed through applications on the device without the user first being required to sign in again.</span></span> <span data-ttu-id="35bcd-108">Na verdade, essa operação forçaria o usuário a entrar novamente em todos os aplicativos que eles consentiram anteriormente, independentemente do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="35bcd-108">In fact, this operation would force the user to sign in again for all applications that they have previously consented to, independent of device.</span></span>

<span data-ttu-id="35bcd-109">Para desenvolvedores, se o aplicativo tentar resgatar um token de acesso delegado para esse usuário usando um token de atualização inválido, o aplicativo receberá um erro.</span><span class="sxs-lookup"><span data-stu-id="35bcd-109">For developers, if the application attempts to redeem a delegated access token for this user by using an invalidated refresh token, the application will get an error.</span></span> <span data-ttu-id="35bcd-110">Se isso acontecer, o aplicativo precisará adquirir um novo token de atualização fazendo uma solicitação ao ponto de extremidade de autorização, o que forçará o usuário a entrar.</span><span class="sxs-lookup"><span data-stu-id="35bcd-110">If this happens, the application will need to acquire a new refresh token by making a request to the authorize endpoint, which will force the user to sign in.</span></span>

## <a name="permissions"></a><span data-ttu-id="35bcd-111">Permissões</span><span class="sxs-lookup"><span data-stu-id="35bcd-111">Permissions</span></span>
<span data-ttu-id="35bcd-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="35bcd-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

+ <span data-ttu-id="35bcd-114">Para que um aplicativo permita que o usuário inscreve invalide os aplicativos aos qual ele consentiu: User.ReadWrite, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="35bcd-114">For an application to allow the signed in user to invalidate applications they've consented to: User.ReadWrite, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>
+ <span data-ttu-id="35bcd-115">Para um aplicativo permitir que um administrador invalide aplicativos que um usuário consentiu: Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="35bcd-115">For an application to allow an administrator to invalidate applications a user has consented to: Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>

## <a name="http-request"></a><span data-ttu-id="35bcd-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="35bcd-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/invalidateAllRefreshTokens
POST /users/{id | userPrincipalName}/invalidateAllRefreshTokens
```
## <a name="request-headers"></a><span data-ttu-id="35bcd-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="35bcd-117">Request headers</span></span>
| <span data-ttu-id="35bcd-118">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="35bcd-118">Header</span></span>       | <span data-ttu-id="35bcd-119">Valor</span><span class="sxs-lookup"><span data-stu-id="35bcd-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="35bcd-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="35bcd-120">Authorization</span></span>  | <span data-ttu-id="35bcd-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="35bcd-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="35bcd-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="35bcd-123">Request body</span></span>
<span data-ttu-id="35bcd-124">Esta operação não tem conteúdo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="35bcd-124">This operation has no request content.</span></span>

## <a name="response"></a><span data-ttu-id="35bcd-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="35bcd-125">Response</span></span>

<span data-ttu-id="35bcd-126">Se bem sucedido, este método retorna um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="35bcd-126">If successful, this method returns `204 No Content` response code.</span></span>

>[!NOTE]
><span data-ttu-id="35bcd-127">Essa API retorna um código de resposta HTTP diferente, semelhante à ação [revokeSignInSessions.](user-revokesigninsessions.md)</span><span class="sxs-lookup"><span data-stu-id="35bcd-127">This API returns a different HTTP response code, similar to the [revokeSignInSessions](user-revokesigninsessions.md) action.</span></span> <span data-ttu-id="35bcd-128">Para obter detalhes, consulte [problema conhecido](/graph/known-issues#revoke-sign-in-sessions-returns-wrong-HTTP-code).</span><span class="sxs-lookup"><span data-stu-id="35bcd-128">For details, see [known issue](/graph/known-issues#revoke-sign-in-sessions-returns-wrong-HTTP-code).</span></span> 

## <a name="example"></a><span data-ttu-id="35bcd-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="35bcd-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="35bcd-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="35bcd-130">Request</span></span>
<span data-ttu-id="35bcd-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="35bcd-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="35bcd-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="35bcd-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_invalidateallrefreshtokens"
}-->
```http
POST https://graph.microsoft.com/beta/me/invalidateAllRefreshTokens
```
# <a name="c"></a>[<span data-ttu-id="35bcd-133">C#</span><span class="sxs-lookup"><span data-stu-id="35bcd-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-invalidateallrefreshtokens-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="35bcd-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="35bcd-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-invalidateallrefreshtokens-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="35bcd-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="35bcd-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-invalidateallrefreshtokens-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="35bcd-136">Java</span><span class="sxs-lookup"><span data-stu-id="35bcd-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-invalidateallrefreshtokens-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="35bcd-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="35bcd-137">Response</span></span>
<span data-ttu-id="35bcd-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="35bcd-138">The following is an example of the response.</span></span> 
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
  "description": "user: invalidateAllRefreshTokens",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


