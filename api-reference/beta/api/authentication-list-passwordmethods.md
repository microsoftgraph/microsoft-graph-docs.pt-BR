---
title: Listar passwordMethods
description: Recupere uma lista de objetos passwordauthenticationmethod.
localization_priority: Normal
author: mmcla
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: f4425a47e7fede4f82a15fec1b04f0c7de655731
ms.sourcegitcommit: 9c16d84eac9c34134864ad63a9bb95c309218a44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/18/2020
ms.locfileid: "43557608"
---
# <a name="list-passwordmethods"></a><span data-ttu-id="c5f88-103">Listar passwordMethods</span><span class="sxs-lookup"><span data-stu-id="c5f88-103">List passwordMethods</span></span>

<span data-ttu-id="c5f88-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c5f88-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c5f88-105">Recupere uma lista de objetos de [método de autenticação de senha](../resources/passwordauthenticationmethod.md) .</span><span class="sxs-lookup"><span data-stu-id="c5f88-105">Retrieve a list of [password authentication method](../resources/passwordauthenticationmethod.md) objects.</span></span> <span data-ttu-id="c5f88-106">Isso retornará exatamente um objeto, pois um usuário pode ter exatamente uma senha.</span><span class="sxs-lookup"><span data-stu-id="c5f88-106">This will return exactly one object, as a user can have exactly one password.</span></span>

## <a name="permissions"></a><span data-ttu-id="c5f88-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="c5f88-107">Permissions</span></span>

<span data-ttu-id="c5f88-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c5f88-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c5f88-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c5f88-110">Permission type</span></span>                        | <span data-ttu-id="c5f88-111">Permissões que atuam em si (de menos para mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c5f88-111">Permissions acting on self (from least to most privileged)</span></span> | <span data-ttu-id="c5f88-112">Permissões que atuam em outros (de menos para mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c5f88-112">Permissions acting on others (from least to most privileged)</span></span>|
|:---------------------------------------|:-------------------------|:-----------------|
| <span data-ttu-id="c5f88-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c5f88-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="c5f88-114">UserAuthenticationMethod. Read, UserAuthenticationMethod. Read. All, UserAuthenticationMethod. ReadWrite, UserAuthenticationMethod. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="c5f88-114">UserAuthenticationMethod.Read, UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite, UserAuthenticationMethod.ReadWrite.All</span></span> | <span data-ttu-id="c5f88-115">UserAuthenticationMethod. Read. All, UserAuthenticationMethod. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="c5f88-115">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="c5f88-116">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c5f88-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c5f88-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c5f88-117">Not supported.</span></span> | <span data-ttu-id="c5f88-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c5f88-118">Not supported.</span></span> |
| <span data-ttu-id="c5f88-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c5f88-119">Application</span></span>                            | <span data-ttu-id="c5f88-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c5f88-120">Not supported.</span></span> | <span data-ttu-id="c5f88-121">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c5f88-121">Not supported.</span></span> |

<span data-ttu-id="c5f88-122">Para cenários delegados em que um administrador está agindo em outro usuário, o administrador precisa [de uma das seguintes funções](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span><span class="sxs-lookup"><span data-stu-id="c5f88-122">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>
* <span data-ttu-id="c5f88-123">Administrador global</span><span class="sxs-lookup"><span data-stu-id="c5f88-123">Global admin</span></span>
* <span data-ttu-id="c5f88-124">Leitor global</span><span class="sxs-lookup"><span data-stu-id="c5f88-124">Global reader</span></span>
* <span data-ttu-id="c5f88-125">Administrador de autenticação privilegiada</span><span class="sxs-lookup"><span data-stu-id="c5f88-125">Privileged authentication admin</span></span>
* <span data-ttu-id="c5f88-126">Administrador de autenticação</span><span class="sxs-lookup"><span data-stu-id="c5f88-126">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="c5f88-127">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c5f88-127">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/authentication/passwordMethods
GET /users/{id}/authentication/passwordMethods
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c5f88-128">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="c5f88-128">Optional query parameters</span></span>

<span data-ttu-id="c5f88-129">Este método não oferece suporte a parâmetros de consulta opcionais para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="c5f88-129">This method does not support optional query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c5f88-130">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c5f88-130">Request headers</span></span>

| <span data-ttu-id="c5f88-131">Nome</span><span class="sxs-lookup"><span data-stu-id="c5f88-131">Name</span></span>      |<span data-ttu-id="c5f88-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="c5f88-132">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="c5f88-133">Autorização</span><span class="sxs-lookup"><span data-stu-id="c5f88-133">Authorization</span></span> | <span data-ttu-id="c5f88-134">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="c5f88-134">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="c5f88-135">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c5f88-135">Request body</span></span>

<span data-ttu-id="c5f88-136">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c5f88-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c5f88-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="c5f88-137">Response</span></span>

<span data-ttu-id="c5f88-138">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [passwordAuthenticationMethod](../resources/passwordauthenticationmethod.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c5f88-138">If successful, this method returns a `200 OK` response code and a collection of [passwordAuthenticationMethod](../resources/passwordauthenticationmethod.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c5f88-139">Exemplos</span><span class="sxs-lookup"><span data-stu-id="c5f88-139">Examples</span></span>

### <a name="request"></a><span data-ttu-id="c5f88-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c5f88-140">Request</span></span>

<span data-ttu-id="c5f88-141">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="c5f88-141">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_passwordmethods"
}-->

```http
GET https://graph.microsoft.com/beta/me/authentication/passwordMethods
```

### <a name="response"></a><span data-ttu-id="c5f88-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="c5f88-142">Response</span></span>

<span data-ttu-id="c5f88-143">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="c5f88-143">The following is an example of the response.</span></span>

> <span data-ttu-id="c5f88-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c5f88-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.passwordAuthenticationMethod",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "28c10230-6103-485e-b985-444c60001490",
      "password": null,
      "creationDateTime": null
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List passwordMethods",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->