---
title: 'usuário: revokeSignInSessions'
description: Invalida todos os tokens de atualização do usuário emitidos para aplicativos (bem como cookies de sessão no navegador de um usuário), redefinindo a propriedade de usuário **signInSessionsValidFromDateTime** para a data e hora atual.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: b28356112cdca6c3f79599224f89bec8a265d84e
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33637084"
---
# <a name="user-revokesigninsessions"></a><span data-ttu-id="aefb0-103">usuário: revokeSignInSessions</span><span class="sxs-lookup"><span data-stu-id="aefb0-103">user: revokeSignInSessions</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="aefb0-104">Invalida todos os tokens de atualização emitidos para aplicativos para um usuário (bem como cookies de sessão no navegador do usuário), redefinindo a propriedade de usuário **signInSessionsValidFromDateTime** para a data e hora atual.</span><span class="sxs-lookup"><span data-stu-id="aefb0-104">Invalidates all the refresh tokens issued to applications for a user (as well as session cookies in a user's browser), by resetting the **signInSessionsValidFromDateTime** user property to the current date-time.</span></span> <span data-ttu-id="aefb0-105">Normalmente, essa operação é executada (pelo usuário ou por um administrador) se o usuário tiver um dispositivo perdido ou roubado.</span><span class="sxs-lookup"><span data-stu-id="aefb0-105">Typically, this operation is performed (by the user or an administrator) if the user has a lost or stolen device.</span></span> <span data-ttu-id="aefb0-106">Essa operação impede o acesso aos dados da organização por meio de aplicativos no dispositivo solicitando que o usuário entre novamente em todos os aplicativos para os quais tenham sido consentidos anteriormente, independentemente do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="aefb0-106">This operation prevents access to the organization's data through applications on the device by requiring the user to sign in again to all applications that they have previously consented to, independent of device.</span></span>

<span data-ttu-id="aefb0-107">Se o aplicativo tentar resgatar um token de acesso delegado para esse usuário usando um token de atualização invalidado, o aplicativo receberá um erro.</span><span class="sxs-lookup"><span data-stu-id="aefb0-107">If the application attempts to redeem a delegated access token for this user by using an invalidated refresh token, the application will get an error.</span></span> <span data-ttu-id="aefb0-108">Se isso acontecer, o aplicativo precisará adquirir um novo token de atualização fazendo uma solicitação para o ponto de extremidade de autorização, que forçará o usuário a entrar.</span><span class="sxs-lookup"><span data-stu-id="aefb0-108">If this happens, the application will need to acquire a new refresh token by making a request to the authorize endpoint, which will force the user to sign in.</span></span>

## <a name="permissions"></a><span data-ttu-id="aefb0-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="aefb0-109">Permissions</span></span>
<span data-ttu-id="aefb0-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="aefb0-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="aefb0-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="aefb0-112">Permission type</span></span>                        | <span data-ttu-id="aefb0-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="aefb0-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="aefb0-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="aefb0-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="aefb0-115">User. ReadWrite, Directory. ReadWrite. All, Directory. AccessAsUser. All</span><span class="sxs-lookup"><span data-stu-id="aefb0-115">User.ReadWrite, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="aefb0-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="aefb0-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="aefb0-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="aefb0-117">Not supported.</span></span> |
|<span data-ttu-id="aefb0-118">Application</span><span class="sxs-lookup"><span data-stu-id="aefb0-118">Application</span></span>                            | <span data-ttu-id="aefb0-119">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="aefb0-119">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="aefb0-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="aefb0-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/revokeSignInSessions
POST /users/{id | userPrincipalName}/revokeSignInSessions
```
## <a name="request-headers"></a><span data-ttu-id="aefb0-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="aefb0-121">Request headers</span></span>
| <span data-ttu-id="aefb0-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="aefb0-122">Header</span></span>       | <span data-ttu-id="aefb0-123">Valor</span><span class="sxs-lookup"><span data-stu-id="aefb0-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="aefb0-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="aefb0-124">Authorization</span></span>  | <span data-ttu-id="aefb0-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="aefb0-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="aefb0-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="aefb0-127">Request body</span></span>
<span data-ttu-id="aefb0-128">Esta operação não tem conteúdo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="aefb0-128">This operation has no request content.</span></span>

## <a name="response"></a><span data-ttu-id="aefb0-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="aefb0-129">Response</span></span>

<span data-ttu-id="aefb0-130">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="aefb0-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="aefb0-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="aefb0-131">Example</span></span>
<span data-ttu-id="aefb0-132">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="aefb0-132">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="aefb0-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="aefb0-133">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "user_revokesigninsessionss"
}-->
```http
POST https://graph.microsoft.com/beta/me/revokeSignInSessions
```

##### <a name="response"></a><span data-ttu-id="aefb0-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="aefb0-134">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="aefb0-135">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="aefb0-135">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="aefb0-136">Basic</span><span class="sxs-lookup"><span data-stu-id="aefb0-136">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/user_revokesigninsessionss-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="aefb0-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="aefb0-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/user_revokesigninsessionss-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/user-revokesigninsessions.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/user-revokesigninsessions.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
