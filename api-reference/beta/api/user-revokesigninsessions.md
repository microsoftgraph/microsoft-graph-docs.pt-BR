---
title: 'usuário: revokeSignInSessions'
description: Invalida todos os tokens de atualização do usuário emitidos para aplicativos (bem como cookies de sessão no navegador de um usuário), redefinindo a propriedade de usuário **signInSessionsValidFromDateTime** para a data e hora atual.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 607b89201958ec2c8062109e2e02b1749b1c96ef
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32536590"
---
# <a name="user-revokesigninsessions"></a><span data-ttu-id="949a4-103">usuário: revokeSignInSessions</span><span class="sxs-lookup"><span data-stu-id="949a4-103">user: revokeSignInSessions</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="949a4-104">Invalida todos os tokens de atualização emitidos para aplicativos para um usuário (bem como cookies de sessão no navegador do usuário), redefinindo a propriedade de usuário **signInSessionsValidFromDateTime** para a data e hora atual.</span><span class="sxs-lookup"><span data-stu-id="949a4-104">Invalidates all the refresh tokens issued to applications for a user (as well as session cookies in a user's browser), by resetting the **signInSessionsValidFromDateTime** user property to the current date-time.</span></span> <span data-ttu-id="949a4-105">Normalmente, essa operação é executada (pelo usuário ou por um administrador) se o usuário tiver um dispositivo perdido ou roubado.</span><span class="sxs-lookup"><span data-stu-id="949a4-105">Typically, this operation is performed (by the user or an administrator) if the user has a lost or stolen device.</span></span> <span data-ttu-id="949a4-106">Essa operação impede o acesso aos dados da organização por meio de aplicativos no dispositivo solicitando que o usuário entre novamente em todos os aplicativos para os quais tenham sido consentidos anteriormente, independentemente do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="949a4-106">This operation prevents access to the organization's data through applications on the device by requiring the user to sign in again to all applications that they have previously consented to, independent of device.</span></span>

<span data-ttu-id="949a4-107">Se o aplicativo tentar resgatar um token de acesso delegado para esse usuário usando um token de atualização invalidado, o aplicativo receberá um erro.</span><span class="sxs-lookup"><span data-stu-id="949a4-107">If the application attempts to redeem a delegated access token for this user by using an invalidated refresh token, the application will get an error.</span></span> <span data-ttu-id="949a4-108">Se isso acontecer, o aplicativo precisará adquirir um novo token de atualização fazendo uma solicitação para o ponto de extremidade de autorização, que forçará o usuário a entrar.</span><span class="sxs-lookup"><span data-stu-id="949a4-108">If this happens, the application will need to acquire a new refresh token by making a request to the authorize endpoint, which will force the user to sign in.</span></span>

## <a name="permissions"></a><span data-ttu-id="949a4-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="949a4-109">Permissions</span></span>
<span data-ttu-id="949a4-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="949a4-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="949a4-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="949a4-112">Permission type</span></span>                        | <span data-ttu-id="949a4-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="949a4-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="949a4-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="949a4-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="949a4-115">User. ReadWrite, Directory. ReadWrite. All, Directory. AccessAsUser. All</span><span class="sxs-lookup"><span data-stu-id="949a4-115">User.ReadWrite, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="949a4-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="949a4-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="949a4-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="949a4-117">Not supported.</span></span> |
|<span data-ttu-id="949a4-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="949a4-118">Application</span></span>                            | <span data-ttu-id="949a4-119">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="949a4-119">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="949a4-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="949a4-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/revokeSignInSessions
POST /users/{id | userPrincipalName}/revokeSignInSessions
```
## <a name="request-headers"></a><span data-ttu-id="949a4-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="949a4-121">Request headers</span></span>
| <span data-ttu-id="949a4-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="949a4-122">Header</span></span>       | <span data-ttu-id="949a4-123">Valor</span><span class="sxs-lookup"><span data-stu-id="949a4-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="949a4-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="949a4-124">Authorization</span></span>  | <span data-ttu-id="949a4-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="949a4-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="949a4-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="949a4-127">Request body</span></span>
<span data-ttu-id="949a4-128">Esta operação não tem conteúdo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="949a4-128">This operation has no request content.</span></span>

## <a name="response"></a><span data-ttu-id="949a4-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="949a4-129">Response</span></span>

<span data-ttu-id="949a4-130">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="949a4-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="949a4-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="949a4-131">Example</span></span>
<span data-ttu-id="949a4-132">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="949a4-132">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="949a4-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="949a4-133">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "user_revokesigninsessionss"
}-->
```http
POST https://graph.microsoft.com/beta/me/revokeSignInSessions
```

##### <a name="response"></a><span data-ttu-id="949a4-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="949a4-134">Response</span></span>
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
    "Error: /api-reference/beta/api/user-revokesigninsessions.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
