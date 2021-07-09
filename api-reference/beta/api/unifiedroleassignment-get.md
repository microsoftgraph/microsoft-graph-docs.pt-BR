---
title: Obter unifiedRoleAssignment
description: Recupere as propriedades e as relações de um objeto unifiedRoleAssignment.
localization_priority: Normal
author: abhijeetsinha
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 238b2e1d6049ec53d779fddba830338b13b6f781
ms.sourcegitcommit: 4888ac7504533344c4fc6828e2a06a002a1d72d3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/09/2021
ms.locfileid: "53351033"
---
# <a name="get-unifiedroleassignment"></a><span data-ttu-id="e3efb-103">Obter unifiedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="e3efb-103">Get unifiedRoleAssignment</span></span>

<span data-ttu-id="e3efb-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e3efb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e3efb-105">Recupere as propriedades e as relações de um [objeto unifiedRoleAssignment.](../resources/unifiedroleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="e3efb-105">Retrieve the properties and relationships of a [unifiedRoleAssignment](../resources/unifiedroleassignment.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="e3efb-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="e3efb-106">Permissions</span></span>

<span data-ttu-id="e3efb-107">Dependendo do provedor RBAC e do tipo de permissão (delegado ou aplicativo) necessário, escolha na tabela a seguinte permissão com menos privilégios necessária para chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="e3efb-107">Depending on the RBAC provider and the permission type (delegated or application) that is needed, choose from the following table the least privileged permission required to call this API.</span></span> <span data-ttu-id="e3efb-108">Para saber mais, incluindo [tomar cuidado](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) antes de escolher as permissões mais privilegiadas, pesquise as seguintes permissões em [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e3efb-108">To learn more, including [taking caution](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) before choosing more privileged permissions, search for the following permissions in [Permissions](/graph/permissions-reference).</span></span>

### <a name="for-directory-azure-ad-provider"></a><span data-ttu-id="e3efb-109">Provedor do Azure AD (Diretório)</span><span class="sxs-lookup"><span data-stu-id="e3efb-109">For Directory (Azure AD) provider</span></span>

|<span data-ttu-id="e3efb-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e3efb-110">Permission type</span></span>      | <span data-ttu-id="e3efb-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e3efb-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e3efb-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e3efb-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="e3efb-113">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="e3efb-113">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>   |
|<span data-ttu-id="e3efb-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e3efb-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e3efb-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e3efb-115">Not supported.</span></span>    |
|<span data-ttu-id="e3efb-116">Application</span><span class="sxs-lookup"><span data-stu-id="e3efb-116">Application</span></span> | <span data-ttu-id="e3efb-117">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e3efb-117">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span></span> |

### <a name="for-entitlement-management-provider"></a><span data-ttu-id="e3efb-118">Para provedor de gerenciamento de direitos</span><span class="sxs-lookup"><span data-stu-id="e3efb-118">For Entitlement management provider</span></span>

|<span data-ttu-id="e3efb-119">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e3efb-119">Permission type</span></span>      | <span data-ttu-id="e3efb-120">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e3efb-120">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e3efb-121">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e3efb-121">Delegated (work or school account)</span></span> |  <span data-ttu-id="e3efb-122">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e3efb-122">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span>  |
|<span data-ttu-id="e3efb-123">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e3efb-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e3efb-124">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e3efb-124">Not supported.</span></span>    |
|<span data-ttu-id="e3efb-125">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e3efb-125">Application</span></span> | <span data-ttu-id="e3efb-126">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e3efb-126">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e3efb-127">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e3efb-127">HTTP request</span></span>

<span data-ttu-id="e3efb-128">Obter uma atribuição de função para um provedor de diretórios:</span><span class="sxs-lookup"><span data-stu-id="e3efb-128">Get a role assignment for a directory provider:</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /roleManagement/directory/roleAssignments/{id}
```

<span data-ttu-id="e3efb-129">Obter uma atribuição de função para o provedor de gerenciamento de direitos:</span><span class="sxs-lookup"><span data-stu-id="e3efb-129">Get a role assignment for the entitlement management provider:</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /roleManagement/entitlementManagement/roleAssignments/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e3efb-130">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="e3efb-130">Optional query parameters</span></span>

<span data-ttu-id="e3efb-131">Este método dá suporte a Parâmetros de consulta do OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="e3efb-131">This method supports OData query parameters to help customize the response.</span></span> <span data-ttu-id="e3efb-132">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="e3efb-132">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="e3efb-133">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e3efb-133">Request headers</span></span>

| <span data-ttu-id="e3efb-134">Nome</span><span class="sxs-lookup"><span data-stu-id="e3efb-134">Name</span></span>      |<span data-ttu-id="e3efb-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="e3efb-135">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="e3efb-136">Autorização</span><span class="sxs-lookup"><span data-stu-id="e3efb-136">Authorization</span></span> | <span data-ttu-id="e3efb-137">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="e3efb-137">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="e3efb-138">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e3efb-138">Request body</span></span>

<span data-ttu-id="e3efb-139">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e3efb-139">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e3efb-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="e3efb-140">Response</span></span>

<span data-ttu-id="e3efb-141">Se tiver êxito, este método retornará um código de resposta e `200 OK` o objeto [unifiedRoleAssignment](../resources/unifiedroleassignment.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e3efb-141">If successful, this method returns a `200 OK` response code and the requested [unifiedRoleAssignment](../resources/unifiedroleassignment.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e3efb-142">Exemplos</span><span class="sxs-lookup"><span data-stu-id="e3efb-142">Examples</span></span>

### <a name="example-1--get-details-of-a-role-assignment"></a><span data-ttu-id="e3efb-143">Exemplo 1 : Obter detalhes de uma atribuição de função</span><span class="sxs-lookup"><span data-stu-id="e3efb-143">Example 1 : Get details of a role assignment</span></span>

#### <a name="request"></a><span data-ttu-id="e3efb-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e3efb-144">Request</span></span>

<span data-ttu-id="e3efb-145">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="e3efb-145">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="e3efb-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="e3efb-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_unifiedroleassignment_1"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/roleManagement/directory/roleAssignments/lAPpYvVpN0KRkAEhdxReEJC2sEqbR_9Hr48lds9SGHI-1
```
# <a name="c"></a>[<span data-ttu-id="e3efb-147">C#</span><span class="sxs-lookup"><span data-stu-id="e3efb-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-unifiedroleassignment-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e3efb-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e3efb-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-unifiedroleassignment-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e3efb-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e3efb-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-unifiedroleassignment-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e3efb-150">Java</span><span class="sxs-lookup"><span data-stu-id="e3efb-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-unifiedroleassignment-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="e3efb-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="e3efb-151">Response</span></span>

<span data-ttu-id="e3efb-152">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="e3efb-152">The following is an example of the response.</span></span>

> <span data-ttu-id="e3efb-153">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="e3efb-153">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-2-get-details-of-a-role-assignment-with-expand"></a><span data-ttu-id="e3efb-154">Exemplo 2: Obter detalhes de uma atribuição de função com `$expand`</span><span class="sxs-lookup"><span data-stu-id="e3efb-154">Example 2: Get details of a role assignment with `$expand`</span></span>

#### <a name="request"></a><span data-ttu-id="e3efb-155">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e3efb-155">Request</span></span>

<span data-ttu-id="e3efb-156">A seguir, um exemplo da solicitação com o `$expand` parâmetro de consulta.</span><span class="sxs-lookup"><span data-stu-id="e3efb-156">The following is an example of the request with the `$expand` query parameter.</span></span>


# <a name="http"></a>[<span data-ttu-id="e3efb-157">HTTP</span><span class="sxs-lookup"><span data-stu-id="e3efb-157">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_unifiedroleassignment_2"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/roleManagement/directory/roleAssignments/lAPpYvVpN0KRkAEhdxReEJC2sEqbR_9Hr48lds9SGHI-1?$expand=roleDefinition,principal,directoryScope
```
# <a name="c"></a>[<span data-ttu-id="e3efb-158">C#</span><span class="sxs-lookup"><span data-stu-id="e3efb-158">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-unifiedroleassignment-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e3efb-159">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e3efb-159">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-unifiedroleassignment-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e3efb-160">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e3efb-160">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-unifiedroleassignment-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e3efb-161">Java</span><span class="sxs-lookup"><span data-stu-id="e3efb-161">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-unifiedroleassignment-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="e3efb-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="e3efb-162">Response</span></span>

<span data-ttu-id="e3efb-163">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="e3efb-163">The following is an example of the response.</span></span>
> <span data-ttu-id="e3efb-164">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="e3efb-164">**Note:** The response object shown here might be shortened for readability.</span></span>

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


