---
title: 'usuário: invalidateAllRefreshTokens'
description: Invalida todos os tokens de atualização do usuário emitidos para aplicativos (bem como os cookies de sessão no navegador de um usuário), redefinindo a propriedade **refreshTokensValidFromDateTime** do usuário para a data e hora atual. Geralmente, essa operação é executada (por usuário ou um administrador), se o usuário tem um dispositivo perdido ou roubado.  Essa operação seria impedir o acesso a qualquer dado da organização acessado por meio de aplicativos no dispositivo sem que o usuário pela primeira vez, sendo necessário para entrar novamente. Na verdade, essa operação seria forçar o usuário entrar novamente para todos os aplicativos que eles tenham anteriormente consentiu, independente do dispositivo.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 740829e4ebd3b64308e514ab1c7633db7f35e7d7
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27950176"
---
# <a name="user-invalidateallrefreshtokens"></a><span data-ttu-id="9c523-106">usuário: invalidateAllRefreshTokens</span><span class="sxs-lookup"><span data-stu-id="9c523-106">user: invalidateAllRefreshTokens</span></span>

> <span data-ttu-id="9c523-107">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="9c523-107">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9c523-108">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="9c523-108">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="9c523-109">Invalida todos os tokens de atualização do usuário emitidos para aplicativos (bem como os cookies de sessão no navegador de um usuário), redefinindo a propriedade **refreshTokensValidFromDateTime** do usuário para a data e hora atual.</span><span class="sxs-lookup"><span data-stu-id="9c523-109">Invalidates all of the user's refresh tokens issued to applications (as well as session cookies in a user's browser), by resetting the **refreshTokensValidFromDateTime** user property to the current date-time.</span></span> <span data-ttu-id="9c523-110">Geralmente, essa operação é executada (por usuário ou um administrador), se o usuário tem um dispositivo perdido ou roubado.</span><span class="sxs-lookup"><span data-stu-id="9c523-110">Typically, this operation is performed (by the user or an administrator) if the user has a lost or stolen device.</span></span>  <span data-ttu-id="9c523-111">Essa operação seria impedir o acesso a qualquer dado da organização acessado por meio de aplicativos no dispositivo sem que o usuário pela primeira vez, sendo necessário para entrar novamente.</span><span class="sxs-lookup"><span data-stu-id="9c523-111">This operation would prevent access to any of the organization's data accessed through applications on the device without the user first being required to sign in again.</span></span> <span data-ttu-id="9c523-112">Na verdade, essa operação seria forçar o usuário entrar novamente para todos os aplicativos que eles tenham anteriormente consentiu, independente do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="9c523-112">In fact, this operation would force the user to sign in again for all applications that they have previously consented to, independent of device.</span></span>

<span data-ttu-id="9c523-113">Para os desenvolvedores, se o aplicativo tenta resgatar um token de acesso delegado para este usuário, usando um token invalidado refresh, o aplicativo receberá um erro.</span><span class="sxs-lookup"><span data-stu-id="9c523-113">For developers, if the application attempts to redeem a delegated access token for this user by using an invalidated refresh token, the application will get an error.</span></span> <span data-ttu-id="9c523-114">Se isso acontecer, o aplicativo será necessário adquirir um novo token refresh fazendo uma solicitação ao ponto de extremidade autorizar, que irá forçar o usuário entrar.</span><span class="sxs-lookup"><span data-stu-id="9c523-114">If this happens, the application will need to acquire a new refresh token by making a request to the authorize endpoint, which will force the user to sign in.</span></span>

## <a name="permissions"></a><span data-ttu-id="9c523-115">Permissões</span><span class="sxs-lookup"><span data-stu-id="9c523-115">Permissions</span></span>
<span data-ttu-id="9c523-p105">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9c523-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

+ <span data-ttu-id="9c523-118">Para um aplicativo permitir o assinadas no usuário para invalidar aplicativos eles tenham consentiu: User.ReadWrite, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="9c523-118">For an application to allow the signed in user to invalidate applications they've consented to: User.ReadWrite, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>
+ <span data-ttu-id="9c523-119">Para um aplicativo permitir que um administrador invalidar aplicativos um usuário aceitou: Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="9c523-119">For an application to allow an administrator to invalidate applications a user has consented to: Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>

## <a name="http-request"></a><span data-ttu-id="9c523-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9c523-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/invalidateAllRefreshTokens
POST /users/{id | userPrincipalName}/invalidateAllRefreshTokens
```
## <a name="request-headers"></a><span data-ttu-id="9c523-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9c523-121">Request headers</span></span>
| <span data-ttu-id="9c523-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9c523-122">Header</span></span>       | <span data-ttu-id="9c523-123">Valor</span><span class="sxs-lookup"><span data-stu-id="9c523-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="9c523-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="9c523-124">Authorization</span></span>  | <span data-ttu-id="9c523-p106">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9c523-p106">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="9c523-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9c523-127">Request body</span></span>
<span data-ttu-id="9c523-128">Esta operação não possui nenhum conteúdo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="9c523-128">This operation has no request content.</span></span>

## <a name="response"></a><span data-ttu-id="9c523-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="9c523-129">Response</span></span>

<span data-ttu-id="9c523-130">Se bem sucedido, este método retorna um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="9c523-130">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="9c523-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9c523-131">Example</span></span>
<span data-ttu-id="9c523-132">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="9c523-132">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="9c523-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9c523-133">Request</span></span>
<span data-ttu-id="9c523-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9c523-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "user_invalidateallrefreshtokens"
}-->
```http
POST https://graph.microsoft.com/beta/me/invalidateAllRefreshTokens
```

##### <a name="response"></a><span data-ttu-id="9c523-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="9c523-135">Response</span></span>
<span data-ttu-id="9c523-136">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9c523-136">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "user: invalidateAllRefreshTokens",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
