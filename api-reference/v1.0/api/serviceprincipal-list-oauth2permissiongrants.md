---
title: List oauth2PermissionGrants
description: Recupere uma lista de objetos oAuth2PermissionGrant, representando as autorizações de permissão delegadas.
localization_priority: Priority
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: sureshja
ms.openlocfilehash: 8ee8df176c435ea24982334a8580d257c9da2d16
ms.sourcegitcommit: 7a6231aeb570ff45d01b3db3df07a411f9f60fd1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/27/2020
ms.locfileid: "44383963"
---
# <a name="list-oauth2permissiongrants"></a><span data-ttu-id="8af8a-103">List oauth2PermissionGrants</span><span class="sxs-lookup"><span data-stu-id="8af8a-103">List oauth2PermissionGrants</span></span>

<span data-ttu-id="8af8a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8af8a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="8af8a-105">Recupere uma lista de entidades [oAuth2PermissionGrant](../resources/oAuth2PermissionGrant.md) , representando as permissões delegadas concedidas à entidade de serviço (representando o aplicativo cliente) para acessar uma API em nome de um usuário.</span><span class="sxs-lookup"><span data-stu-id="8af8a-105">Retrieve a list of [oAuth2PermissionGrant](../resources/oAuth2PermissionGrant.md) entities, representing delegated permissions granted to the service principal (representing the client application) to access an API on behalf of a user.</span></span>

## <a name="permissions"></a><span data-ttu-id="8af8a-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="8af8a-106">Permissions</span></span>

<span data-ttu-id="8af8a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8af8a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8af8a-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8af8a-109">Permission type</span></span>      | <span data-ttu-id="8af8a-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8af8a-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8af8a-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8af8a-111">Delegated (work or school account)</span></span> | <span data-ttu-id="8af8a-112">Directory. Read. All, DelegatedPermissionGrant. ReadWrite. All, Directory. ReadWrite. All, Directory. AccessAsUser. All</span><span class="sxs-lookup"><span data-stu-id="8af8a-112">Directory.Read.All, DelegatedPermissionGrant.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="8af8a-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8af8a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8af8a-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8af8a-114">Not supported.</span></span>    |
|<span data-ttu-id="8af8a-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8af8a-115">Application</span></span> | <span data-ttu-id="8af8a-116">Directory. Read. All, DelegatedPermissionGrant. ReadWrite. All, Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="8af8a-116">Directory.Read.All, DelegatedPermissionGrant.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8af8a-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8af8a-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /servicePrincipals/{id}/oauth2PermissionGrants
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8af8a-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="8af8a-118">Optional query parameters</span></span>

<span data-ttu-id="8af8a-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="8af8a-119">This method supports the [OData query parameters](/graph/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8af8a-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8af8a-120">Request headers</span></span>

| <span data-ttu-id="8af8a-121">Nome</span><span class="sxs-lookup"><span data-stu-id="8af8a-121">Name</span></span>           | <span data-ttu-id="8af8a-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="8af8a-122">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="8af8a-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="8af8a-123">Authorization</span></span>  | <span data-ttu-id="8af8a-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8af8a-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="8af8a-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8af8a-126">Request body</span></span>

<span data-ttu-id="8af8a-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="8af8a-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8af8a-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="8af8a-128">Response</span></span>

<span data-ttu-id="8af8a-129">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8af8a-129">If successful, this method returns a `200 OK` response code and collection of [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8af8a-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="8af8a-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="8af8a-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8af8a-131">Request</span></span>

<span data-ttu-id="8af8a-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8af8a-132">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="8af8a-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="8af8a-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_servicePrincipal_oAuth2PermissionGrants"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/servicePrincipals/{id}/oauth2PermissionGrants
```
# <a name="c"></a>[<span data-ttu-id="8af8a-134">C#</span><span class="sxs-lookup"><span data-stu-id="8af8a-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-serviceprincipal-oauth2permissiongrants-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8af8a-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8af8a-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-serviceprincipal-oauth2permissiongrants-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8af8a-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8af8a-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-serviceprincipal-oauth2permissiongrants-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8af8a-137">Java</span><span class="sxs-lookup"><span data-stu-id="8af8a-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-serviceprincipal-oauth2permissiongrants-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="8af8a-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="8af8a-138">Response</span></span>

<span data-ttu-id="8af8a-139">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8af8a-139">Here is an example of the response.</span></span> 

> <span data-ttu-id="8af8a-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8af8a-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.oAuth2PermissionGrant",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 253

{
  "value": [
    {
      "id": "id-value",
      "clientId": "clientId-value",
      "consentType": "consentType-value",
      "principalId": "principalId-value",
      "resourceId": "resourceId-value",
      "scope": "scope-value"
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
