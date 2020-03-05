---
title: 'usuário: invalidateAllRefreshTokens'
description: Invalida todos os tokens de atualização do usuário emitidos para aplicativos (bem como cookies de sessão no navegador de um usuário), redefinindo a propriedade de usuário **refreshTokensValidFromDateTime** para a data e hora atual. Normalmente, essa operação é executada (pelo usuário ou por um administrador) se o usuário tiver um dispositivo perdido ou roubado.  Essa operação impediria o acesso a qualquer um dos dados da organização acessados por meio de aplicativos no dispositivo, sem que o usuário primeiro precise entrar novamente. Na verdade, essa operação forçaria o usuário a entrar novamente para todos os aplicativos dos quais eles tinham sido consentidos anteriormente, independentemente do dispositivo.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 6f6eae0438acecf204b2b3076522548cf4035a43
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42451921"
---
# <a name="user-invalidateallrefreshtokens"></a><span data-ttu-id="b90e4-106">usuário: invalidateAllRefreshTokens</span><span class="sxs-lookup"><span data-stu-id="b90e4-106">user: invalidateAllRefreshTokens</span></span>

<span data-ttu-id="b90e4-107">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="b90e4-107">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b90e4-108">Invalida todos os tokens de atualização do usuário emitidos para aplicativos (bem como cookies de sessão no navegador de um usuário), redefinindo a propriedade de usuário **refreshTokensValidFromDateTime** para a data e hora atual.</span><span class="sxs-lookup"><span data-stu-id="b90e4-108">Invalidates all of the user's refresh tokens issued to applications (as well as session cookies in a user's browser), by resetting the **refreshTokensValidFromDateTime** user property to the current date-time.</span></span> <span data-ttu-id="b90e4-109">Normalmente, essa operação é executada (pelo usuário ou por um administrador) se o usuário tiver um dispositivo perdido ou roubado.</span><span class="sxs-lookup"><span data-stu-id="b90e4-109">Typically, this operation is performed (by the user or an administrator) if the user has a lost or stolen device.</span></span>  <span data-ttu-id="b90e4-110">Essa operação impediria o acesso a qualquer um dos dados da organização acessados por meio de aplicativos no dispositivo, sem que o usuário primeiro precise entrar novamente.</span><span class="sxs-lookup"><span data-stu-id="b90e4-110">This operation would prevent access to any of the organization's data accessed through applications on the device without the user first being required to sign in again.</span></span> <span data-ttu-id="b90e4-111">Na verdade, essa operação forçaria o usuário a entrar novamente para todos os aplicativos dos quais eles tinham sido consentidos anteriormente, independentemente do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b90e4-111">In fact, this operation would force the user to sign in again for all applications that they have previously consented to, independent of device.</span></span>

<span data-ttu-id="b90e4-112">Para desenvolvedores, se o aplicativo tentar resgatar um token de acesso delegado para esse usuário usando um token de atualização invalidado, o aplicativo receberá um erro.</span><span class="sxs-lookup"><span data-stu-id="b90e4-112">For developers, if the application attempts to redeem a delegated access token for this user by using an invalidated refresh token, the application will get an error.</span></span> <span data-ttu-id="b90e4-113">Se isso acontecer, o aplicativo precisará adquirir um novo token de atualização fazendo uma solicitação para o ponto de extremidade de autorização, que forçará o usuário a entrar.</span><span class="sxs-lookup"><span data-stu-id="b90e4-113">If this happens, the application will need to acquire a new refresh token by making a request to the authorize endpoint, which will force the user to sign in.</span></span>

## <a name="permissions"></a><span data-ttu-id="b90e4-114">Permissões</span><span class="sxs-lookup"><span data-stu-id="b90e4-114">Permissions</span></span>
<span data-ttu-id="b90e4-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b90e4-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

+ <span data-ttu-id="b90e4-117">Para um aplicativo permitir que o usuário conectado invalidasse os aplicativos que eles consentiam: user. ReadWrite, Directory. ReadWrite. All, Directory. AccessAsUser. All</span><span class="sxs-lookup"><span data-stu-id="b90e4-117">For an application to allow the signed in user to invalidate applications they've consented to: User.ReadWrite, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>
+ <span data-ttu-id="b90e4-118">Para um aplicativo permitir que um administrador invalidar aplicativos aos quais um usuário tenha sido enviado: Directory. ReadWrite. All, Directory. AccessAsUser. All</span><span class="sxs-lookup"><span data-stu-id="b90e4-118">For an application to allow an administrator to invalidate applications a user has consented to: Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>

## <a name="http-request"></a><span data-ttu-id="b90e4-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b90e4-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/invalidateAllRefreshTokens
POST /users/{id | userPrincipalName}/invalidateAllRefreshTokens
```
## <a name="request-headers"></a><span data-ttu-id="b90e4-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b90e4-120">Request headers</span></span>
| <span data-ttu-id="b90e4-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b90e4-121">Header</span></span>       | <span data-ttu-id="b90e4-122">Valor</span><span class="sxs-lookup"><span data-stu-id="b90e4-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="b90e4-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="b90e4-123">Authorization</span></span>  | <span data-ttu-id="b90e4-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b90e4-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="b90e4-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b90e4-126">Request body</span></span>
<span data-ttu-id="b90e4-127">Esta operação não tem conteúdo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="b90e4-127">This operation has no request content.</span></span>

## <a name="response"></a><span data-ttu-id="b90e4-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="b90e4-128">Response</span></span>

<span data-ttu-id="b90e4-129">Se bem sucedido, este método retorna um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="b90e4-129">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="b90e4-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b90e4-130">Example</span></span>
<span data-ttu-id="b90e4-131">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="b90e4-131">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="b90e4-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b90e4-132">Request</span></span>
<span data-ttu-id="b90e4-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b90e4-133">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b90e4-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="b90e4-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_invalidateallrefreshtokens"
}-->
```http
POST https://graph.microsoft.com/beta/me/invalidateAllRefreshTokens
```
# <a name="c"></a>[<span data-ttu-id="b90e4-135">C#</span><span class="sxs-lookup"><span data-stu-id="b90e4-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-invalidateallrefreshtokens-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b90e4-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b90e4-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-invalidateallrefreshtokens-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b90e4-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b90e4-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-invalidateallrefreshtokens-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="b90e4-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="b90e4-138">Response</span></span>
<span data-ttu-id="b90e4-139">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b90e4-139">Here is an example of the response.</span></span> 
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
