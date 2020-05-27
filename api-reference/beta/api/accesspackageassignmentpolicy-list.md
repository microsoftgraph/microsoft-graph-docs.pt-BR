---
title: Listar accessPackageAssignmentPolicies
description: Recupere uma lista de objetos accessPackageAssignmentPolicy.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: c3d2a732bdc8ecc9fc0b4efded56f4d9751c8d11
ms.sourcegitcommit: 7a6231aeb570ff45d01b3db3df07a411f9f60fd1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/27/2020
ms.locfileid: "44383508"
---
# <a name="list-accesspackageassignmentpolicies"></a><span data-ttu-id="1038a-103">Listar accessPackageAssignmentPolicies</span><span class="sxs-lookup"><span data-stu-id="1038a-103">List accessPackageAssignmentPolicies</span></span>

<span data-ttu-id="1038a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1038a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1038a-105">No [Gerenciamento de direitos do Azure ad](../resources/entitlementmanagement-root.md), recupere uma lista de objetos [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="1038a-105">In [Azure AD entitlement management](../resources/entitlementmanagement-root.md), retrieve a list of [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) objects.</span></span> <span data-ttu-id="1038a-106">Se o usuário delegado estiver em uma função de diretório, a lista resultante incluirá todas as políticas de atribuição que o chamador tem acesso para ler, entre todos os catálogos e pacotes de acesso.</span><span class="sxs-lookup"><span data-stu-id="1038a-106">If the delegated user is in a directory role, the resulting list includes all the assignment policies that the caller has access to read, across all catalogs and access packages.</span></span>  <span data-ttu-id="1038a-107">Se o usuário delegado for um Gerenciador de pacotes do Access ou proprietário do catálogo, ele deverá recuperar as políticas para os pacotes do Access que eles podem ler com o [accessPackages de lista](accesspackage-list.md) incluindo `$expand=accessPackageAssignmentPolicies` como um parâmetro de consulta.</span><span class="sxs-lookup"><span data-stu-id="1038a-107">If the delegated user is an access package manager or catalog owner, they should instead retrieve the policies for the access packages they can read with [list accessPackages](accesspackage-list.md) by including `$expand=accessPackageAssignmentPolicies` as a query parameter.</span></span>

## <a name="permissions"></a><span data-ttu-id="1038a-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="1038a-108">Permissions</span></span>

<span data-ttu-id="1038a-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1038a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1038a-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1038a-111">Permission type</span></span>                        | <span data-ttu-id="1038a-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1038a-112">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="1038a-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1038a-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="1038a-114">EntitlementManagement. Read. All, EntitlementManagement. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="1038a-114">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="1038a-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1038a-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1038a-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1038a-116">Not supported.</span></span> |
| <span data-ttu-id="1038a-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1038a-117">Application</span></span>                            | <span data-ttu-id="1038a-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1038a-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1038a-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1038a-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityGovernance/entitlementManagement/accessPackageAssignmentPolicies
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1038a-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="1038a-120">Optional query parameters</span></span>

<span data-ttu-id="1038a-121">Este método oferece suporte a alguns dos parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="1038a-121">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="1038a-122">Por exemplo, para recuperar uma política de atribuição de pacote do Access com um nome de exibição especificado, inclua `$filter=displayName eq 'Employee sales support'` na consulta.</span><span class="sxs-lookup"><span data-stu-id="1038a-122">For example, to retrieve an access package assignment policy with a specified display name, include `$filter=displayName eq 'Employee sales support'` in the query.</span></span> <span data-ttu-id="1038a-123">Para obter informações gerais, confira [parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="1038a-123">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="1038a-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1038a-124">Request headers</span></span>

| <span data-ttu-id="1038a-125">Nome</span><span class="sxs-lookup"><span data-stu-id="1038a-125">Name</span></span>      |<span data-ttu-id="1038a-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="1038a-126">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="1038a-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="1038a-127">Authorization</span></span> | <span data-ttu-id="1038a-128">\{token\} de portador.</span><span class="sxs-lookup"><span data-stu-id="1038a-128">Bearer \{token\}.</span></span> <span data-ttu-id="1038a-129">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1038a-129">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1038a-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1038a-130">Request body</span></span>

<span data-ttu-id="1038a-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1038a-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1038a-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="1038a-132">Response</span></span>

<span data-ttu-id="1038a-133">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1038a-133">If successful, this method returns a `200 OK` response code and a collection of [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1038a-134">Exemplos</span><span class="sxs-lookup"><span data-stu-id="1038a-134">Examples</span></span>

### <a name="request"></a><span data-ttu-id="1038a-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1038a-135">Request</span></span>

<span data-ttu-id="1038a-136">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="1038a-136">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="1038a-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="1038a-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accesspackageassignmentpolicies"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignmentPolicies
```
# <a name="c"></a>[<span data-ttu-id="1038a-138">C#</span><span class="sxs-lookup"><span data-stu-id="1038a-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accesspackageassignmentpolicies-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1038a-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1038a-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accesspackageassignmentpolicies-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1038a-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1038a-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accesspackageassignmentpolicies-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="1038a-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="1038a-141">Response</span></span>

<span data-ttu-id="1038a-142">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="1038a-142">The following is an example of the response.</span></span>

> <span data-ttu-id="1038a-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1038a-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
