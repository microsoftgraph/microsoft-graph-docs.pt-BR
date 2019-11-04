---
title: Listar accessPackageAssignmentRequests
description: Recupere uma lista de objetos accessPackageAssignmentRequest.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: d97b0f7c3f06652a7d22d0b803d471b95a233e62
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37935045"
---
# <a name="list-accesspackageassignmentrequests"></a><span data-ttu-id="9cbe1-103">Listar accessPackageAssignmentRequests</span><span class="sxs-lookup"><span data-stu-id="9cbe1-103">List accessPackageAssignmentRequests</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9cbe1-104">No [Gerenciamento de direitos do Azure ad](../resources/entitlementmanagement-root.md), recupere uma lista de objetos [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) .</span><span class="sxs-lookup"><span data-stu-id="9cbe1-104">In [Azure AD entitlement management](../resources/entitlementmanagement-root.md), retrieve a list of [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) objects.</span></span>  <span data-ttu-id="9cbe1-105">A lista resultante inclui todas as solicitações de atribuição, atuais e bem como expiradas, que o chamador tem acesso para leitura, entre todos os catálogos e pacotes de acesso.</span><span class="sxs-lookup"><span data-stu-id="9cbe1-105">The resulting list includes all the assignment requests, current and well as expired, that the caller has access to read, across all catalogs and access packages.</span></span>

## <a name="permissions"></a><span data-ttu-id="9cbe1-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="9cbe1-106">Permissions</span></span>

<span data-ttu-id="9cbe1-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9cbe1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="9cbe1-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9cbe1-109">Permission type</span></span>                        | <span data-ttu-id="9cbe1-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9cbe1-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="9cbe1-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9cbe1-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="9cbe1-112">EntitlementManagement. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="9cbe1-112">EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="9cbe1-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9cbe1-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9cbe1-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9cbe1-114">Not supported.</span></span> |
| <span data-ttu-id="9cbe1-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9cbe1-115">Application</span></span>                            | <span data-ttu-id="9cbe1-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9cbe1-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9cbe1-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9cbe1-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityGovernance/entitlementManagement/accessPackageAssignmentRequests
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9cbe1-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="9cbe1-118">Optional query parameters</span></span>

<span data-ttu-id="9cbe1-119">Este método oferece suporte a alguns dos parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="9cbe1-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="9cbe1-120">Por exemplo, para recuperar o pacote de acesso de cada solicitação, `$expand=accessPackage` inclua na consulta.</span><span class="sxs-lookup"><span data-stu-id="9cbe1-120">For example, to retrieve the access package of each request, include `$expand=accessPackage` in the query.</span></span>  <span data-ttu-id="9cbe1-121">Para obter informações gerais, confira [parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="9cbe1-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="9cbe1-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9cbe1-122">Request headers</span></span>

| <span data-ttu-id="9cbe1-123">Nome</span><span class="sxs-lookup"><span data-stu-id="9cbe1-123">Name</span></span>      |<span data-ttu-id="9cbe1-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="9cbe1-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="9cbe1-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="9cbe1-125">Authorization</span></span> | <span data-ttu-id="9cbe1-126">\{token\} de portador.</span><span class="sxs-lookup"><span data-stu-id="9cbe1-126">Bearer \{token\}.</span></span> <span data-ttu-id="9cbe1-127">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9cbe1-127">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9cbe1-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9cbe1-128">Request body</span></span>

<span data-ttu-id="9cbe1-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="9cbe1-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9cbe1-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="9cbe1-130">Response</span></span>

<span data-ttu-id="9cbe1-131">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9cbe1-131">If successful, this method returns a `200 OK` response code and a collection of [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="9cbe1-132">Exemplos</span><span class="sxs-lookup"><span data-stu-id="9cbe1-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="9cbe1-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9cbe1-133">Request</span></span>

<span data-ttu-id="9cbe1-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="9cbe1-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_accesspackageassignmentrequests"
}-->

```http
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignmentRequests
```

### <a name="response"></a><span data-ttu-id="9cbe1-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="9cbe1-135">Response</span></span>

<span data-ttu-id="9cbe1-136">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="9cbe1-136">The following is an example of the response.</span></span>

> <span data-ttu-id="9cbe1-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9cbe1-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessPackageAssignmentRequest",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "433dafca-5047-4614-95f7-a03510b1ded3",
      "requestType": "AdminAdd",
      "requestState": "Delivered",
      "requestStatus": "Fulfilled",
      "isValidationOnly": false,
      "createdDateTime": "2019-10-25T22:55:11.623Z"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List accessPackageAssignmentRequests",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
