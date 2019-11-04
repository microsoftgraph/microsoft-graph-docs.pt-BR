---
title: Obter accessPackageAssignmentRequest
description: Recupere as propriedades e os relacionamentos de um objeto accessPackageAssignmentRequest.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 5768664edbdce00b8004ee9031520fdcc9331ef3
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37935046"
---
# <a name="get-accesspackageassignmentrequest"></a><span data-ttu-id="a29a4-103">Obter accessPackageAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="a29a4-103">Get accessPackageAssignmentRequest</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a29a4-104">No [Azure ad pretitulation Management](../resources/entitlementmanagement-root.md), recupere as propriedades e os relacionamentos de um objeto [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) .</span><span class="sxs-lookup"><span data-stu-id="a29a4-104">In [Azure AD entitlement management](../resources/entitlementmanagement-root.md), retrieve the properties and relationships of an  [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="a29a4-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="a29a4-105">Permissions</span></span>

<span data-ttu-id="a29a4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a29a4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a29a4-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a29a4-108">Permission type</span></span>                        | <span data-ttu-id="a29a4-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a29a4-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="a29a4-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a29a4-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="a29a4-111">EntitlementManagement. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="a29a4-111">EntitlementManagement.ReadWrite.All</span></span>  |
| <span data-ttu-id="a29a4-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a29a4-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a29a4-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a29a4-113">Not supported.</span></span> |
| <span data-ttu-id="a29a4-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a29a4-114">Application</span></span>                            | <span data-ttu-id="a29a4-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a29a4-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a29a4-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a29a4-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityGovernance/entitlementManagement/accessPackageAssignmentRequests/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a29a4-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="a29a4-117">Optional query parameters</span></span>

<span data-ttu-id="a29a4-118">Este método oferece suporte a alguns dos parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="a29a4-118">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="a29a4-119">Por exemplo, para recuperar o pacote do Access que foi solicitado, `$expand=accessPackage` inclua na consulta.</span><span class="sxs-lookup"><span data-stu-id="a29a4-119">For example, to retrieve the access package that was requested, include `$expand=accessPackage` in the query.</span></span> <span data-ttu-id="a29a4-120">Para obter informações gerais, confira [parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="a29a4-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="a29a4-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a29a4-121">Request headers</span></span>

| <span data-ttu-id="a29a4-122">Nome</span><span class="sxs-lookup"><span data-stu-id="a29a4-122">Name</span></span>      |<span data-ttu-id="a29a4-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="a29a4-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="a29a4-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="a29a4-124">Authorization</span></span> | <span data-ttu-id="a29a4-125">\{token\} de portador.</span><span class="sxs-lookup"><span data-stu-id="a29a4-125">Bearer \{token\}.</span></span> <span data-ttu-id="a29a4-126">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a29a4-126">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a29a4-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a29a4-127">Request body</span></span>

<span data-ttu-id="a29a4-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a29a4-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a29a4-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="a29a4-129">Response</span></span>

<span data-ttu-id="a29a4-130">Se tiver êxito, este método retornará `200 OK` um código de resposta e o objeto [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a29a4-130">If successful, this method returns a `200 OK` response code and the requested [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a29a4-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="a29a4-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a29a4-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a29a4-132">Request</span></span>

<span data-ttu-id="a29a4-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="a29a4-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_accesspackageassignmentrequest"
}-->

```http
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignmentRequests/{id}
```

### <a name="response"></a><span data-ttu-id="a29a4-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="a29a4-134">Response</span></span>

<span data-ttu-id="a29a4-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="a29a4-135">The following is an example of the response.</span></span>

> <span data-ttu-id="a29a4-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a29a4-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessPackageAssignmentRequest"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "433dafca-5047-4614-95f7-a03510b1ded3",
  "requestType": "AdminAdd",
  "requestState": "Delivered",
  "requestStatus": "Fulfilled",
  "isValidationOnly": false,
  "createdDateTime": "2019-10-25T22:55:11.623Z"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get accessPackageAssignmentRequest",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
