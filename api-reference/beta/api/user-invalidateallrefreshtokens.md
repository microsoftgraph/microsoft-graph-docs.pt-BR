---
title: 'usuário: invalidateAllRefreshTokens'
description: Invalida todos os tokens de atualização do usuário emitidos para aplicativos (bem como cookies de sessão no navegador de um usuário), redefinindo a propriedade de usuário **refreshTokensValidFromDateTime** para a data e hora atual. Normalmente, essa operação é executada (pelo usuário ou por um administrador) se o usuário tiver um dispositivo perdido ou roubado.  Essa operação impediria o acesso a qualquer um dos dados da organização acessados por meio de aplicativos no dispositivo, sem que o usuário primeiro precise entrar novamente. Na verdade, essa operação forçaria o usuário a entrar novamente para todos os aplicativos dos quais eles tinham sido consentidos anteriormente, independentemente do dispositivo.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: e4efc33f3c0cb0f0ec4f4ef4026598d6d2f8a581
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/15/2019
ms.locfileid: "36421082"
---
# <a name="user-invalidateallrefreshtokens"></a><span data-ttu-id="79d8b-106">usuário: invalidateAllRefreshTokens</span><span class="sxs-lookup"><span data-stu-id="79d8b-106">user: invalidateAllRefreshTokens</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="79d8b-107">Invalida todos os tokens de atualização do usuário emitidos para aplicativos (bem como cookies de sessão no navegador de um usuário), redefinindo a propriedade de usuário **refreshTokensValidFromDateTime** para a data e hora atual.</span><span class="sxs-lookup"><span data-stu-id="79d8b-107">Invalidates all of the user's refresh tokens issued to applications (as well as session cookies in a user's browser), by resetting the **refreshTokensValidFromDateTime** user property to the current date-time.</span></span> <span data-ttu-id="79d8b-108">Normalmente, essa operação é executada (pelo usuário ou por um administrador) se o usuário tiver um dispositivo perdido ou roubado.</span><span class="sxs-lookup"><span data-stu-id="79d8b-108">Typically, this operation is performed (by the user or an administrator) if the user has a lost or stolen device.</span></span>  <span data-ttu-id="79d8b-109">Essa operação impediria o acesso a qualquer um dos dados da organização acessados por meio de aplicativos no dispositivo, sem que o usuário primeiro precise entrar novamente.</span><span class="sxs-lookup"><span data-stu-id="79d8b-109">This operation would prevent access to any of the organization's data accessed through applications on the device without the user first being required to sign in again.</span></span> <span data-ttu-id="79d8b-110">Na verdade, essa operação forçaria o usuário a entrar novamente para todos os aplicativos dos quais eles tinham sido consentidos anteriormente, independentemente do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="79d8b-110">In fact, this operation would force the user to sign in again for all applications that they have previously consented to, independent of device.</span></span>

<span data-ttu-id="79d8b-111">Para desenvolvedores, se o aplicativo tentar resgatar um token de acesso delegado para esse usuário usando um token de atualização invalidado, o aplicativo receberá um erro.</span><span class="sxs-lookup"><span data-stu-id="79d8b-111">For developers, if the application attempts to redeem a delegated access token for this user by using an invalidated refresh token, the application will get an error.</span></span> <span data-ttu-id="79d8b-112">Se isso acontecer, o aplicativo precisará adquirir um novo token de atualização fazendo uma solicitação para o ponto de extremidade de autorização, que forçará o usuário a entrar.</span><span class="sxs-lookup"><span data-stu-id="79d8b-112">If this happens, the application will need to acquire a new refresh token by making a request to the authorize endpoint, which will force the user to sign in.</span></span>

## <a name="permissions"></a><span data-ttu-id="79d8b-113">Permissões</span><span class="sxs-lookup"><span data-stu-id="79d8b-113">Permissions</span></span>
<span data-ttu-id="79d8b-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="79d8b-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

+ <span data-ttu-id="79d8b-116">Para um aplicativo permitir que o usuário conectado invalidasse os aplicativos que eles consentiam: user. ReadWrite, Directory. ReadWrite. All, Directory. AccessAsUser. All</span><span class="sxs-lookup"><span data-stu-id="79d8b-116">For an application to allow the signed in user to invalidate applications they've consented to: User.ReadWrite, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>
+ <span data-ttu-id="79d8b-117">Para um aplicativo permitir que um administrador invalidar aplicativos aos quais um usuário tenha sido enviado: Directory. ReadWrite. All, Directory. AccessAsUser. All</span><span class="sxs-lookup"><span data-stu-id="79d8b-117">For an application to allow an administrator to invalidate applications a user has consented to: Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>

## <a name="http-request"></a><span data-ttu-id="79d8b-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="79d8b-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/invalidateAllRefreshTokens
POST /users/{id | userPrincipalName}/invalidateAllRefreshTokens
```
## <a name="request-headers"></a><span data-ttu-id="79d8b-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="79d8b-119">Request headers</span></span>
| <span data-ttu-id="79d8b-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="79d8b-120">Header</span></span>       | <span data-ttu-id="79d8b-121">Valor</span><span class="sxs-lookup"><span data-stu-id="79d8b-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="79d8b-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="79d8b-122">Authorization</span></span>  | <span data-ttu-id="79d8b-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="79d8b-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="79d8b-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="79d8b-125">Request body</span></span>
<span data-ttu-id="79d8b-126">Esta operação não tem conteúdo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="79d8b-126">This operation has no request content.</span></span>

## <a name="response"></a><span data-ttu-id="79d8b-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="79d8b-127">Response</span></span>

<span data-ttu-id="79d8b-128">Se bem sucedido, este método retorna um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="79d8b-128">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="79d8b-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="79d8b-129">Example</span></span>
<span data-ttu-id="79d8b-130">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="79d8b-130">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="79d8b-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="79d8b-131">Request</span></span>
<span data-ttu-id="79d8b-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="79d8b-132">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="79d8b-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="79d8b-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_invalidateallrefreshtokens"
}-->
```http
POST https://graph.microsoft.com/beta/me/invalidateAllRefreshTokens
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="79d8b-134">C#</span><span class="sxs-lookup"><span data-stu-id="79d8b-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-invalidateallrefreshtokens-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="79d8b-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="79d8b-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-invalidateallrefreshtokens-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="79d8b-136">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="79d8b-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-invalidateallrefreshtokens-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="79d8b-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="79d8b-137">Response</span></span>
<span data-ttu-id="79d8b-138">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="79d8b-138">Here is an example of the response.</span></span> 
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
