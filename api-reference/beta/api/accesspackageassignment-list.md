---
title: Listar accessPackageAssignments
description: Recupere uma lista de objetos accesspackageassignment.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 605bc5bdfcafbf4c7aaae9903530bc5d067c748f
ms.sourcegitcommit: 744c2d8be5a1ce158068bcfeaad1aabf8166c556
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/22/2021
ms.locfileid: "49934531"
---
# <a name="list-accesspackageassignments"></a><span data-ttu-id="a67c1-103">Listar accessPackageAssignments</span><span class="sxs-lookup"><span data-stu-id="a67c1-103">List accessPackageAssignments</span></span>

<span data-ttu-id="a67c1-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a67c1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a67c1-105">No gerenciamento de direitos do [Azure AD,](../resources/entitlementmanagement-root.md)recupere uma lista de [objetos accessPackageAssignment.](../resources/accesspackageassignment.md)</span><span class="sxs-lookup"><span data-stu-id="a67c1-105">In [Azure AD entitlement management](../resources/entitlementmanagement-root.md), retrieve a list of [accessPackageAssignment](../resources/accesspackageassignment.md) objects.</span></span> <span data-ttu-id="a67c1-106">Para administradores de todo o diretório, a lista resultante inclui todas as atribuições, atuais e bem expiradas, que o chamador tem acesso para ler em todos os catálogos e pacotes de acesso.</span><span class="sxs-lookup"><span data-stu-id="a67c1-106">For directory-wide administrators, the resulting list includes all the assignments, current and well as expired, that the caller has access to read, across all catalogs and access packages.</span></span>  <span data-ttu-id="a67c1-107">Se o chamador estiver em nome de um usuário delegado que está atribuído apenas a funções administrativas delegadas específicas do catálogo, a solicitação deverá fornecer um filtro para indicar um pacote de acesso específico, como: `$filter=accessPackage/id eq 'a914b616-e04e-476b-aa37-91038f0b165b'` .</span><span class="sxs-lookup"><span data-stu-id="a67c1-107">If the caller is on behalf of a delegated user who is assigned only to catalog-specific delegated administrative roles, the request must supply a filter to indicate a specific access package, such as: `$filter=accessPackage/id eq 'a914b616-e04e-476b-aa37-91038f0b165b'`.</span></span>


## <a name="permissions"></a><span data-ttu-id="a67c1-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="a67c1-108">Permissions</span></span>

<span data-ttu-id="a67c1-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a67c1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a67c1-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a67c1-111">Permission type</span></span>                        | <span data-ttu-id="a67c1-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a67c1-112">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="a67c1-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a67c1-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="a67c1-114">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a67c1-114">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="a67c1-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a67c1-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a67c1-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a67c1-116">Not supported.</span></span> |
| <span data-ttu-id="a67c1-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a67c1-117">Application</span></span>                            | <span data-ttu-id="a67c1-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a67c1-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a67c1-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a67c1-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityGovernance/entitlementManagement/accessPackageAssignments
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a67c1-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="a67c1-120">Optional query parameters</span></span>

