---
title: Listar accessPackageAssignmentPolicies
description: Recupere uma lista de objetos accessPackageAssignmentPolicy.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: be973adb399d60846282acd55f9d44d5968af7ce
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50439706"
---
# <a name="list-accesspackageassignmentpolicies"></a><span data-ttu-id="43086-103">Listar accessPackageAssignmentPolicies</span><span class="sxs-lookup"><span data-stu-id="43086-103">List accessPackageAssignmentPolicies</span></span>

<span data-ttu-id="43086-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="43086-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="43086-105">No gerenciamento de direitos do [Azure AD,](../resources/entitlementmanagement-root.md)recupere uma lista de [objetos accessPackageAssignmentPolicy.](../resources/accesspackageassignmentpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="43086-105">In [Azure AD entitlement management](../resources/entitlementmanagement-root.md), retrieve a list of [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) objects.</span></span> <span data-ttu-id="43086-106">Se o usuário delegado estiver em uma função de diretório, a lista resultante incluirá todas as políticas de atribuição que o chamador tem acesso à leitura, em todos os catálogos e pacotes de acesso.</span><span class="sxs-lookup"><span data-stu-id="43086-106">If the delegated user is in a directory role, the resulting list includes all the assignment policies that the caller has access to read, across all catalogs and access packages.</span></span>  <span data-ttu-id="43086-107">Se o usuário delegado for um gerenciador de pacotes de acesso ou proprietário de catálogo, ele deverá recuperar as políticas dos pacotes de acesso que podem ser lidos com [accessPackages](accesspackage-list.md) de lista incluindo como parâmetro de `$expand=accessPackageAssignmentPolicies` consulta.</span><span class="sxs-lookup"><span data-stu-id="43086-107">If the delegated user is an access package manager or catalog owner, they should instead retrieve the policies for the access packages they can read with [list accessPackages](accesspackage-list.md) by including `$expand=accessPackageAssignmentPolicies` as a query parameter.</span></span>

## <a name="permissions"></a><span data-ttu-id="43086-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="43086-108">Permissions</span></span>

<span data-ttu-id="43086-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="43086-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="43086-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="43086-111">Permission type</span></span>                        | <span data-ttu-id="43086-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="43086-112">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="43086-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="43086-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="43086-114">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="43086-114">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="43086-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="43086-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="43086-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="43086-116">Not supported.</span></span> |
| <span data-ttu-id="43086-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="43086-117">Application</span></span>                            | <span data-ttu-id="43086-118">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="43086-118">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="43086-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="43086-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityGovernance/entitlementManagement/accessPackageAssignmentPolicies
```

## <a name="optional-query-parameters"></a><span data-ttu-id="43086-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="43086-120">Optional query parameters</span></span>

<span data-ttu-id="43086-121">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="43086-121">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="43086-122">Por exemplo, para recuperar uma política de atribuição de pacote de acesso com um nome de exibição especificado, `$filter=displayName eq 'Employee sales support'` inclua na consulta.</span><span class="sxs-lookup"><span data-stu-id="43086-122">For example, to retrieve an access package assignment policy with a specified display name, include `$filter=displayName eq 'Employee sales support'` in the query.</span></span> <span data-ttu-id="43086-123">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="43086-123">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="43086-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="43086-124">Request headers</span></span>

| <span data-ttu-id="43086-125">Nome</span><span class="sxs-lookup"><span data-stu-id="43086-125">Name</span></span>      |<span data-ttu-id="43086-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="43086-126">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="43086-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="43086-127">Authorization</span></span> | <span data-ttu-id="43086-128">\{token\} de portador.</span><span class="sxs-lookup"><span data-stu-id="43086-128">Bearer \{token\}.</span></span> <span data-ttu-id="43086-129">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="43086-129">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="43086-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="43086-130">Request body</span></span>

<span data-ttu-id="43086-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="43086-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="43086-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="43086-132">Response</span></span>

<span data-ttu-id="43086-133">Se tiver êxito, este método retornará um código de resposta e uma coleção de `200 OK` [objetos accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="43086-133">If successful, this method returns a `200 OK` response code and a collection of [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="43086-134">Exemplos</span><span class="sxs-lookup"><span data-stu-id="43086-134">Examples</span></span>

### <a name="request"></a><span data-ttu-id="43086-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="43086-135">Request</span></span>

<span data-ttu-id="43086-136">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="43086-136">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="43086-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="43086-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accesspackageassignmentpolicies"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignmentPolicies
```
# <a name="c"></a>[<span data-ttu-id="43086-138">C#</span><span class="sxs-lookup"><span data-stu-id="43086-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accesspackageassignmentpolicies-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="43086-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="43086-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accesspackageassignmentpolicies-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="43086-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="43086-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accesspackageassignmentpolicies-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="43086-141">Java</span><span class="sxs-lookup"><span data-stu-id="43086-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-accesspackageassignmentpolicies-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="43086-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="43086-142">Response</span></span>

<span data-ttu-id="43086-143">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="43086-143">The following is an example of the response.</span></span>

> <span data-ttu-id="43086-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="43086-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessPackageAssignmentPolicy",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "b2eba9a1-b357-42ee-83a8-336522ed6cbf",
      "accessPackageId": "1b153a13-76da-4d07-9afa-c6c2b1f2e824",
      "displayName": "All Users",
      "description": "All users can request for access to the directory.",
      "canExtend": false,
      "durationInDays": 365,
      "accessReviewSettings": null
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List accessPackageAssignmentPolicies",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


