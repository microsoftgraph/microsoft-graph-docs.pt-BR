---
title: 'usuário: revokeSignInSessions'
description: Invalida todos os tokens de atualização do usuário emitidos para aplicativos (bem como cookies de sessão no navegador de um usuário), redefinindo a propriedade de usuário **signInSessionsValidFromDateTime** para a data e hora atual.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: a39c7af37cd5ab94a33a06a7dd4c91c0c4b55600
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35449005"
---
# <a name="user-revokesigninsessions"></a><span data-ttu-id="3cd0b-103">usuário: revokeSignInSessions</span><span class="sxs-lookup"><span data-stu-id="3cd0b-103">user: revokeSignInSessions</span></span>

<span data-ttu-id="3cd0b-104">Invalida todos os tokens de atualização emitidos para aplicativos para um usuário (bem como cookies de sessão no navegador do usuário), redefinindo a propriedade de usuário **signInSessionsValidFromDateTime** para a data e hora atual.</span><span class="sxs-lookup"><span data-stu-id="3cd0b-104">Invalidates all the refresh tokens issued to applications for a user (as well as session cookies in a user's browser), by resetting the **signInSessionsValidFromDateTime** user property to the current date-time.</span></span> <span data-ttu-id="3cd0b-105">Normalmente, essa operação é executada (pelo usuário ou por um administrador) se o usuário tiver um dispositivo perdido ou roubado.</span><span class="sxs-lookup"><span data-stu-id="3cd0b-105">Typically, this operation is performed (by the user or an administrator) if the user has a lost or stolen device.</span></span> <span data-ttu-id="3cd0b-106">Essa operação impede o acesso aos dados da organização por meio de aplicativos no dispositivo solicitando que o usuário entre novamente em todos os aplicativos para os quais tenham sido consentidos anteriormente, independentemente do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="3cd0b-106">This operation prevents access to the organization's data through applications on the device by requiring the user to sign in again to all applications that they have previously consented to, independent of device.</span></span>

><span data-ttu-id="3cd0b-107">Se o aplicativo tentar resgatar um token de acesso delegado para esse usuário usando um token de atualização invalidado, o aplicativo receberá um erro.</span><span class="sxs-lookup"><span data-stu-id="3cd0b-107">If the application attempts to redeem a delegated access token for this user by using an invalidated refresh token, the application will get an error.</span></span> <span data-ttu-id="3cd0b-108">Se isso acontecer, o aplicativo precisará adquirir um novo token de atualização fazendo uma solicitação para o ponto de extremidade de autorização, que forçará o usuário a entrar.</span><span class="sxs-lookup"><span data-stu-id="3cd0b-108">If this happens, the application will need to acquire a new refresh token by making a request to the authorize endpoint, which will force the user to sign in.</span></span>

>[!NOTE]
><span data-ttu-id="3cd0b-109">Após chamar o **revokeSignInSessions**, pode haver um pequeno atraso de alguns minutos antes de os tokens serem revogados.</span><span class="sxs-lookup"><span data-stu-id="3cd0b-109">After calling **revokeSignInSessions**, there might be a small delay of a few minutes before tokens are revoked.</span></span>

## <a name="permissions"></a><span data-ttu-id="3cd0b-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="3cd0b-110">Permissions</span></span>

<span data-ttu-id="3cd0b-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3cd0b-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3cd0b-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3cd0b-113">Permission type</span></span>                        | <span data-ttu-id="3cd0b-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3cd0b-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="3cd0b-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3cd0b-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="3cd0b-116">User. ReadWrite, Directory. ReadWrite. All, Directory. AccessAsUser. All</span><span class="sxs-lookup"><span data-stu-id="3cd0b-116">User.ReadWrite, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="3cd0b-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3cd0b-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3cd0b-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3cd0b-118">Not supported.</span></span> |
|<span data-ttu-id="3cd0b-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3cd0b-119">Application</span></span>                            | <span data-ttu-id="3cd0b-120">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="3cd0b-120">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3cd0b-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3cd0b-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/revokeSignInSessions
POST /users/{id | userPrincipalName}/revokeSignInSessions
```

## <a name="request-headers"></a><span data-ttu-id="3cd0b-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3cd0b-122">Request headers</span></span>
| <span data-ttu-id="3cd0b-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3cd0b-123">Header</span></span>       | <span data-ttu-id="3cd0b-124">Valor</span><span class="sxs-lookup"><span data-stu-id="3cd0b-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="3cd0b-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="3cd0b-125">Authorization</span></span>  | <span data-ttu-id="3cd0b-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3cd0b-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="3cd0b-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3cd0b-128">Request body</span></span>
<span data-ttu-id="3cd0b-129">Esta operação não tem conteúdo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="3cd0b-129">This operation has no request content.</span></span>

## <a name="response"></a><span data-ttu-id="3cd0b-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="3cd0b-130">Response</span></span>

<span data-ttu-id="3cd0b-131">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="3cd0b-131">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="3cd0b-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3cd0b-132">Example</span></span>
<span data-ttu-id="3cd0b-133">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="3cd0b-133">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="3cd0b-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3cd0b-134">Request</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="3cd0b-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="3cd0b-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_revokesigninsessionss"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/revokeSignInSessions
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="3cd0b-136">C#</span><span class="sxs-lookup"><span data-stu-id="3cd0b-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-revokesigninsessionss-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3cd0b-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="3cd0b-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-revokesigninsessionss-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="3cd0b-138">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="3cd0b-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-revokesigninsessionss-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="3cd0b-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="3cd0b-139">Response</span></span>
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
