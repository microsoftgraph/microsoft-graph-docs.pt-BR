---
title: Listar accessPackageAssignmentPolicies
description: Recupere uma lista de objetos accessPackageAssignmentPolicy.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: d2e823980dc9966a5f3e85eef82d00c606e5c180
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37935048"
---
# <a name="list-accesspackageassignmentpolicies"></a><span data-ttu-id="64fb9-103">Listar accessPackageAssignmentPolicies</span><span class="sxs-lookup"><span data-stu-id="64fb9-103">List accessPackageAssignmentPolicies</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="64fb9-104">No [Gerenciamento de direitos do Azure ad](../resources/entitlementmanagement-root.md), recupere uma lista de objetos [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="64fb9-104">In [Azure AD entitlement management](../resources/entitlementmanagement-root.md), retrieve a list of [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) objects.</span></span>   <span data-ttu-id="64fb9-105">A lista resultante inclui todas as políticas de atribuição às quais o chamador tem acesso para leitura, entre todos os catálogos e pacotes de acesso.</span><span class="sxs-lookup"><span data-stu-id="64fb9-105">The resulting list includes all the assignment policies which the caller has access to read, across all catalogs and access packages.</span></span>

## <a name="permissions"></a><span data-ttu-id="64fb9-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="64fb9-106">Permissions</span></span>

<span data-ttu-id="64fb9-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="64fb9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="64fb9-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="64fb9-109">Permission type</span></span>                        | <span data-ttu-id="64fb9-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="64fb9-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="64fb9-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="64fb9-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="64fb9-112">EntitlementManagement. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="64fb9-112">EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="64fb9-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="64fb9-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="64fb9-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="64fb9-114">Not supported.</span></span> |
| <span data-ttu-id="64fb9-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="64fb9-115">Application</span></span>                            | <span data-ttu-id="64fb9-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="64fb9-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="64fb9-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="64fb9-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityGovernance/entitlementManagement/accessPackageAssignmentPolicies
```

## <a name="optional-query-parameters"></a><span data-ttu-id="64fb9-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="64fb9-118">Optional query parameters</span></span>

<span data-ttu-id="64fb9-119">Este método oferece suporte a alguns dos parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="64fb9-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="64fb9-120">Por exemplo, para recuperar uma política de atribuição de pacote do Access com um nome de exibição `$filter=displayName eq 'Employee sales support'` especificado, inclua na consulta.</span><span class="sxs-lookup"><span data-stu-id="64fb9-120">For example, to retrieve a access package assignment policy with a specifed display name, include `$filter=displayName eq 'Employee sales support'` in the query.</span></span> <span data-ttu-id="64fb9-121">Para obter informações gerais, confira [parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="64fb9-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="64fb9-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="64fb9-122">Request headers</span></span>

| <span data-ttu-id="64fb9-123">Nome</span><span class="sxs-lookup"><span data-stu-id="64fb9-123">Name</span></span>      |<span data-ttu-id="64fb9-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="64fb9-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="64fb9-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="64fb9-125">Authorization</span></span> | <span data-ttu-id="64fb9-126">\{token\} de portador.</span><span class="sxs-lookup"><span data-stu-id="64fb9-126">Bearer \{token\}.</span></span> <span data-ttu-id="64fb9-127">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="64fb9-127">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="64fb9-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="64fb9-128">Request body</span></span>

<span data-ttu-id="64fb9-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="64fb9-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="64fb9-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="64fb9-130">Response</span></span>

<span data-ttu-id="64fb9-131">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="64fb9-131">If successful, this method returns a `200 OK` response code and a collection of [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="64fb9-132">Exemplos</span><span class="sxs-lookup"><span data-stu-id="64fb9-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="64fb9-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="64fb9-133">Request</span></span>

<span data-ttu-id="64fb9-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="64fb9-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_accesspackageassignmentpolicies"
}-->

```http
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignmentPolicies
```

### <a name="response"></a><span data-ttu-id="64fb9-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="64fb9-135">Response</span></span>

<span data-ttu-id="64fb9-136">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="64fb9-136">The following is an example of the response.</span></span>

> <span data-ttu-id="64fb9-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="64fb9-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
      "isEnabled": false,
      "canExtend": false,
      "durationInDays": 365
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