<span data-ttu-id="a67c1-121">Se o chamador estiver em nome de um usuário delegado que está atribuído apenas a funções administrativas delegadas específicas do catálogo, a solicitação deverá fornecer um filtro para indicar um pacote de acesso específico, como: `$filter=accessPackage/id eq 'a914b616-e04e-476b-aa37-91038f0b165b'` .</span><span class="sxs-lookup"><span data-stu-id="a67c1-121">If the caller is on behalf of a delegated user who is assigned only to catalog-specific delegated administrative roles, the request must supply a filter to indicate a specific access package, such as: `$filter=accessPackage/id eq 'a914b616-e04e-476b-aa37-91038f0b165b'`.</span></span>  <span data-ttu-id="a67c1-122">Esse método também dá suporte a alguns dos parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="a67c1-122">This method also supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="a67c1-123">Por exemplo, para também retornar o assunto de destino e o pacote de acesso, inclua `$expand=target,accessPackage` .</span><span class="sxs-lookup"><span data-stu-id="a67c1-123">For example, to also return the target subject and access package, include `$expand=target,accessPackage`.</span></span> <span data-ttu-id="a67c1-124">Para recuperar apenas atribuições entregues, você pode incluir uma `$filter=assignmentState eq 'Delivered'` consulta.</span><span class="sxs-lookup"><span data-stu-id="a67c1-124">To retrieve only delivered assignments, you can include a query `$filter=assignmentState eq 'Delivered'`.</span></span> <span data-ttu-id="a67c1-125">Para recuperar apenas atribuições para um usuário específico, você pode incluir uma consulta com atribuições direcionando a ID de objeto desse usuário: `$expand=target&$filter=target/objectid+eq+'7deff43e-1f17-44ef-9e5f-d516b0ba11d4'` .</span><span class="sxs-lookup"><span data-stu-id="a67c1-125">To retrieve only assignments for a particular user, you can include a query with assignments targeting the object ID of that user: `$expand=target&$filter=target/objectid+eq+'7deff43e-1f17-44ef-9e5f-d516b0ba11d4'`.</span></span>  <span data-ttu-id="a67c1-126">Para recuperar apenas atribuições para um usuário específico e um pacote de acesso específico, você pode incluir uma consulta com atribuições segmentando esse pacote de acesso e a ID de objeto desse usuário: `$expand=accessPackage,target&$filter=accessPackage/id eq '9bbe5f7d-f1e7-4eb1-a586-38cdf6f8b1ea' and target/objectid eq '7deff43e-1f17-44ef-9e5f-d516b0ba11d4'` .</span><span class="sxs-lookup"><span data-stu-id="a67c1-126">To retrieve only assignments for a particular user and a particular access package, you can include a query with assignments targeting that access package and the object ID of that user: `$expand=accessPackage,target&$filter=accessPackage/id eq '9bbe5f7d-f1e7-4eb1-a586-38cdf6f8b1ea' and target/objectid eq '7deff43e-1f17-44ef-9e5f-d516b0ba11d4'`.</span></span>  <span data-ttu-id="a67c1-127">Para recuperar apenas atribuições resultantes de uma diretiva de atribuição de pacote de acesso específica, você pode incluir uma consulta para essa política: `$filter=accessPackageAssignmentPolicy/id eq 'd92ebb54-9b46-492d-ab7f-01f76767da7f'` .</span><span class="sxs-lookup"><span data-stu-id="a67c1-127">To retrieve only assignments resulting from a particular access package assignment policy, you can include a query for that policy: `$filter=accessPackageAssignmentPolicy/id eq 'd92ebb54-9b46-492d-ab7f-01f76767da7f'`.</span></span>

<span data-ttu-id="a67c1-128">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="a67c1-128">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="a67c1-129">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a67c1-129">Request headers</span></span>

| <span data-ttu-id="a67c1-130">Nome</span><span class="sxs-lookup"><span data-stu-id="a67c1-130">Name</span></span>      |<span data-ttu-id="a67c1-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="a67c1-131">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="a67c1-132">Autorização</span><span class="sxs-lookup"><span data-stu-id="a67c1-132">Authorization</span></span> | <span data-ttu-id="a67c1-133">\{token\} de portador.</span><span class="sxs-lookup"><span data-stu-id="a67c1-133">Bearer \{token\}.</span></span> <span data-ttu-id="a67c1-134">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a67c1-134">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a67c1-135">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a67c1-135">Request body</span></span>

<span data-ttu-id="a67c1-136">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a67c1-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a67c1-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="a67c1-137">Response</span></span>

<span data-ttu-id="a67c1-138">Se bem-sucedido, este método retorna um código de resposta e uma coleção de `200 OK` [objetos accessPackageAssignment](../resources/accesspackageassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a67c1-138">If successful, this method returns a `200 OK` response code and a collection of [accessPackageAssignment](../resources/accesspackageassignment.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a67c1-139">Exemplos</span><span class="sxs-lookup"><span data-stu-id="a67c1-139">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a67c1-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a67c1-140">Request</span></span>

<span data-ttu-id="a67c1-141">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="a67c1-141">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a67c1-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="a67c1-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accesspackageassignments"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignments
```
# <a name="c"></a>[<span data-ttu-id="a67c1-143">C#</span><span class="sxs-lookup"><span data-stu-id="a67c1-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accesspackageassignments-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a67c1-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a67c1-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accesspackageassignments-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a67c1-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a67c1-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accesspackageassignments-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a67c1-146">Java</span><span class="sxs-lookup"><span data-stu-id="a67c1-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-accesspackageassignments-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="a67c1-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="a67c1-147">Response</span></span>

<span data-ttu-id="a67c1-148">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="a67c1-148">The following is an example of the response.</span></span>

> <span data-ttu-id="a67c1-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a67c1-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


