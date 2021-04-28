---
title: Obter authenticationMethod
description: Recupere as propriedades e as relações de um objeto authenticationMethod.
localization_priority: Normal
author: mmcla
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 40f5a7ec777e17b1b19c7f33f354c607f53b5480
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52054620"
---
# <a name="get-authenticationmethod"></a><span data-ttu-id="99e58-103">Obter authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="99e58-103">Get authenticationMethod</span></span>

<span data-ttu-id="99e58-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="99e58-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="99e58-105">Recupere as propriedades e as relações de um [objeto authenticationMethod.](../resources/authenticationmethod.md)</span><span class="sxs-lookup"><span data-stu-id="99e58-105">Retrieve the properties and relationships of an [authenticationMethod](../resources/authenticationmethod.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="99e58-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="99e58-106">Permissions</span></span>

<span data-ttu-id="99e58-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="99e58-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="permissions-acting-on-self"></a><span data-ttu-id="99e58-109">Permissões agindo em si mesmo</span><span class="sxs-lookup"><span data-stu-id="99e58-109">Permissions acting on self</span></span>

|<span data-ttu-id="99e58-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="99e58-110">Permission type</span></span>      | <span data-ttu-id="99e58-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="99e58-111">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="99e58-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="99e58-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="99e58-113">UserAuthenticationMethod.Read, UserAuthenticationMethod.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="99e58-113">UserAuthenticationMethod.Read, UserAuthenticationMethod.ReadWrite</span></span> |
| <span data-ttu-id="99e58-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="99e58-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="99e58-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="99e58-115">Not supported.</span></span> |
| <span data-ttu-id="99e58-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="99e58-116">Application</span></span>                            | <span data-ttu-id="99e58-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="99e58-117">Not supported.</span></span> |

### <a name="permissions-acting-on-other-users"></a><span data-ttu-id="99e58-118">Permissões atuando em outros usuários</span><span class="sxs-lookup"><span data-stu-id="99e58-118">Permissions acting on other users</span></span>

|<span data-ttu-id="99e58-119">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="99e58-119">Permission type</span></span>      | <span data-ttu-id="99e58-120">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="99e58-120">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|:-----------------|
| <span data-ttu-id="99e58-121">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="99e58-121">Delegated (work or school account)</span></span>     | <span data-ttu-id="99e58-122">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="99e58-122">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="99e58-123">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="99e58-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="99e58-124">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="99e58-124">Not supported.</span></span> |
| <span data-ttu-id="99e58-125">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="99e58-125">Application</span></span>                            | <span data-ttu-id="99e58-126">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="99e58-126">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |

<span data-ttu-id="99e58-127">Para cenários delegados em que um administrador está atuando em outro usuário, o administrador precisa de uma [das seguintes funções:](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)</span><span class="sxs-lookup"><span data-stu-id="99e58-127">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>
* <span data-ttu-id="99e58-128">Administração global</span><span class="sxs-lookup"><span data-stu-id="99e58-128">Global admin</span></span>
* <span data-ttu-id="99e58-129">Leitor global</span><span class="sxs-lookup"><span data-stu-id="99e58-129">Global reader</span></span>
* <span data-ttu-id="99e58-130">Administrador de autenticação privilegiada</span><span class="sxs-lookup"><span data-stu-id="99e58-130">Privileged authentication admin</span></span>
* <span data-ttu-id="99e58-131">Administrador de autenticação (apenas vê números de telefone mascarados)</span><span class="sxs-lookup"><span data-stu-id="99e58-131">Authentication admin (only sees masked phone numbers)</span></span>

## <a name="http-request"></a><span data-ttu-id="99e58-132">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="99e58-132">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/authentication/methods/{id}
GET /users/{id | userPrincipalName}/authentication/methods/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="99e58-133">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="99e58-133">Optional query parameters</span></span>

<span data-ttu-id="99e58-134">Este método não dá suporte a parâmetros de consulta opcionais para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="99e58-134">This method does not support optional query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="99e58-135">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="99e58-135">Request headers</span></span>

| <span data-ttu-id="99e58-136">Nome</span><span class="sxs-lookup"><span data-stu-id="99e58-136">Name</span></span>      |<span data-ttu-id="99e58-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="99e58-137">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="99e58-138">Autorização</span><span class="sxs-lookup"><span data-stu-id="99e58-138">Authorization</span></span> | <span data-ttu-id="99e58-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="99e58-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="99e58-141">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="99e58-141">Request body</span></span>

<span data-ttu-id="99e58-142">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="99e58-142">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="99e58-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="99e58-143">Response</span></span>

<span data-ttu-id="99e58-144">Se tiver êxito, este método retornará um código de `200 OK` resposta e o objeto [authenticationMethod](../resources/authenticationmethod.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="99e58-144">If successful, this method returns a `200 OK` response code and the requested [authenticationMethod](../resources/authenticationmethod.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="99e58-145">Exemplos</span><span class="sxs-lookup"><span data-stu-id="99e58-145">Examples</span></span>

### <a name="request"></a><span data-ttu-id="99e58-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="99e58-146">Request</span></span>

<span data-ttu-id="99e58-147">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="99e58-147">The following is an example of the request.</span></span>


```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/authentication/methods/{id}
```

### <a name="response"></a><span data-ttu-id="99e58-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="99e58-148">Response</span></span>

<span data-ttu-id="99e58-149">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="99e58-149">The following is an example of the response.</span></span>

> <span data-ttu-id="99e58-150">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="99e58-150">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.authenticationMethod"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.type": "#microsoft.graph.windowsHelloForBusinessAuthenticationMethod",
    "id": "b5e01f81-1f81-b5e0-811f-e0b5811fe0b5",
    "displayName": "Jordan's Surface Book",
    "createdDateTime": "2020-11-27T23:12:49Z",
    "keyStrength": "normal"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get authenticationMethod",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
