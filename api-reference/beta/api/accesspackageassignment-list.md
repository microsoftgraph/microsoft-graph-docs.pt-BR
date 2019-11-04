---
title: Listar accessPackageAssignments
description: Recupere uma lista de objetos accesspackageassignment.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 8ed838b01364e5616db6ed8b2236dc0b5593d9ff
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37935054"
---
# <a name="list-accesspackageassignments"></a><span data-ttu-id="e83c2-103">Listar accessPackageAssignments</span><span class="sxs-lookup"><span data-stu-id="e83c2-103">List accessPackageAssignments</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e83c2-104">No [Gerenciamento de direitos do Azure ad](../resources/entitlementmanagement-root.md), recupere uma lista de objetos [accessPackageAssignment](../resources/accesspackageassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="e83c2-104">In [Azure AD entitlement management](../resources/entitlementmanagement-root.md), retrieve a list of [accessPackageAssignment](../resources/accesspackageassignment.md) objects.</span></span>  <span data-ttu-id="e83c2-105">A lista resultante inclui todas as atribuições, atuais e bem como expiradas, que o chamador tem acesso para leitura, entre todos os catálogos e pacotes de acesso.</span><span class="sxs-lookup"><span data-stu-id="e83c2-105">The resulting list includes all the assignments, current and well as expired, that the caller has access to read, across all catalogs and access packages.</span></span>

## <a name="permissions"></a><span data-ttu-id="e83c2-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="e83c2-106">Permissions</span></span>

<span data-ttu-id="e83c2-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e83c2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e83c2-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e83c2-109">Permission type</span></span>                        | <span data-ttu-id="e83c2-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e83c2-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="e83c2-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e83c2-111">Delegated (work or school account)</span></span>     |  <span data-ttu-id="e83c2-112">EntitlementManagement. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="e83c2-112">EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="e83c2-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e83c2-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e83c2-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e83c2-114">Not supported.</span></span> |
| <span data-ttu-id="e83c2-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e83c2-115">Application</span></span>                            | <span data-ttu-id="e83c2-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e83c2-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e83c2-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e83c2-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityGovernance/entitlementManagement/accessPackageAssignments
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e83c2-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="e83c2-118">Optional query parameters</span></span>

<span data-ttu-id="e83c2-119">Este método oferece suporte a alguns dos parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="e83c2-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="e83c2-120">Por exemplo, para recuperar apenas atribuições entregues, você pode incluir uma `$filter=assignmentState eq 'Delivered'`consulta.</span><span class="sxs-lookup"><span data-stu-id="e83c2-120">For example, to retrieve only Delivered assignments, you can include a query `$filter=assignmentState eq 'Delivered'`.</span></span>
<span data-ttu-id="e83c2-121">Para obter informações gerais, confira [parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="e83c2-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="e83c2-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e83c2-122">Request headers</span></span>

| <span data-ttu-id="e83c2-123">Nome</span><span class="sxs-lookup"><span data-stu-id="e83c2-123">Name</span></span>      |<span data-ttu-id="e83c2-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="e83c2-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="e83c2-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="e83c2-125">Authorization</span></span> | <span data-ttu-id="e83c2-126">\{token\} de portador.</span><span class="sxs-lookup"><span data-stu-id="e83c2-126">Bearer \{token\}.</span></span> <span data-ttu-id="e83c2-127">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e83c2-127">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e83c2-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e83c2-128">Request body</span></span>

<span data-ttu-id="e83c2-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e83c2-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e83c2-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="e83c2-130">Response</span></span>

<span data-ttu-id="e83c2-131">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [accessPackageAssignment](../resources/accesspackageassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e83c2-131">If successful, this method returns a `200 OK` response code and a collection of [accessPackageAssignment](../resources/accesspackageassignment.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e83c2-132">Exemplos</span><span class="sxs-lookup"><span data-stu-id="e83c2-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="e83c2-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e83c2-133">Request</span></span>

<span data-ttu-id="e83c2-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="e83c2-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_accesspackageassignments"
}-->

```http
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignments
```

### <a name="response"></a><span data-ttu-id="e83c2-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="e83c2-135">Response</span></span>

<span data-ttu-id="e83c2-136">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="e83c2-136">The following is an example of the response.</span></span>

> <span data-ttu-id="e83c2-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e83c2-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
