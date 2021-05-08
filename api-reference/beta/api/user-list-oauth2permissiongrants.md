---
title: Lista oauth2PermissionGrants
description: Recuperar uma lista de objetos oAuth2PermissionGrant, representando concessões de permissão delegadas.
localization_priority: Priority
doc_type: apiPageType
ms.prod: identity-and-sign-in
author: psignoret
ms.openlocfilehash: b2bab33e8e78c7c42e7d47fd6dcf4a889579528b
ms.sourcegitcommit: 34891a1c601976166958be1aa04bab5936592b44
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2021
ms.locfileid: "52231788"
---
# <a name="list-oauth2permissiongrants"></a><span data-ttu-id="8f894-103">Lista oauth2PermissionGrants</span><span class="sxs-lookup"><span data-stu-id="8f894-103">List oauth2PermissionGrants</span></span>

<span data-ttu-id="8f894-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8f894-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8f894-105">Recuperar uma lista de entidades [oAuth2PermissionGrant](../resources/oAuth2PermissionGrant.md), que representam permissões delegadas concedidas para habilitar um aplicativo cliente para acessar uma API em nome do usuário.</span><span class="sxs-lookup"><span data-stu-id="8f894-105">Retrieve a list of [oAuth2PermissionGrant](../resources/oAuth2PermissionGrant.md) entities, which represent delegated permissions granted to enable a client application to access an API on behalf of the user.</span></span>

> [!NOTE]
> <span data-ttu-id="8f894-106">Consultar as concessões de permissão delegada para um usuário só retornará permissões delegadas para o usuário específico.</span><span class="sxs-lookup"><span data-stu-id="8f894-106">Querying the delegated permission grants for a user will only return delegated permissions grants that are specifically for the given user.</span></span> <span data-ttu-id="8f894-107">As permissões delegadas concedidas em nome de todos os usuários da organização _não_ são incluídas na resposta.</span><span class="sxs-lookup"><span data-stu-id="8f894-107">Delegated permissions granted on behalf of all users in the organization are _not_ included in the response.</span></span>

> [!NOTE]
> <span data-ttu-id="8f894-108">Essa solicitação pode ter atrasos de replicação para concessão de permissão delegada que foram criadas, atualizadas ou excluídas recentemente.</span><span class="sxs-lookup"><span data-stu-id="8f894-108">This request might have replication delays for delegated permission grants that were recently created, updated, or deleted.</span></span>

## <a name="permissions"></a><span data-ttu-id="8f894-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="8f894-109">Permissions</span></span>

<span data-ttu-id="8f894-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8f894-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8f894-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8f894-112">Permission type</span></span>      | <span data-ttu-id="8f894-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8f894-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8f894-114">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8f894-114">Delegated (work or school account)</span></span> | <span data-ttu-id="8f894-115">Directory.Read.All, DelegatedPermissionGrant.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="8f894-115">Directory.Read.All, DelegatedPermissionGrant.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="8f894-116">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8f894-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8f894-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8f894-117">Not supported.</span></span>    |
|<span data-ttu-id="8f894-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8f894-118">Application</span></span> | <span data-ttu-id="8f894-119">Directory.Read.All, DelegatedPermissionGrant.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8f894-119">Directory.Read.All, DelegatedPermissionGrant.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8f894-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8f894-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/oauth2PermissionGrants
GET /users/{id | userPrincipalName}/oauth2PermissionGrants
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8f894-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="8f894-121">Optional query parameters</span></span>

<span data-ttu-id="8f894-122">Este método dá suporte a [Parâmetros de consulta OData](/graph/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="8f894-122">This method supports the [OData query parameters](/graph/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8f894-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8f894-123">Request headers</span></span>

| <span data-ttu-id="8f894-124">Nome</span><span class="sxs-lookup"><span data-stu-id="8f894-124">Name</span></span>           | <span data-ttu-id="8f894-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="8f894-125">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="8f894-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="8f894-126">Authorization</span></span>  | <span data-ttu-id="8f894-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8f894-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="8f894-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8f894-129">Request body</span></span>

<span data-ttu-id="8f894-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="8f894-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8f894-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="8f894-131">Response</span></span>

<span data-ttu-id="8f894-132">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8f894-132">If successful, this method returns a `200 OK` response code and a collection of [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8f894-133">Exemplos</span><span class="sxs-lookup"><span data-stu-id="8f894-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="8f894-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8f894-134">Request</span></span>

<span data-ttu-id="8f894-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8f894-135">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="8f894-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="8f894-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_user_oAuth2PermissionGrants"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/users/7d54cb02-aaa3-4016-9f9c-a4b49422dd9b/oauth2PermissionGrants
```
# <a name="c"></a>[<span data-ttu-id="8f894-137">C#</span><span class="sxs-lookup"><span data-stu-id="8f894-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-user-oauth2permissiongrants-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8f894-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8f894-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-user-oauth2permissiongrants-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8f894-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8f894-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-user-oauth2permissiongrants-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8f894-140">Java</span><span class="sxs-lookup"><span data-stu-id="8f894-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-user-oauth2permissiongrants-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="8f894-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="8f894-141">Response</span></span>

<span data-ttu-id="8f894-142">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8f894-142">Here is an example of the response.</span></span> 

> <span data-ttu-id="8f894-143">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="8f894-143">**Note:** The response object shown here might be shortened for readability.</span></span>

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


