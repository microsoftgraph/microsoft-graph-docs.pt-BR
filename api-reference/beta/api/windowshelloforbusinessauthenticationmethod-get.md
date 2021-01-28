---
title: Obter windowsHelloForBusinessAuthenticationMethod
description: Leia as propriedades e as relações de um objeto windowsHelloForBusinessAuthenticationMethod.
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 74181a0af8f2c6da8fde310ce70899522bb3b27b
ms.sourcegitcommit: 9a03b719d1316729dd022bf4d268894e91515475
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/28/2021
ms.locfileid: "50033880"
---
# <a name="get-windowshelloforbusinessauthenticationmethod"></a><span data-ttu-id="81773-103">Obter windowsHelloForBusinessAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="81773-103">Get windowsHelloForBusinessAuthenticationMethod</span></span>
<span data-ttu-id="81773-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="81773-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="81773-105">Leia as propriedades e as relações de um [objeto windowsHelloForBusinessAuthenticationMethod.](../resources/windowshelloforbusinessauthenticationmethod.md)</span><span class="sxs-lookup"><span data-stu-id="81773-105">Read the properties and relationships of a [windowsHelloForBusinessAuthenticationMethod](../resources/windowshelloforbusinessauthenticationmethod.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="81773-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="81773-106">Permissions</span></span>

<span data-ttu-id="81773-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="81773-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="permissions-acting-on-self"></a><span data-ttu-id="81773-109">Permissões agindo por si só</span><span class="sxs-lookup"><span data-stu-id="81773-109">Permissions acting on self</span></span>

|<span data-ttu-id="81773-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="81773-110">Permission type</span></span>      | <span data-ttu-id="81773-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="81773-111">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="81773-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="81773-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="81773-113">UserAuthenticationMethod.Read, UserAuthenticationMethod.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="81773-113">UserAuthenticationMethod.Read, UserAuthenticationMethod.ReadWrite</span></span> |
| <span data-ttu-id="81773-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="81773-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="81773-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="81773-115">Not supported.</span></span> |
| <span data-ttu-id="81773-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="81773-116">Application</span></span>                            | <span data-ttu-id="81773-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="81773-117">Not supported.</span></span> |

### <a name="permissions-acting-on-other-users"></a><span data-ttu-id="81773-118">Permissões atuando em outros usuários</span><span class="sxs-lookup"><span data-stu-id="81773-118">Permissions acting on other users</span></span>

|<span data-ttu-id="81773-119">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="81773-119">Permission type</span></span>      | <span data-ttu-id="81773-120">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="81773-120">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="81773-121">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="81773-121">Delegated (work or school account)</span></span>     | <span data-ttu-id="81773-122">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="81773-122">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="81773-123">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="81773-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="81773-124">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="81773-124">Not supported.</span></span> |
| <span data-ttu-id="81773-125">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="81773-125">Application</span></span>                            | <span data-ttu-id="81773-126">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="81773-126">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |

<span data-ttu-id="81773-127">Para cenários delegados em que um administrador está agindo em outro usuário, o administrador precisa [de uma das seguintes funções:](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)</span><span class="sxs-lookup"><span data-stu-id="81773-127">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>
* <span data-ttu-id="81773-128">Administração global</span><span class="sxs-lookup"><span data-stu-id="81773-128">Global admin</span></span>
* <span data-ttu-id="81773-129">Leitor global</span><span class="sxs-lookup"><span data-stu-id="81773-129">Global reader</span></span>
* <span data-ttu-id="81773-130">Administrador de autenticação privilegiada</span><span class="sxs-lookup"><span data-stu-id="81773-130">Privileged authentication admin</span></span>
* <span data-ttu-id="81773-131">Administrador de autenticação (vê apenas números de telefone com máscara)</span><span class="sxs-lookup"><span data-stu-id="81773-131">Authentication admin (only sees masked phone numbers)</span></span>

## <a name="http-request"></a><span data-ttu-id="81773-132">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="81773-132">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/authentication/windowsHelloForBusinessMethods/{windowsHelloForBusinessAuthenticationMethodId}
GET /users/{id | userPrincipalName}/authentication/windowsHelloForBusinessMethods/{windowsHelloForBusinessAuthenticationMethodId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="81773-133">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="81773-133">Optional query parameters</span></span>

<span data-ttu-id="81773-134">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="81773-134">Not supported.</span></span>

## <a name="request-headers"></a><span data-ttu-id="81773-135">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="81773-135">Request headers</span></span>
|<span data-ttu-id="81773-136">Nome</span><span class="sxs-lookup"><span data-stu-id="81773-136">Name</span></span>|<span data-ttu-id="81773-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="81773-137">Description</span></span>|
|:---|:---|
|<span data-ttu-id="81773-138">Autorização</span><span class="sxs-lookup"><span data-stu-id="81773-138">Authorization</span></span>|<span data-ttu-id="81773-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="81773-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="81773-141">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="81773-141">Request body</span></span>
<span data-ttu-id="81773-142">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="81773-142">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="81773-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="81773-143">Response</span></span>

<span data-ttu-id="81773-144">Se bem-sucedido, este método retorna um código de resposta e um objeto `200 OK` [windowsHelloForBusinessAuthenticationMethod](../resources/windowshelloforbusinessauthenticationmethod.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="81773-144">If successful, this method returns a `200 OK` response code and a [windowsHelloForBusinessAuthenticationMethod](../resources/windowshelloforbusinessauthenticationmethod.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="81773-145">Exemplos</span><span class="sxs-lookup"><span data-stu-id="81773-145">Examples</span></span>

### <a name="request"></a><span data-ttu-id="81773-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="81773-146">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_windowshelloforbusinessauthenticationmethod"
}
-->
``` http
GET https://graph.microsoft.com/beta/users/annie@contoso.com/authentication/windowsHelloForBusinessMethods/_jpuR-TGZtk6aQCLF3BQjA2
```

### <a name="response"></a><span data-ttu-id="81773-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="81773-147">Response</span></span>
<span data-ttu-id="81773-148">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="81773-148">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.windowsHelloForBusinessAuthenticationMethod"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsHelloForBusinessAuthenticationMethod",
    "id": "b5e01f81-1f81-b5e0-811f-e0b5811fe0b5",
    "displayName": "Jordan's Surface Book",
    "createdDateTime": "2020-11-27T23:12:49Z",
    "keyStrength": "normal"
  }
}
```

