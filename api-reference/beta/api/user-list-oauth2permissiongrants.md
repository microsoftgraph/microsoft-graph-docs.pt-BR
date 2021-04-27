---
title: Lista oauth2PermissionGrants
description: Recuperar uma lista de objetos oAuth2PermissionGrant, representando concessões de permissão delegadas.
localization_priority: Priority
doc_type: apiPageType
ms.prod: identity-and-sign-in
author: psignoret
ms.openlocfilehash: 435d577ccf892b0cbf03a2899ec039150ae09f9f
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52052597"
---
# <a name="list-oauth2permissiongrants"></a><span data-ttu-id="2ef0a-103">Lista oauth2PermissionGrants</span><span class="sxs-lookup"><span data-stu-id="2ef0a-103">List oauth2PermissionGrants</span></span>

<span data-ttu-id="2ef0a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2ef0a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2ef0a-105">Recuperar uma lista de entidades [oAuth2PermissionGrant](../resources/oAuth2PermissionGrant.md), que representam permissões delegadas concedidas para habilitar um aplicativo cliente para acessar uma API em nome do usuário.</span><span class="sxs-lookup"><span data-stu-id="2ef0a-105">Retrieve a list of [oAuth2PermissionGrant](../resources/oAuth2PermissionGrant.md) entities, which represent delegated permissions granted to enable a client application to access an API on behalf of the user.</span></span>

> [!NOTE]
> <span data-ttu-id="2ef0a-106">Consultar as concessões de permissão delegada para um usuário só retornará permissões delegadas para o usuário específico.</span><span class="sxs-lookup"><span data-stu-id="2ef0a-106">Querying the delegated permission grants for a user will only return delegated permissions grants that are specifically for the given user.</span></span> <span data-ttu-id="2ef0a-107">As permissões delegadas concedidas em nome de todos os usuários da organização _não_ são incluídas na resposta.</span><span class="sxs-lookup"><span data-stu-id="2ef0a-107">Delegated permissions granted on behalf of all users in the organization are _not_ included in the response.</span></span>

## <a name="permissions"></a><span data-ttu-id="2ef0a-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="2ef0a-108">Permissions</span></span>

<span data-ttu-id="2ef0a-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2ef0a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2ef0a-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2ef0a-111">Permission type</span></span>      | <span data-ttu-id="2ef0a-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2ef0a-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2ef0a-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2ef0a-113">Delegated (work or school account)</span></span> | <span data-ttu-id="2ef0a-114">Directory.Read.All, DelegatedPermissionGrant.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="2ef0a-114">Directory.Read.All, DelegatedPermissionGrant.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="2ef0a-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2ef0a-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2ef0a-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2ef0a-116">Not supported.</span></span>    |
|<span data-ttu-id="2ef0a-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2ef0a-117">Application</span></span> | <span data-ttu-id="2ef0a-118">Directory.Read.All, DelegatedPermissionGrant.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2ef0a-118">Directory.Read.All, DelegatedPermissionGrant.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2ef0a-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2ef0a-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/oauth2PermissionGrants
GET /users/{id | userPrincipalName}/oauth2PermissionGrants
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2ef0a-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="2ef0a-120">Optional query parameters</span></span>

<span data-ttu-id="2ef0a-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="2ef0a-121">This method supports the [OData query parameters](/graph/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2ef0a-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2ef0a-122">Request headers</span></span>

| <span data-ttu-id="2ef0a-123">Nome</span><span class="sxs-lookup"><span data-stu-id="2ef0a-123">Name</span></span>           | <span data-ttu-id="2ef0a-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="2ef0a-124">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="2ef0a-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="2ef0a-125">Authorization</span></span>  | <span data-ttu-id="2ef0a-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2ef0a-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="2ef0a-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2ef0a-128">Request body</span></span>

<span data-ttu-id="2ef0a-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="2ef0a-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2ef0a-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="2ef0a-130">Response</span></span>

<span data-ttu-id="2ef0a-131">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2ef0a-131">If successful, this method returns a `200 OK` response code and a collection of [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="2ef0a-132">Exemplos</span><span class="sxs-lookup"><span data-stu-id="2ef0a-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="2ef0a-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2ef0a-133">Request</span></span>

<span data-ttu-id="2ef0a-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2ef0a-134">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="2ef0a-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="2ef0a-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_user_oAuth2PermissionGrants"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/users/7d54cb02-aaa3-4016-9f9c-a4b49422dd9b/oauth2PermissionGrants
```
# <a name="c"></a>[<span data-ttu-id="2ef0a-136">C#</span><span class="sxs-lookup"><span data-stu-id="2ef0a-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-user-oauth2permissiongrants-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2ef0a-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2ef0a-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-user-oauth2permissiongrants-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2ef0a-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2ef0a-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-user-oauth2permissiongrants-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2ef0a-139">Java</span><span class="sxs-lookup"><span data-stu-id="2ef0a-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-user-oauth2permissiongrants-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="2ef0a-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="2ef0a-140">Response</span></span>

<span data-ttu-id="2ef0a-141">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2ef0a-141">Here is an example of the response.</span></span> 

> <span data-ttu-id="2ef0a-142">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="2ef0a-142">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.oAuth2PermissionGrant",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "clientId": "85477313-ea43-4c7d-b8a4-54fed35d0b60",
      "consentType": "Principal",
      "expiryTime": "2021-09-19T07:06:52.6843299Z",
      "id": "E3NHhUPqfUy4pFT-010LYFo5-ycA-_5Fhl7nHbaJ7qACy1R9o6oWQJ-cpLSUIt2b",
      "principalId": "7d54cb02-aaa3-4016-9f9c-a4b49422dd9b",
      "resourceId": "27fb395a-fb00-45fe-865e-e71db689eea0",
      "scope": " Contacts.ReadWrite openid profile",
      "startTime": "0001-01-01T00:00:00Z"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List oAuth2PermissionGrants",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


