---
title: Lista oauth2PermissionGrants
description: Recuperar uma lista de objetos oAuth2PermissionGrant, representando concessões de permissão delegadas.
localization_priority: Priority
doc_type: apiPageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: b9ca5f2576d6f1e9dff8382ef3e69107260807ac
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50134537"
---
# <a name="list-oauth2permissiongrants"></a><span data-ttu-id="efb63-103">Lista oauth2PermissionGrants</span><span class="sxs-lookup"><span data-stu-id="efb63-103">List oauth2PermissionGrants</span></span>

<span data-ttu-id="efb63-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="efb63-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="efb63-105">Recuperar uma lista de entidades [oAuth2PermissionGrant](../resources/oAuth2PermissionGrant.md), representando permissões delegadas concedidas à entidade de serviço (que representa o aplicativo cliente) para acessar uma API em nome de um usuário.</span><span class="sxs-lookup"><span data-stu-id="efb63-105">Retrieve a list of [oAuth2PermissionGrant](../resources/oAuth2PermissionGrant.md) entities, representing delegated permissions granted to the service principal (representing the client application) to access an API on behalf of a user.</span></span>

## <a name="permissions"></a><span data-ttu-id="efb63-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="efb63-106">Permissions</span></span>

<span data-ttu-id="efb63-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="efb63-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="efb63-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="efb63-109">Permission type</span></span>      | <span data-ttu-id="efb63-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="efb63-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="efb63-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="efb63-111">Delegated (work or school account)</span></span> | <span data-ttu-id="efb63-112">Directory.Read.All, DelegatedPermissionGrant.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="efb63-112">Directory.Read.All, DelegatedPermissionGrant.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="efb63-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="efb63-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="efb63-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="efb63-114">Not supported.</span></span>    |
|<span data-ttu-id="efb63-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="efb63-115">Application</span></span> | <span data-ttu-id="efb63-116">Directory.Read.All, DelegatedPermissionGrant.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="efb63-116">Directory.Read.All, DelegatedPermissionGrant.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="efb63-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="efb63-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /servicePrincipals/{id}/oauth2PermissionGrants
```

## <a name="optional-query-parameters"></a><span data-ttu-id="efb63-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="efb63-118">Optional query parameters</span></span>

<span data-ttu-id="efb63-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="efb63-119">This method supports the [OData query parameters](/graph/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="efb63-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="efb63-120">Request headers</span></span>

| <span data-ttu-id="efb63-121">Nome</span><span class="sxs-lookup"><span data-stu-id="efb63-121">Name</span></span>           | <span data-ttu-id="efb63-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="efb63-122">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="efb63-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="efb63-123">Authorization</span></span>  | <span data-ttu-id="efb63-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="efb63-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="efb63-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="efb63-126">Request body</span></span>

<span data-ttu-id="efb63-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="efb63-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="efb63-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="efb63-128">Response</span></span>

<span data-ttu-id="efb63-129">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="efb63-129">If successful, this method returns a `200 OK` response code and collection of [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="efb63-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="efb63-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="efb63-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="efb63-131">Request</span></span>

<span data-ttu-id="efb63-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="efb63-132">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="efb63-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="efb63-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_servicePrincipal_oAuth2PermissionGrants"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/servicePrincipals/{id}/oauth2PermissionGrants
```
# <a name="c"></a>[<span data-ttu-id="efb63-134">C#</span><span class="sxs-lookup"><span data-stu-id="efb63-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-serviceprincipal-oauth2permissiongrants-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="efb63-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="efb63-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-serviceprincipal-oauth2permissiongrants-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="efb63-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="efb63-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-serviceprincipal-oauth2permissiongrants-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="efb63-137">Java</span><span class="sxs-lookup"><span data-stu-id="efb63-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-serviceprincipal-oauth2permissiongrants-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="efb63-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="efb63-138">Response</span></span>

<span data-ttu-id="efb63-139">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="efb63-139">Here is an example of the response.</span></span> 

> <span data-ttu-id="efb63-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="efb63-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

