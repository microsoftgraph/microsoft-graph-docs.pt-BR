---
title: A lista exclui coleção de permissionGrantPolicy
description: Recupere uma lista de conjuntos de condição que descrevem condições sob as quais um evento de concessão de permissão é excluído em uma política de concessão de permissão.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: psignoret
ms.openlocfilehash: 340b371ca1ffbcdb5e39b12c17cc34a0fe8ef96e
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/01/2020
ms.locfileid: "49523265"
---
# <a name="list-excludes-collection-of-permissiongrantpolicy"></a><span data-ttu-id="b9a25-103">A lista exclui coleção de permissionGrantPolicy</span><span class="sxs-lookup"><span data-stu-id="b9a25-103">List excludes collection of permissionGrantPolicy</span></span>

<span data-ttu-id="b9a25-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b9a25-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b9a25-105">Recupere os conjuntos de condição que são *excluídos* em um [permissionGrantPolicy](../resources/permissiongrantpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="b9a25-105">Retrieve the condition sets which are *excluded* in a [permissionGrantPolicy](../resources/permissiongrantpolicy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="b9a25-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="b9a25-106">Permissions</span></span>

<span data-ttu-id="b9a25-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b9a25-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b9a25-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b9a25-109">Permission type</span></span>      | <span data-ttu-id="b9a25-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b9a25-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b9a25-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b9a25-111">Delegated (work or school account)</span></span> | <span data-ttu-id="b9a25-112">Policy. Read. PermissionGrant, Directory. Read. All</span><span class="sxs-lookup"><span data-stu-id="b9a25-112">Policy.Read.PermissionGrant, Directory.Read.All</span></span> |
|<span data-ttu-id="b9a25-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b9a25-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b9a25-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b9a25-114">Not supported.</span></span>    |
|<span data-ttu-id="b9a25-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b9a25-115">Application</span></span> | <span data-ttu-id="b9a25-116">Policy. Read. PermissionGrant, Directory. Read. All</span><span class="sxs-lookup"><span data-stu-id="b9a25-116">Policy.Read.PermissionGrant, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b9a25-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b9a25-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /policies/permissionGrantPolicies/{id}/excludes
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b9a25-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="b9a25-118">Optional query parameters</span></span>

<span data-ttu-id="b9a25-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="b9a25-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b9a25-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b9a25-120">Request headers</span></span>

| <span data-ttu-id="b9a25-121">Nome</span><span class="sxs-lookup"><span data-stu-id="b9a25-121">Name</span></span>           | <span data-ttu-id="b9a25-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="b9a25-122">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="b9a25-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="b9a25-123">Authorization</span></span>  | <span data-ttu-id="b9a25-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b9a25-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="b9a25-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b9a25-126">Request body</span></span>

<span data-ttu-id="b9a25-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b9a25-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b9a25-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="b9a25-128">Response</span></span>

<span data-ttu-id="b9a25-129">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [permissionGrantConditionSet](../resources/permissiongrantconditionset.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b9a25-129">If successful, this method returns a `200 OK` response code and a collection of [permissionGrantConditionSet](../resources/permissiongrantconditionset.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b9a25-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b9a25-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="b9a25-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b9a25-131">Request</span></span>

<span data-ttu-id="b9a25-132">Veja a seguir um exemplo da solicitação para recuperar os conjuntos de condições de **exclusão** da política de concessão de permissão interna `microsoft-application-admin` .</span><span class="sxs-lookup"><span data-stu-id="b9a25-132">The following is an example of the request to retrieve the **excludes** condition sets of the built-on permission grant policy `microsoft-application-admin`.</span></span> <span data-ttu-id="b9a25-133">Essa política de concessão de permissão inclui todas as permissões delegadas e todas as permissões de aplicativo, excluindo permissões de aplicativo para o Microsoft Graph e permissões de aplicativo do Azure AD Graph.</span><span class="sxs-lookup"><span data-stu-id="b9a25-133">This permission grant policy includes all delegated permissions, and all application permissions excluding application permissions for Microsoft Graph and application permissions for Azure AD Graph.</span></span>



# <a name="http"></a>[<span data-ttu-id="b9a25-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="b9a25-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "permissiongrantpolicy_get_excludes"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/policies/permissionGrantPolicies/microsoft-application-admin/excludes
```
# <a name="c"></a>[<span data-ttu-id="b9a25-135">C#</span><span class="sxs-lookup"><span data-stu-id="b9a25-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/permissiongrantpolicy-get-excludes-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b9a25-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b9a25-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/permissiongrantpolicy-get-excludes-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b9a25-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b9a25-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/permissiongrantpolicy-get-excludes-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b9a25-138">Java</span><span class="sxs-lookup"><span data-stu-id="b9a25-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/permissiongrantpolicy-get-excludes-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="b9a25-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="b9a25-139">Response</span></span>

<span data-ttu-id="b9a25-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="b9a25-140">The following is an example of the response.</span></span>

> <span data-ttu-id="b9a25-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b9a25-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.permissionGrantConditionSet",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "c85b029f-4abf-47d8-ae61-d2a38299033a",
      "permissionClassification": "all",
      "permissionType": "application",
      "resourceApplication": "00000003-0000-0000-c000-000000000000",
      "permissions": [ "all" ],
      "clientApplicationIds": [ "all" ],
      "clientApplicationTenantIds": [ "all" ],
      "clientApplicationPublisherIds": [ "all" ],
      "clientApplicationsFromVerifiedPublisherOnly": false
    },
    {
      "id": "2a1fbb36-9d9a-42d8-8804-de2aa45aca80",
      "permissionClassification": "all",
      "permissionType": "application",
      "resourceApplication": "00000002-0000-0000-c000-000000000000",
      "permissions": [ "all" ],
      "clientApplicationIds": [ "all" ],
      "clientApplicationTenantIds": [ "all" ],
      "clientApplicationPublisherIds": [ "all" ],
      "clientApplicationsFromVerifiedPublisherOnly": false
    }
  ]
}
```
