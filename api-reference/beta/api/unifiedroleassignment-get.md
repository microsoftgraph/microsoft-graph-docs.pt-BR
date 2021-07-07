---
title: Obter unifiedRoleAssignment
description: Recupere as propriedades e as relações de um objeto unifiedRoleAssignment.
localization_priority: Normal
author: abhijeetsinha
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: e24f9a2ae184502123cca58188902d0f66782b87
ms.sourcegitcommit: ada6eab637b9b318129aefb98edbe7316399d9ba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/07/2021
ms.locfileid: "53317032"
---
# <a name="get-unifiedroleassignment"></a><span data-ttu-id="501d7-103">Obter unifiedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="501d7-103">Get unifiedRoleAssignment</span></span>

<span data-ttu-id="501d7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="501d7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="501d7-105">Recupere as propriedades e as relações de um [objeto unifiedRoleAssignment.](../resources/unifiedroleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="501d7-105">Retrieve the properties and relationships of a [unifiedRoleAssignment](../resources/unifiedroleassignment.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="501d7-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="501d7-106">Permissions</span></span>

<span data-ttu-id="501d7-107">Dependendo do provedor RBAC e do tipo de permissão (delegado ou aplicativo) necessário, escolha na tabela a seguinte permissão com menos privilégios necessária para chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="501d7-107">Depending on the RBAC provider and the permission type (delegated or application) that is needed, choose from the following table the least privileged permission required to call this API.</span></span> <span data-ttu-id="501d7-108">Para saber mais, incluindo [tomar cuidado](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) antes de escolher as permissões mais privilegiadas, pesquise as seguintes permissões em [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="501d7-108">To learn more, including [taking caution](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) before choosing more privileged permissions, search for the following permissions in [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="501d7-109">Provedor com suporte</span><span class="sxs-lookup"><span data-stu-id="501d7-109">Supported provider</span></span>      | <span data-ttu-id="501d7-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="501d7-110">Delegated (work or school account)</span></span>  | <span data-ttu-id="501d7-111">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="501d7-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="501d7-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="501d7-112">Application</span></span> |
|:-----------------------|:------------------------------------|:---------------------------------------|:------------|
| <span data-ttu-id="501d7-113">Diretório</span><span class="sxs-lookup"><span data-stu-id="501d7-113">Directory</span></span> | <span data-ttu-id="501d7-114">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="501d7-114">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> | <span data-ttu-id="501d7-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="501d7-115">Not supported.</span></span>| <span data-ttu-id="501d7-116">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="501d7-116">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span></span> |
| <span data-ttu-id="501d7-117">Gerenciamento de direitos</span><span class="sxs-lookup"><span data-stu-id="501d7-117">Entitlement management</span></span> | <span data-ttu-id="501d7-118">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="501d7-118">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> | <span data-ttu-id="501d7-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="501d7-119">Not supported.</span></span> | <span data-ttu-id="501d7-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="501d7-120">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="501d7-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="501d7-121">HTTP request</span></span>

<span data-ttu-id="501d7-122">Obter uma atribuição de função para um provedor de diretórios:</span><span class="sxs-lookup"><span data-stu-id="501d7-122">Get a role assignment for a directory provider:</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /roleManagement/directory/roleAssignments/{id}
```

<span data-ttu-id="501d7-123">Obter uma atribuição de função para o provedor de gerenciamento de direitos:</span><span class="sxs-lookup"><span data-stu-id="501d7-123">Get a role assignment for the entitlement management provider:</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /roleManagement/entitlementManagement/roleAssignments/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="501d7-124">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="501d7-124">Optional query parameters</span></span>

<span data-ttu-id="501d7-125">Este método dá suporte a Parâmetros de consulta do OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="501d7-125">This method supports OData query parameters to help customize the response.</span></span> <span data-ttu-id="501d7-126">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="501d7-126">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="501d7-127">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="501d7-127">Request headers</span></span>

| <span data-ttu-id="501d7-128">Nome</span><span class="sxs-lookup"><span data-stu-id="501d7-128">Name</span></span>      |<span data-ttu-id="501d7-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="501d7-129">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="501d7-130">Autorização</span><span class="sxs-lookup"><span data-stu-id="501d7-130">Authorization</span></span> | <span data-ttu-id="501d7-131">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="501d7-131">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="501d7-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="501d7-132">Request body</span></span>

<span data-ttu-id="501d7-133">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="501d7-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="501d7-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="501d7-134">Response</span></span>

<span data-ttu-id="501d7-135">Se tiver êxito, este método retornará um código de resposta e `200 OK` o objeto [unifiedRoleAssignment](../resources/unifiedroleassignment.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="501d7-135">If successful, this method returns a `200 OK` response code and the requested [unifiedRoleAssignment](../resources/unifiedroleassignment.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="501d7-136">Exemplos</span><span class="sxs-lookup"><span data-stu-id="501d7-136">Examples</span></span>

### <a name="example-1--get-details-of-a-role-assignment"></a><span data-ttu-id="501d7-137">Exemplo 1 : Obter detalhes de uma atribuição de função</span><span class="sxs-lookup"><span data-stu-id="501d7-137">Example 1 : Get details of a role assignment</span></span>

#### <a name="request"></a><span data-ttu-id="501d7-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="501d7-138">Request</span></span>

<span data-ttu-id="501d7-139">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="501d7-139">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="501d7-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="501d7-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_unifiedroleassignment_1"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/roleManagement/directory/roleAssignments/lAPpYvVpN0KRkAEhdxReEJC2sEqbR_9Hr48lds9SGHI-1
```
# <a name="c"></a>[<span data-ttu-id="501d7-141">C#</span><span class="sxs-lookup"><span data-stu-id="501d7-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-unifiedroleassignment-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="501d7-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="501d7-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-unifiedroleassignment-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="501d7-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="501d7-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-unifiedroleassignment-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="501d7-144">Java</span><span class="sxs-lookup"><span data-stu-id="501d7-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-unifiedroleassignment-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="501d7-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="501d7-145">Response</span></span>

<span data-ttu-id="501d7-146">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="501d7-146">The following is an example of the response.</span></span>

> <span data-ttu-id="501d7-147">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="501d7-147">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleAssignment"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#roleManagement/directory/roleAssignments/$entity",
    "id": "lAPpYvVpN0KRkAEhdxReEJC2sEqbR_9Hr48lds9SGHI-1",
    "roleDefinitionId": "62e90394-69f5-4237-9190-012177145e10",
    "principalId": "4ab0b690-479b-47ff-af8f-2576cf521872",
    "directoryScopeId": "28ca5a85-489a-49a0-b555-0a6d81e56f0"
}
```

### <a name="example-2-get-details-of-a-role-assignment-with-expand"></a><span data-ttu-id="501d7-148">Exemplo 2: Obter detalhes de uma atribuição de função com `$expand`</span><span class="sxs-lookup"><span data-stu-id="501d7-148">Example 2: Get details of a role assignment with `$expand`</span></span>

#### <a name="request"></a><span data-ttu-id="501d7-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="501d7-149">Request</span></span>

<span data-ttu-id="501d7-150">A seguir, um exemplo da solicitação com o `$expand` parâmetro de consulta.</span><span class="sxs-lookup"><span data-stu-id="501d7-150">The following is an example of the request with the `$expand` query parameter.</span></span>


# <a name="http"></a>[<span data-ttu-id="501d7-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="501d7-151">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_unifiedroleassignment_2"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/roleManagement/directory/roleAssignments/lAPpYvVpN0KRkAEhdxReEJC2sEqbR_9Hr48lds9SGHI-1?$expand=roleDefinition,principal,directoryScope
```
# <a name="c"></a>[<span data-ttu-id="501d7-152">C#</span><span class="sxs-lookup"><span data-stu-id="501d7-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-unifiedroleassignment-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="501d7-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="501d7-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-unifiedroleassignment-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="501d7-154">Objective-C</span><span class="sxs-lookup"><span data-stu-id="501d7-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-unifiedroleassignment-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="501d7-155">Java</span><span class="sxs-lookup"><span data-stu-id="501d7-155">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-unifiedroleassignment-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="501d7-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="501d7-156">Response</span></span>

<span data-ttu-id="501d7-157">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="501d7-157">The following is an example of the response.</span></span>
> <span data-ttu-id="501d7-158">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="501d7-158">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleAssignment"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#roleManagement/directory/roleAssignments/$entity",
    "@odata.type": "#microsoft.graph.unifiedRoleAssignment",
    "id": "lAPpYvVpN0KRkAEhdxReEJC2sEqbR_9Hr48lds9SGHI-1",
    "roleDefinitionId": "c2cf284d-6c41-4e6b-afac-4b80928c9034",
    "roleDefinition": {
      "id": "c2cf284d-6c41-4e6b-afac-4b80928c9034",
      "displayName": "Billing Administrator",
      "description": "Can perform common billing related tasks like updating payment information.",
      "rolePermissions": [
        {
          "allowedResourceActions": [
            "microsoft.commerce.billing/allEntities/allTasks",
            "microsoft.directory/organization/basic/update",
          ],
          "excludedResourceActions": []
        }],
      "isEnabled": true,
      },
    "principalId": "f8ca5a85-489a-49a0-b555-0a6d81e56f0d",
    "principal": {
      "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users/$entity",
      "id": "f8ca5a85-489a-49a0-b555-0a6d81e56f0d ",
      "userPrincipalName": "alice@contoso.com",
      "displayName": "Alice Smith"
    },
    "directoryScopeId": "28ca5a85-489a-49a0-b555-0a6d81e56f0d",
    "directoryScope": {
      "@odata.context": "https://graph.microsoft.com/beta/$metadata#organization/$entity",
      "id": "28ca5a85-489a-49a0-b555-0a6d81e56f0d",
      "displayName": "Contoso_Seattle_Admins"
    }
}
```
<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get unifiedRoleAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


