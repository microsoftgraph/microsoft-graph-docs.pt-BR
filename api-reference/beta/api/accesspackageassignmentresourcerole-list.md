---
title: Listar accessPackageAssignmentResourceRoles
description: Recupere uma lista de objetos accessPackageAssignmentResourceRrole.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 16d2e91b00832b4745682861573985cc5bde27fb
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37935038"
---
# <a name="list-accesspackageassignmentresourceroles"></a><span data-ttu-id="5c1e9-103">Listar accessPackageAssignmentResourceRoles</span><span class="sxs-lookup"><span data-stu-id="5c1e9-103">List accessPackageAssignmentResourceRoles</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5c1e9-104">Recupere uma lista de objetos [accessPackageAssignmentResourceRole](../resources/accesspackageassignmentresourcerole.md) .</span><span class="sxs-lookup"><span data-stu-id="5c1e9-104">Retrieve a list of [accessPackageAssignmentResourceRole](../resources/accesspackageassignmentresourcerole.md) objects.</span></span>  <span data-ttu-id="5c1e9-105">A lista resultante inclui todas as funções de recurso de todas as atribuições que o chamador tem acesso para ler, entre todos os catálogos e pacotes de acesso.</span><span class="sxs-lookup"><span data-stu-id="5c1e9-105">The resulting list includes all the resource roles of all assignments that the caller has access to read, across all catalogs and access packages.</span></span>

## <a name="permissions"></a><span data-ttu-id="5c1e9-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="5c1e9-106">Permissions</span></span>

<span data-ttu-id="5c1e9-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5c1e9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5c1e9-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5c1e9-109">Permission type</span></span>                        | <span data-ttu-id="5c1e9-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5c1e9-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="5c1e9-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5c1e9-111">Delegated (work or school account)</span></span>     |  <span data-ttu-id="5c1e9-112">EntitlementManagement. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="5c1e9-112">EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="5c1e9-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5c1e9-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5c1e9-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5c1e9-114">Not supported.</span></span> |
| <span data-ttu-id="5c1e9-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5c1e9-115">Application</span></span>                            | <span data-ttu-id="5c1e9-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5c1e9-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5c1e9-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5c1e9-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityGovernance/entitlementManagement/accessPackageAssignmentResourceRoles
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5c1e9-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="5c1e9-118">Optional query parameters</span></span>

<span data-ttu-id="5c1e9-119">Este método oferece suporte a alguns dos parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="5c1e9-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="5c1e9-120">Para obter informações gerais, confira [parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="5c1e9-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="5c1e9-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5c1e9-121">Request headers</span></span>

| <span data-ttu-id="5c1e9-122">Nome</span><span class="sxs-lookup"><span data-stu-id="5c1e9-122">Name</span></span>      |<span data-ttu-id="5c1e9-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="5c1e9-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="5c1e9-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="5c1e9-124">Authorization</span></span> | <span data-ttu-id="5c1e9-125">\{token\} de portador.</span><span class="sxs-lookup"><span data-stu-id="5c1e9-125">Bearer \{token\}.</span></span> <span data-ttu-id="5c1e9-126">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5c1e9-126">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5c1e9-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5c1e9-127">Request body</span></span>

<span data-ttu-id="5c1e9-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5c1e9-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5c1e9-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="5c1e9-129">Response</span></span>

<span data-ttu-id="5c1e9-130">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [accessPackageAssignmentResourceRole](../resources/accesspackageassignmentresourcerole.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5c1e9-130">If successful, this method returns a `200 OK` response code and a collection of [accessPackageAssignmentResourceRole](../resources/accesspackageassignmentresourcerole.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="5c1e9-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="5c1e9-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="5c1e9-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5c1e9-132">Request</span></span>

<span data-ttu-id="5c1e9-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="5c1e9-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_accesspackageassignmentresourceroles"
}-->

```http
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignmentResourceRoles
```

### <a name="response"></a><span data-ttu-id="5c1e9-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="5c1e9-134">Response</span></span>

<span data-ttu-id="5c1e9-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="5c1e9-135">The following is an example of the response.</span></span>

> <span data-ttu-id="5c1e9-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5c1e9-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessPackageAssignmentResourceRole",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "1bf101d2-4d9c-437f-bbf5-3d13d98f5479",
      "originId": "originId-value",
      "originSystem": "SharePointOnline",
      "status": "Fulfilled"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List accessPackageAssignmentResourceRoles",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
