---
title: Listar accessPackageAssignments
description: Recupere uma lista de objetos accesspackageassignment.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: be1f603eaf1f6cd5ea429219495ab9ed4a26b4ce
ms.sourcegitcommit: 79267b6d78c3510ef609953c5a664e692794caaa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/21/2020
ms.locfileid: "45197041"
---
# <a name="list-accesspackageassignments"></a><span data-ttu-id="a9ba7-103">Listar accessPackageAssignments</span><span class="sxs-lookup"><span data-stu-id="a9ba7-103">List accessPackageAssignments</span></span>

<span data-ttu-id="a9ba7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a9ba7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a9ba7-105">No [Gerenciamento de direitos do Azure ad](../resources/entitlementmanagement-root.md), recupere uma lista de objetos [accessPackageAssignment](../resources/accesspackageassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="a9ba7-105">In [Azure AD entitlement management](../resources/entitlementmanagement-root.md), retrieve a list of [accessPackageAssignment](../resources/accesspackageassignment.md) objects.</span></span> <span data-ttu-id="a9ba7-106">A lista resultante inclui todas as atribuições, atuais e bem como expiradas, que o chamador tem acesso para leitura, entre todos os catálogos e pacotes de acesso.</span><span class="sxs-lookup"><span data-stu-id="a9ba7-106">The resulting list includes all the assignments, current and well as expired, that the caller has access to read, across all catalogs and access packages.</span></span>

## <a name="permissions"></a><span data-ttu-id="a9ba7-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="a9ba7-107">Permissions</span></span>

<span data-ttu-id="a9ba7-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a9ba7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a9ba7-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a9ba7-110">Permission type</span></span>                        | <span data-ttu-id="a9ba7-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a9ba7-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="a9ba7-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a9ba7-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="a9ba7-113">EntitlementManagement. Read. All, EntitlementManagement. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="a9ba7-113">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="a9ba7-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a9ba7-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a9ba7-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a9ba7-115">Not supported.</span></span> |
| <span data-ttu-id="a9ba7-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a9ba7-116">Application</span></span>                            | <span data-ttu-id="a9ba7-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a9ba7-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a9ba7-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a9ba7-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityGovernance/entitlementManagement/accessPackageAssignments
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a9ba7-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="a9ba7-119">Optional query parameters</span></span>

<span data-ttu-id="a9ba7-120">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="a9ba7-120">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="a9ba7-121">Por exemplo, para retornar também o assunto de destino e o pacote de acesso, inclua `$expand=target,accessPackage` .</span><span class="sxs-lookup"><span data-stu-id="a9ba7-121">For example, to also return the target subject and access package, include `$expand=target,accessPackage`.</span></span> <span data-ttu-id="a9ba7-122">Para recuperar apenas as atribuições entregues, você pode incluir uma consulta `$filter=assignmentState eq 'Delivered'` .</span><span class="sxs-lookup"><span data-stu-id="a9ba7-122">To retrieve only delivered assignments, you can include a query `$filter=assignmentState eq 'Delivered'`.</span></span> <span data-ttu-id="a9ba7-123">Para recuperar apenas as atribuições de um usuário específico, você pode incluir uma consulta com atribuições direcionadas à ID do objeto do usuário: `$expand=target&$filter=target/objectid+eq+'7deff43e-1f17-44ef-9e5f-d516b0ba11d4'` .</span><span class="sxs-lookup"><span data-stu-id="a9ba7-123">To retrieve only assignments for a particular user, you can include a query with assignments targeting the object ID of that user: `$expand=target&$filter=target/objectid+eq+'7deff43e-1f17-44ef-9e5f-d516b0ba11d4'`.</span></span>  <span data-ttu-id="a9ba7-124">Para recuperar somente as atribuições de um determinado usuário e um pacote de acesso específico, você pode incluir uma consulta com atribuições direcionando o pacote de acesso e a ID do objeto desse usuário: `$expand=accessPackage,target&$filter=accessPackage/id eq '9bbe5f7d-f1e7-4eb1-a586-38cdf6f8b1ea' and target/objectid eq '7deff43e-1f17-44ef-9e5f-d516b0ba11d4'` .</span><span class="sxs-lookup"><span data-stu-id="a9ba7-124">To retrieve only assignments for a particular user and a particular access package, you can include a query with assignments targeting that access package and the object ID of that user: `$expand=accessPackage,target&$filter=accessPackage/id eq '9bbe5f7d-f1e7-4eb1-a586-38cdf6f8b1ea' and target/objectid eq '7deff43e-1f17-44ef-9e5f-d516b0ba11d4'`.</span></span>  <span data-ttu-id="a9ba7-125">Para recuperar apenas atribuições resultantes de uma determinada política de atribuição de pacote de acesso, você pode incluir uma consulta para essa política: `$filter=accessPackageAssignmentPolicy/id eq 'd92ebb54-9b46-492d-ab7f-01f76767da7f'` .</span><span class="sxs-lookup"><span data-stu-id="a9ba7-125">To retrieve only assignments resulting from a particular access package assignment policy, you can include a query for that policy: `$filter=accessPackageAssignmentPolicy/id eq 'd92ebb54-9b46-492d-ab7f-01f76767da7f'`.</span></span>

<span data-ttu-id="a9ba7-126">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="a9ba7-126">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="a9ba7-127">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a9ba7-127">Request headers</span></span>

| <span data-ttu-id="a9ba7-128">Nome</span><span class="sxs-lookup"><span data-stu-id="a9ba7-128">Name</span></span>      |<span data-ttu-id="a9ba7-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="a9ba7-129">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="a9ba7-130">Autorização</span><span class="sxs-lookup"><span data-stu-id="a9ba7-130">Authorization</span></span> | <span data-ttu-id="a9ba7-131">\{token\} de portador.</span><span class="sxs-lookup"><span data-stu-id="a9ba7-131">Bearer \{token\}.</span></span> <span data-ttu-id="a9ba7-132">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a9ba7-132">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a9ba7-133">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a9ba7-133">Request body</span></span>

<span data-ttu-id="a9ba7-134">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a9ba7-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a9ba7-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="a9ba7-135">Response</span></span>

<span data-ttu-id="a9ba7-136">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [accessPackageAssignment](../resources/accesspackageassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a9ba7-136">If successful, this method returns a `200 OK` response code and a collection of [accessPackageAssignment](../resources/accesspackageassignment.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a9ba7-137">Exemplos</span><span class="sxs-lookup"><span data-stu-id="a9ba7-137">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a9ba7-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a9ba7-138">Request</span></span>

<span data-ttu-id="a9ba7-139">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="a9ba7-139">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a9ba7-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="a9ba7-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accesspackageassignments"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignments
```
# <a name="c"></a>[<span data-ttu-id="a9ba7-141">C#</span><span class="sxs-lookup"><span data-stu-id="a9ba7-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accesspackageassignments-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a9ba7-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a9ba7-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accesspackageassignments-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a9ba7-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a9ba7-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accesspackageassignments-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="a9ba7-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="a9ba7-144">Response</span></span>

<span data-ttu-id="a9ba7-145">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="a9ba7-145">The following is an example of the response.</span></span>

> <span data-ttu-id="a9ba7-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a9ba7-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessPackageAssignment",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "9bdae7b4-6ece-487b-9eb8-9679dbd67aa2",
      "catalogId": "cc30dc98-6d3c-4fa0-bed8-fd76d0efd993",
      "accessPackageId": "e3f47362-993f-4fcb-8a38-532ffca16150",
      "assignmentPolicyId": "63ebd106-8116-40e7-a0ab-01ae475d11bb",
      "targetId": "ab4291f6-66b7-42bf-b597-a05b29414f5c",
      "assignmentStatus": "ExpiredNotificationTriggered",
      "assignmentState": "Expired",
      "isExtended": false,
      "expiredDateTime": "2019-04-25T23:45:40.42Z"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List accessPackageAssignments",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
