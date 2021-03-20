---
title: Obter authenticationMethod
description: Recupere as propriedades e as relações de um objeto authenticationMethod.
localization_priority: Normal
author: mmcla
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: ff118645edf0a303c5017d11e7cdbb1e770bab58
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50948981"
---
# <a name="get-authenticationmethod"></a><span data-ttu-id="d9802-103">Obter authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="d9802-103">Get authenticationMethod</span></span>

<span data-ttu-id="d9802-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d9802-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d9802-105">Recupere as propriedades e as relações de um [objeto authenticationMethod.](../resources/authenticationmethod.md)</span><span class="sxs-lookup"><span data-stu-id="d9802-105">Retrieve the properties and relationships of an [authenticationMethod](../resources/authenticationmethod.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="d9802-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="d9802-106">Permissions</span></span>

<span data-ttu-id="d9802-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d9802-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="permissions-acting-on-self"></a><span data-ttu-id="d9802-109">Permissões agindo em si mesmo</span><span class="sxs-lookup"><span data-stu-id="d9802-109">Permissions acting on self</span></span>

|<span data-ttu-id="d9802-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d9802-110">Permission type</span></span>      | <span data-ttu-id="d9802-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d9802-111">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="d9802-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d9802-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="d9802-113">UserAuthenticationMethod.Read, UserAuthenticationMethod.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d9802-113">UserAuthenticationMethod.Read, UserAuthenticationMethod.ReadWrite</span></span> |
| <span data-ttu-id="d9802-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d9802-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d9802-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d9802-115">Not supported.</span></span> |
| <span data-ttu-id="d9802-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d9802-116">Application</span></span>                            | <span data-ttu-id="d9802-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d9802-117">Not supported.</span></span> |

### <a name="permissions-acting-on-other-users"></a><span data-ttu-id="d9802-118">Permissões atuando em outros usuários</span><span class="sxs-lookup"><span data-stu-id="d9802-118">Permissions acting on other users</span></span>

|<span data-ttu-id="d9802-119">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d9802-119">Permission type</span></span>      | <span data-ttu-id="d9802-120">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d9802-120">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|:-----------------|
| <span data-ttu-id="d9802-121">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d9802-121">Delegated (work or school account)</span></span>     | <span data-ttu-id="d9802-122">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d9802-122">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="d9802-123">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d9802-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d9802-124">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d9802-124">Not supported.</span></span> |
| <span data-ttu-id="d9802-125">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d9802-125">Application</span></span>                            | <span data-ttu-id="d9802-126">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d9802-126">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |

<span data-ttu-id="d9802-127">Para cenários delegados em que um administrador está atuando em outro usuário, o administrador precisa de uma [das seguintes funções:](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)</span><span class="sxs-lookup"><span data-stu-id="d9802-127">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>
* <span data-ttu-id="d9802-128">Administrador global</span><span class="sxs-lookup"><span data-stu-id="d9802-128">Global admin</span></span>
* <span data-ttu-id="d9802-129">Leitor global</span><span class="sxs-lookup"><span data-stu-id="d9802-129">Global reader</span></span>
* <span data-ttu-id="d9802-130">Administrador de autenticação privilegiada</span><span class="sxs-lookup"><span data-stu-id="d9802-130">Privileged authentication admin</span></span>
* <span data-ttu-id="d9802-131">Administrador de autenticação (apenas vê números de telefone mascarados)</span><span class="sxs-lookup"><span data-stu-id="d9802-131">Authentication admin (only sees masked phone numbers)</span></span>

## <a name="http-request"></a><span data-ttu-id="d9802-132">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d9802-132">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/authentication/methods/{id}
GET /users/{id | userPrincipalName}/authentication/methods/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d9802-133">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="d9802-133">Optional query parameters</span></span>

<span data-ttu-id="d9802-134">Este método não dá suporte a parâmetros de consulta opcionais para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="d9802-134">This method does not support optional query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d9802-135">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d9802-135">Request headers</span></span>

| <span data-ttu-id="d9802-136">Nome</span><span class="sxs-lookup"><span data-stu-id="d9802-136">Name</span></span>      |<span data-ttu-id="d9802-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="d9802-137">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="d9802-138">Autorização</span><span class="sxs-lookup"><span data-stu-id="d9802-138">Authorization</span></span> | <span data-ttu-id="d9802-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d9802-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d9802-141">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d9802-141">Request body</span></span>

<span data-ttu-id="d9802-142">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d9802-142">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d9802-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="d9802-143">Response</span></span>

<span data-ttu-id="d9802-144">Se tiver êxito, este método retornará um código de `200 OK` resposta e o objeto [authenticationMethod](../resources/authenticationmethod.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d9802-144">If successful, this method returns a `200 OK` response code and the requested [authenticationMethod](../resources/authenticationmethod.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d9802-145">Exemplos</span><span class="sxs-lookup"><span data-stu-id="d9802-145">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d9802-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d9802-146">Request</span></span>

<span data-ttu-id="d9802-147">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="d9802-147">The following is an example of the request.</span></span>


```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/authentication/methods/{id}
```

### <a name="response"></a><span data-ttu-id="d9802-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="d9802-148">Response</span></span>

<span data-ttu-id="d9802-149">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="d9802-149">The following is an example of the response.</span></span>

> <span data-ttu-id="d9802-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d9802-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
