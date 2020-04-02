---
title: 'usuário: revokeSignInSessions'
description: Invalida todos os tokens de atualização do usuário emitidos para aplicativos (bem como cookies de sessão no navegador de um usuário), redefinindo a propriedade de usuário **signInSessionsValidFromDateTime** para a data e hora atual.
localization_priority: Normal
author: krbain
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: cd85304459f0d3208b62f2976aa1a53bda8cb2b9
ms.sourcegitcommit: d6386c5d4bb8917132c3f6c4de945487939b7fb7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/02/2020
ms.locfileid: "43107343"
---
# <a name="user-revokesigninsessions"></a><span data-ttu-id="f9ffa-103">usuário: revokeSignInSessions</span><span class="sxs-lookup"><span data-stu-id="f9ffa-103">user: revokeSignInSessions</span></span>

<span data-ttu-id="f9ffa-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f9ffa-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f9ffa-105">Invalida todos os tokens de atualização emitidos para aplicativos para um usuário (bem como cookies de sessão no navegador do usuário), redefinindo a propriedade de usuário **signInSessionsValidFromDateTime** para a data e hora atual.</span><span class="sxs-lookup"><span data-stu-id="f9ffa-105">Invalidates all the refresh tokens issued to applications for a user (as well as session cookies in a user's browser), by resetting the **signInSessionsValidFromDateTime** user property to the current date-time.</span></span> <span data-ttu-id="f9ffa-106">Normalmente, essa operação é executada (pelo usuário ou por um administrador) se o usuário tiver um dispositivo perdido ou roubado.</span><span class="sxs-lookup"><span data-stu-id="f9ffa-106">Typically, this operation is performed (by the user or an administrator) if the user has a lost or stolen device.</span></span> <span data-ttu-id="f9ffa-107">Essa operação impede o acesso aos dados da organização por meio de aplicativos no dispositivo solicitando que o usuário entre novamente em todos os aplicativos para os quais tenham sido consentidos anteriormente, independentemente do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f9ffa-107">This operation prevents access to the organization's data through applications on the device by requiring the user to sign in again to all applications that they have previously consented to, independent of device.</span></span>

<span data-ttu-id="f9ffa-108">Se o aplicativo tentar resgatar um token de acesso delegado para esse usuário usando um token de atualização invalidado, o aplicativo receberá um erro.</span><span class="sxs-lookup"><span data-stu-id="f9ffa-108">If the application attempts to redeem a delegated access token for this user by using an invalidated refresh token, the application will get an error.</span></span> <span data-ttu-id="f9ffa-109">Se isso acontecer, o aplicativo precisará adquirir um novo token de atualização fazendo uma solicitação para o ponto de extremidade de autorização, que forçará o usuário a entrar.</span><span class="sxs-lookup"><span data-stu-id="f9ffa-109">If this happens, the application will need to acquire a new refresh token by making a request to the authorize endpoint, which will force the user to sign in.</span></span>

>[!NOTE]
><span data-ttu-id="f9ffa-110">Após chamar o **revokeSignInSessions**, pode haver um pequeno atraso de alguns minutos antes de os tokens serem revogados.</span><span class="sxs-lookup"><span data-stu-id="f9ffa-110">After calling **revokeSignInSessions**, there might be a small delay of a few minutes before tokens are revoked.</span></span>

## <a name="permissions"></a><span data-ttu-id="f9ffa-111">Permissões</span><span class="sxs-lookup"><span data-stu-id="f9ffa-111">Permissions</span></span>

<span data-ttu-id="f9ffa-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f9ffa-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f9ffa-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f9ffa-114">Permission type</span></span>                        | <span data-ttu-id="f9ffa-115">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f9ffa-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="f9ffa-116">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f9ffa-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="f9ffa-117">User. ReadWrite, Directory. ReadWrite. All, Directory. AccessAsUser. All</span><span class="sxs-lookup"><span data-stu-id="f9ffa-117">User.ReadWrite, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="f9ffa-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f9ffa-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f9ffa-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f9ffa-119">Not supported.</span></span> |
|<span data-ttu-id="f9ffa-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f9ffa-120">Application</span></span>                            | <span data-ttu-id="f9ffa-121">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="f9ffa-121">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f9ffa-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f9ffa-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/revokeSignInSessions
POST /users/{id | userPrincipalName}/revokeSignInSessions
```

## <a name="request-headers"></a><span data-ttu-id="f9ffa-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f9ffa-123">Request headers</span></span>
| <span data-ttu-id="f9ffa-124">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f9ffa-124">Header</span></span>       | <span data-ttu-id="f9ffa-125">Valor</span><span class="sxs-lookup"><span data-stu-id="f9ffa-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="f9ffa-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="f9ffa-126">Authorization</span></span>  | <span data-ttu-id="f9ffa-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f9ffa-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="f9ffa-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f9ffa-129">Content-Type</span></span>  | <span data-ttu-id="f9ffa-130">application/json</span><span class="sxs-lookup"><span data-stu-id="f9ffa-130">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="f9ffa-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f9ffa-131">Request body</span></span>
<span data-ttu-id="f9ffa-132">Esta operação não tem conteúdo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="f9ffa-132">This operation has no request content.</span></span>

## <a name="response"></a><span data-ttu-id="f9ffa-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="f9ffa-133">Response</span></span>

<span data-ttu-id="f9ffa-134">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="f9ffa-134">If successful, this method returns a `204 No Content` response code.</span></span>

>[!NOTE]
><span data-ttu-id="f9ffa-135">Essa API tem um [problema conhecido](/graph/known-issues#revoke-sign-in-sessions-returns-wrong-HTTP-code).</span><span class="sxs-lookup"><span data-stu-id="f9ffa-135">This API has a [known issue](/graph/known-issues#revoke-sign-in-sessions-returns-wrong-HTTP-code).</span></span> <span data-ttu-id="f9ffa-136">Ele retorna um código de resposta HTTP diferente.</span><span class="sxs-lookup"><span data-stu-id="f9ffa-136">It returns a different HTTP response code.</span></span>

## <a name="example"></a><span data-ttu-id="f9ffa-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f9ffa-137">Example</span></span>
<span data-ttu-id="f9ffa-138">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="f9ffa-138">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="f9ffa-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f9ffa-139">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="f9ffa-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="f9ffa-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_revokesigninsessionss"
}-->
```http
POST https://graph.microsoft.com/beta/me/revokeSignInSessions
```
# <a name="c"></a>[<span data-ttu-id="f9ffa-141">C#</span><span class="sxs-lookup"><span data-stu-id="f9ffa-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-revokesigninsessionss-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f9ffa-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f9ffa-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-revokesigninsessionss-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f9ffa-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f9ffa-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-revokesigninsessionss-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="f9ffa-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="f9ffa-144">Response</span></span>
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
