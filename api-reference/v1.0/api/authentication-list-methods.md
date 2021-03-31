---
title: Métodos de List
description: Recupere uma lista de objetos do método de autenticação.
localization_priority: Normal
author: mmcla
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 1cca7f87bc5eb6b0c12108b0214ab81db99f0568
ms.sourcegitcommit: 8ca598ac70647bf4f897361ee90d3aa31d2ecca5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/31/2021
ms.locfileid: "51468594"
---
# <a name="list-methods"></a><span data-ttu-id="39909-103">Métodos de List</span><span class="sxs-lookup"><span data-stu-id="39909-103">List methods</span></span>

<span data-ttu-id="39909-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="39909-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="39909-105">Recupere uma lista de objetos [do método de autenticação.](../resources/authenticationmethod.md)</span><span class="sxs-lookup"><span data-stu-id="39909-105">Retrieve a list of [authentication method](../resources/authenticationmethod.md) objects.</span></span>

> <span data-ttu-id="39909-106">**Observação:** Somente os métodos suportados no v1.0 serão retornados.</span><span class="sxs-lookup"><span data-stu-id="39909-106">**Note:** Only methods supported on v1.0 will be returned.</span></span>

## <a name="permissions"></a><span data-ttu-id="39909-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="39909-107">Permissions</span></span>

<span data-ttu-id="39909-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="39909-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="permissions-acting-on-self"></a><span data-ttu-id="39909-110">Permissões agindo em si mesmo</span><span class="sxs-lookup"><span data-stu-id="39909-110">Permissions acting on self</span></span>

|<span data-ttu-id="39909-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="39909-111">Permission type</span></span>      | <span data-ttu-id="39909-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="39909-112">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="39909-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="39909-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="39909-114">UserAuthenticationMethod.Read, UserAuthenticationMethod.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="39909-114">UserAuthenticationMethod.Read, UserAuthenticationMethod.ReadWrite</span></span> |
| <span data-ttu-id="39909-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="39909-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="39909-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="39909-116">Not supported.</span></span> |
| <span data-ttu-id="39909-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="39909-117">Application</span></span>                            | <span data-ttu-id="39909-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="39909-118">Not supported.</span></span> |

### <a name="permissions-acting-on-other-users"></a><span data-ttu-id="39909-119">Permissões atuando em outros usuários</span><span class="sxs-lookup"><span data-stu-id="39909-119">Permissions acting on other users</span></span>

|<span data-ttu-id="39909-120">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="39909-120">Permission type</span></span>      | <span data-ttu-id="39909-121">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="39909-121">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|:-----------------|
| <span data-ttu-id="39909-122">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="39909-122">Delegated (work or school account)</span></span>     | <span data-ttu-id="39909-123">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="39909-123">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="39909-124">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="39909-124">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="39909-125">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="39909-125">Not supported.</span></span> |
| <span data-ttu-id="39909-126">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="39909-126">Application</span></span>                            | <span data-ttu-id="39909-127">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="39909-127">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |

<span data-ttu-id="39909-128">Para cenários delegados em que um administrador está atuando em outro usuário, o administrador precisa de uma [das seguintes funções:](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)</span><span class="sxs-lookup"><span data-stu-id="39909-128">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>
* <span data-ttu-id="39909-129">Administrador global</span><span class="sxs-lookup"><span data-stu-id="39909-129">Global admin</span></span>
* <span data-ttu-id="39909-130">Leitor global</span><span class="sxs-lookup"><span data-stu-id="39909-130">Global reader</span></span>
* <span data-ttu-id="39909-131">Administrador de autenticação privilegiada</span><span class="sxs-lookup"><span data-stu-id="39909-131">Privileged authentication admin</span></span>
* <span data-ttu-id="39909-132">Administrador de autenticação (apenas vê números de telefone mascarados)</span><span class="sxs-lookup"><span data-stu-id="39909-132">Authentication admin (only sees masked phone numbers)</span></span>

## <a name="http-request"></a><span data-ttu-id="39909-133">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="39909-133">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/authentication/methods
GET /users/{id | userPrincipalName}/authentication/methods
```

## <a name="optional-query-parameters"></a><span data-ttu-id="39909-134">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="39909-134">Optional query parameters</span></span>

<span data-ttu-id="39909-135">Este método não dá suporte a parâmetros de consulta opcionais para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="39909-135">This method does not support optional query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="39909-136">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="39909-136">Request headers</span></span>

| <span data-ttu-id="39909-137">Nome</span><span class="sxs-lookup"><span data-stu-id="39909-137">Name</span></span>      |<span data-ttu-id="39909-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="39909-138">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="39909-139">Autorização</span><span class="sxs-lookup"><span data-stu-id="39909-139">Authorization</span></span> | <span data-ttu-id="39909-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="39909-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="39909-142">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="39909-142">Request body</span></span>

<span data-ttu-id="39909-143">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="39909-143">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="39909-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="39909-144">Response</span></span>

<span data-ttu-id="39909-145">Se tiver êxito, este método retornará um código de resposta e uma coleção de objetos `200 OK` [authenticationMethod](../resources/authenticationmethod.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="39909-145">If successful, this method returns a `200 OK` response code and a collection of [authenticationMethod](../resources/authenticationmethod.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="39909-146">Exemplos</span><span class="sxs-lookup"><span data-stu-id="39909-146">Examples</span></span>

### <a name="request"></a><span data-ttu-id="39909-147">Solicitação</span><span class="sxs-lookup"><span data-stu-id="39909-147">Request</span></span>

<span data-ttu-id="39909-148">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="39909-148">The following is an example of the request.</span></span>


```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/authentication/methods
```

### <a name="response"></a><span data-ttu-id="39909-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="39909-149">Response</span></span>

<span data-ttu-id="39909-150">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="39909-150">The following is an example of the response.</span></span>

> <span data-ttu-id="39909-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="39909-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.authenticationMethod",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.fido2AuthenticationMethod",
      "id": "-2_GRUg2-HYz6_1YG4YRAQ2",
      "displayName": "Red key",
      "creationDateTime": "2020-08-10T06:44:09Z",
      "aaGuid": "2fc0579f-8113-47ea-b116-555a8db9202a",
      "model": "NFC key",
      "attestationCertificates": [
          "dbe793efdf1945e2df25d93653a1e8a3268a9075"
      ],
      "attestationLevel": "attested"
    },
    {
    "@odata.type": "#microsoft.graph.windowsHelloForBusinessAuthenticationMethod",
    "id": "b5e01f81-1f81-b5e0-811f-e0b5811fe0b5",
    "displayName": "Jordan's Surface Book",
    "createdDateTime": "2020-11-27T23:12:49Z",
    "keyStrength": "normal"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List methods",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
