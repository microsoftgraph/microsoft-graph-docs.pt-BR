---
title: 'usuário: invalidateAllRefreshTokens'
description: Invalida todos os tokens de atualização do usuário emitidos para aplicativos e cookies de sessão no navegador do usuário.
localization_priority: Normal
author: krbain
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: 8eccbef22631657a570062d1f0c1107fba63a70b
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48017077"
---
# <a name="user-invalidateallrefreshtokens"></a><span data-ttu-id="bcc14-103">usuário: invalidateAllRefreshTokens</span><span class="sxs-lookup"><span data-stu-id="bcc14-103">user: invalidateAllRefreshTokens</span></span>

<span data-ttu-id="bcc14-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bcc14-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bcc14-105">Invalida todos os tokens de atualização do usuário emitidos para aplicativos (bem como cookies de sessão no navegador de um usuário), redefinindo a propriedade de usuário **refreshTokensValidFromDateTime** para a data e hora atual.</span><span class="sxs-lookup"><span data-stu-id="bcc14-105">Invalidates all of the user's refresh tokens issued to applications (as well as session cookies in a user's browser), by resetting the **refreshTokensValidFromDateTime** user property to the current date-time.</span></span> <span data-ttu-id="bcc14-106">Normalmente, essa operação é executada (pelo usuário ou por um administrador) se o usuário tiver um dispositivo perdido ou roubado.</span><span class="sxs-lookup"><span data-stu-id="bcc14-106">Typically, this operation is performed (by the user or an administrator) if the user has a lost or stolen device.</span></span>  <span data-ttu-id="bcc14-107">Essa operação impediria o acesso a qualquer um dos dados da organização acessados por meio de aplicativos no dispositivo, sem que o usuário primeiro precise entrar novamente.</span><span class="sxs-lookup"><span data-stu-id="bcc14-107">This operation would prevent access to any of the organization's data accessed through applications on the device without the user first being required to sign in again.</span></span> <span data-ttu-id="bcc14-108">Na verdade, essa operação forçaria o usuário a entrar novamente para todos os aplicativos dos quais eles tinham sido consentidos anteriormente, independentemente do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="bcc14-108">In fact, this operation would force the user to sign in again for all applications that they have previously consented to, independent of device.</span></span>

<span data-ttu-id="bcc14-109">Para desenvolvedores, se o aplicativo tentar resgatar um token de acesso delegado para esse usuário usando um token de atualização invalidado, o aplicativo receberá um erro.</span><span class="sxs-lookup"><span data-stu-id="bcc14-109">For developers, if the application attempts to redeem a delegated access token for this user by using an invalidated refresh token, the application will get an error.</span></span> <span data-ttu-id="bcc14-110">Se isso acontecer, o aplicativo precisará adquirir um novo token de atualização fazendo uma solicitação para o ponto de extremidade de autorização, que forçará o usuário a entrar.</span><span class="sxs-lookup"><span data-stu-id="bcc14-110">If this happens, the application will need to acquire a new refresh token by making a request to the authorize endpoint, which will force the user to sign in.</span></span>

## <a name="permissions"></a><span data-ttu-id="bcc14-111">Permissões</span><span class="sxs-lookup"><span data-stu-id="bcc14-111">Permissions</span></span>
<span data-ttu-id="bcc14-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bcc14-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

+ <span data-ttu-id="bcc14-114">Para um aplicativo permitir que o usuário conectado invalidasse os aplicativos que eles consentiam: user. ReadWrite, Directory. ReadWrite. All, Directory. AccessAsUser. All</span><span class="sxs-lookup"><span data-stu-id="bcc14-114">For an application to allow the signed in user to invalidate applications they've consented to: User.ReadWrite, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>
+ <span data-ttu-id="bcc14-115">Para um aplicativo permitir que um administrador invalidar aplicativos aos quais um usuário tenha sido enviado: Directory. ReadWrite. All, Directory. AccessAsUser. All</span><span class="sxs-lookup"><span data-stu-id="bcc14-115">For an application to allow an administrator to invalidate applications a user has consented to: Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>

## <a name="http-request"></a><span data-ttu-id="bcc14-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bcc14-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/invalidateAllRefreshTokens
POST /users/{id | userPrincipalName}/invalidateAllRefreshTokens
```
## <a name="request-headers"></a><span data-ttu-id="bcc14-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bcc14-117">Request headers</span></span>
| <span data-ttu-id="bcc14-118">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="bcc14-118">Header</span></span>       | <span data-ttu-id="bcc14-119">Valor</span><span class="sxs-lookup"><span data-stu-id="bcc14-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="bcc14-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="bcc14-120">Authorization</span></span>  | <span data-ttu-id="bcc14-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bcc14-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="bcc14-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bcc14-123">Request body</span></span>
<span data-ttu-id="bcc14-124">Esta operação não tem conteúdo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="bcc14-124">This operation has no request content.</span></span>

## <a name="response"></a><span data-ttu-id="bcc14-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="bcc14-125">Response</span></span>

<span data-ttu-id="bcc14-126">Se bem sucedido, este método retorna um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="bcc14-126">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="bcc14-127">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bcc14-127">Example</span></span>
<span data-ttu-id="bcc14-128">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="bcc14-128">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="bcc14-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bcc14-129">Request</span></span>
<span data-ttu-id="bcc14-130">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="bcc14-130">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="bcc14-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="bcc14-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_invalidateallrefreshtokens"
}-->
```http
POST https://graph.microsoft.com/beta/me/invalidateAllRefreshTokens
```
# <a name="c"></a>[<span data-ttu-id="bcc14-132">C#</span><span class="sxs-lookup"><span data-stu-id="bcc14-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-invalidateallrefreshtokens-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="bcc14-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bcc14-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-invalidateallrefreshtokens-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="bcc14-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bcc14-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-invalidateallrefreshtokens-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="bcc14-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="bcc14-135">Response</span></span>
<span data-ttu-id="bcc14-136">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bcc14-136">Here is an example of the response.</span></span> 
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


