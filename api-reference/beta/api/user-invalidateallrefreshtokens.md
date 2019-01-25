---
title: 'usuário: invalidateAllRefreshTokens'
description: Invalida todos os tokens de atualização do usuário emitidos para aplicativos (bem como os cookies de sessão no navegador de um usuário), redefinindo a propriedade **refreshTokensValidFromDateTime** do usuário para a data e hora atual. Geralmente, essa operação é executada (por usuário ou um administrador), se o usuário tem um dispositivo perdido ou roubado.  Essa operação seria impedir o acesso a qualquer dado da organização acessado por meio de aplicativos no dispositivo sem que o usuário pela primeira vez, sendo necessário para entrar novamente. Na verdade, essa operação seria forçar o usuário entrar novamente para todos os aplicativos que eles tenham anteriormente consentiu, independente do dispositivo.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: c006787c0d68ae0c6ecbb331a9ff410f957a6f93
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29524524"
---
# <a name="user-invalidateallrefreshtokens"></a><span data-ttu-id="c371e-106">usuário: invalidateAllRefreshTokens</span><span class="sxs-lookup"><span data-stu-id="c371e-106">user: invalidateAllRefreshTokens</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c371e-107">Invalida todos os tokens de atualização do usuário emitidos para aplicativos (bem como os cookies de sessão no navegador de um usuário), redefinindo a propriedade **refreshTokensValidFromDateTime** do usuário para a data e hora atual.</span><span class="sxs-lookup"><span data-stu-id="c371e-107">Invalidates all of the user's refresh tokens issued to applications (as well as session cookies in a user's browser), by resetting the **refreshTokensValidFromDateTime** user property to the current date-time.</span></span> <span data-ttu-id="c371e-108">Geralmente, essa operação é executada (por usuário ou um administrador), se o usuário tem um dispositivo perdido ou roubado.</span><span class="sxs-lookup"><span data-stu-id="c371e-108">Typically, this operation is performed (by the user or an administrator) if the user has a lost or stolen device.</span></span>  <span data-ttu-id="c371e-109">Essa operação seria impedir o acesso a qualquer dado da organização acessado por meio de aplicativos no dispositivo sem que o usuário pela primeira vez, sendo necessário para entrar novamente.</span><span class="sxs-lookup"><span data-stu-id="c371e-109">This operation would prevent access to any of the organization's data accessed through applications on the device without the user first being required to sign in again.</span></span> <span data-ttu-id="c371e-110">Na verdade, essa operação seria forçar o usuário entrar novamente para todos os aplicativos que eles tenham anteriormente consentiu, independente do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="c371e-110">In fact, this operation would force the user to sign in again for all applications that they have previously consented to, independent of device.</span></span>

<span data-ttu-id="c371e-111">Para os desenvolvedores, se o aplicativo tenta resgatar um token de acesso delegado para este usuário, usando um token invalidado refresh, o aplicativo receberá um erro.</span><span class="sxs-lookup"><span data-stu-id="c371e-111">For developers, if the application attempts to redeem a delegated access token for this user by using an invalidated refresh token, the application will get an error.</span></span> <span data-ttu-id="c371e-112">Se isso acontecer, o aplicativo será necessário adquirir um novo token refresh fazendo uma solicitação ao ponto de extremidade autorizar, que irá forçar o usuário entrar.</span><span class="sxs-lookup"><span data-stu-id="c371e-112">If this happens, the application will need to acquire a new refresh token by making a request to the authorize endpoint, which will force the user to sign in.</span></span>

## <a name="permissions"></a><span data-ttu-id="c371e-113">Permissões</span><span class="sxs-lookup"><span data-stu-id="c371e-113">Permissions</span></span>
<span data-ttu-id="c371e-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c371e-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

+ <span data-ttu-id="c371e-116">Para um aplicativo permitir o assinadas no usuário para invalidar aplicativos eles tenham consentiu: User.ReadWrite, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="c371e-116">For an application to allow the signed in user to invalidate applications they've consented to: User.ReadWrite, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>
+ <span data-ttu-id="c371e-117">Para um aplicativo permitir que um administrador invalidar aplicativos um usuário aceitou: Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="c371e-117">For an application to allow an administrator to invalidate applications a user has consented to: Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>

## <a name="http-request"></a><span data-ttu-id="c371e-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c371e-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/invalidateAllRefreshTokens
POST /users/{id | userPrincipalName}/invalidateAllRefreshTokens
```
## <a name="request-headers"></a><span data-ttu-id="c371e-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c371e-119">Request headers</span></span>
| <span data-ttu-id="c371e-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c371e-120">Header</span></span>       | <span data-ttu-id="c371e-121">Valor</span><span class="sxs-lookup"><span data-stu-id="c371e-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="c371e-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="c371e-122">Authorization</span></span>  | <span data-ttu-id="c371e-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c371e-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c371e-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c371e-125">Request body</span></span>
<span data-ttu-id="c371e-126">Esta operação não possui nenhum conteúdo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="c371e-126">This operation has no request content.</span></span>

## <a name="response"></a><span data-ttu-id="c371e-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="c371e-127">Response</span></span>

<span data-ttu-id="c371e-128">Se bem sucedido, este método retorna um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="c371e-128">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="c371e-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c371e-129">Example</span></span>
<span data-ttu-id="c371e-130">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="c371e-130">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="c371e-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c371e-131">Request</span></span>
<span data-ttu-id="c371e-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c371e-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "user_invalidateallrefreshtokens"
}-->
```http
POST https://graph.microsoft.com/beta/me/invalidateAllRefreshTokens
```

##### <a name="response"></a><span data-ttu-id="c371e-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="c371e-133">Response</span></span>
<span data-ttu-id="c371e-134">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c371e-134">Here is an example of the response.</span></span> 
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
    "Error: /api-reference/beta/api/user-invalidateallrefreshtokens.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
