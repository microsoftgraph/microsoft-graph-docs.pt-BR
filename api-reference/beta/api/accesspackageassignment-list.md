---
title: Listar accessPackageAssignments
description: Recupere uma lista de objetos accesspackageassignment.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: a14bfbdf7785c378a132d308711d4fd21a815413
ms.sourcegitcommit: f51ba08d604d93f5f6af9ee8979cbf76baa285ce
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/19/2020
ms.locfileid: "42108424"
---
# <a name="list-accesspackageassignments"></a><span data-ttu-id="a9429-103">Listar accessPackageAssignments</span><span class="sxs-lookup"><span data-stu-id="a9429-103">List accessPackageAssignments</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a9429-104">No [Gerenciamento de direitos do Azure ad](../resources/entitlementmanagement-root.md), recupere uma lista de objetos [accessPackageAssignment](../resources/accesspackageassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="a9429-104">In [Azure AD entitlement management](../resources/entitlementmanagement-root.md), retrieve a list of [accessPackageAssignment](../resources/accesspackageassignment.md) objects.</span></span>  <span data-ttu-id="a9429-105">A lista resultante inclui todas as atribuições, atuais e bem como expiradas, que o chamador tem acesso para leitura, entre todos os catálogos e pacotes de acesso.</span><span class="sxs-lookup"><span data-stu-id="a9429-105">The resulting list includes all the assignments, current and well as expired, that the caller has access to read, across all catalogs and access packages.</span></span>

## <a name="permissions"></a><span data-ttu-id="a9429-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="a9429-106">Permissions</span></span>

<span data-ttu-id="a9429-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a9429-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a9429-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a9429-109">Permission type</span></span>                        | <span data-ttu-id="a9429-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a9429-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="a9429-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a9429-111">Delegated (work or school account)</span></span>     |  <span data-ttu-id="a9429-112">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a9429-112">EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="a9429-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a9429-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a9429-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a9429-114">Not supported.</span></span> |
| <span data-ttu-id="a9429-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a9429-115">Application</span></span>                            | <span data-ttu-id="a9429-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a9429-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a9429-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a9429-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityGovernance/entitlementManagement/accessPackageAssignments
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a9429-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="a9429-118">Optional query parameters</span></span>

<span data-ttu-id="a9429-119">Este método oferece suporte a alguns dos parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="a9429-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="a9429-120">Por exemplo, para retornar também o usuário de destino e o pacote de `$expand=target,accessPackage`acesso, inclua.</span><span class="sxs-lookup"><span data-stu-id="a9429-120">For example, to also return the target user and access package, include `$expand=target,accessPackage`.</span></span> <span data-ttu-id="a9429-121">Para recuperar apenas as atribuições entregues, você pode incluir `$filter=assignmentState eq 'Delivered'`uma consulta.</span><span class="sxs-lookup"><span data-stu-id="a9429-121">To retrieve only delivered assignments, you can include a query `$filter=assignmentState eq 'Delivered'`.</span></span> <span data-ttu-id="a9429-122">Para recuperar somente as atribuições de um usuário específico, você pode incluir uma consulta com atribuições direcionadas à ID `$expand=target&$filter=target/objectid+eq+'7deff43e-1f17-44ef-9e5f-d516b0ba11d4'`do objeto do usuário.</span><span class="sxs-lookup"><span data-stu-id="a9429-122">To retrieve only assignments for a particular user, you can include a query with assignments targeting the object ID of that user `$expand=target&$filter=target/objectid+eq+'7deff43e-1f17-44ef-9e5f-d516b0ba11d4'`.</span></span>  <span data-ttu-id="a9429-123">Para recuperar somente as atribuições de um determinado usuário e um pacote de acesso específico, você pode incluir uma consulta com atribuições direcionando o pacote de acesso e `$expand=accessPackage,target&$filter=accessPackage/id eq '9bbe5f7d-f1e7-4eb1-a586-38cdf6f8b1ea' and target/objectid eq '7deff43e-1f17-44ef-9e5f-d516b0ba11d4'`a ID do objeto desse usuário.</span><span class="sxs-lookup"><span data-stu-id="a9429-123">To retrieve only assignments for a particular user and a particular access package, you can include a query with assignments targeting that access package and the object ID of that user `$expand=accessPackage,target&$filter=accessPackage/id eq '9bbe5f7d-f1e7-4eb1-a586-38cdf6f8b1ea' and target/objectid eq '7deff43e-1f17-44ef-9e5f-d516b0ba11d4'`.</span></span>

<span data-ttu-id="a9429-124">Para obter informações gerais, confira [parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="a9429-124">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="a9429-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a9429-125">Request headers</span></span>

| <span data-ttu-id="a9429-126">Nome</span><span class="sxs-lookup"><span data-stu-id="a9429-126">Name</span></span>      |<span data-ttu-id="a9429-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="a9429-127">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="a9429-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="a9429-128">Authorization</span></span> | <span data-ttu-id="a9429-129">\{token\} de portador.</span><span class="sxs-lookup"><span data-stu-id="a9429-129">Bearer \{token\}.</span></span> <span data-ttu-id="a9429-130">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a9429-130">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a9429-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a9429-131">Request body</span></span>

<span data-ttu-id="a9429-132">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a9429-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a9429-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="a9429-133">Response</span></span>

<span data-ttu-id="a9429-134">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [accessPackageAssignment](../resources/accesspackageassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a9429-134">If successful, this method returns a `200 OK` response code and a collection of [accessPackageAssignment](../resources/accesspackageassignment.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a9429-135">Exemplos</span><span class="sxs-lookup"><span data-stu-id="a9429-135">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a9429-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a9429-136">Request</span></span>

<span data-ttu-id="a9429-137">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="a9429-137">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a9429-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="a9429-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accesspackageassignments"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignments
```
# <a name="c"></a>[<span data-ttu-id="a9429-139">C#</span><span class="sxs-lookup"><span data-stu-id="a9429-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accesspackageassignments-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a9429-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a9429-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accesspackageassignments-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a9429-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a9429-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accesspackageassignments-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="a9429-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="a9429-142">Response</span></span>

<span data-ttu-id="a9429-143">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="a9429-143">The following is an example of the response.</span></span>

> <span data-ttu-id="a9429-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a9429-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
