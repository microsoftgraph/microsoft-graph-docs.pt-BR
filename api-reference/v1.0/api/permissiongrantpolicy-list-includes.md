---
title: List inclui coleção de permissionGrantPolicy
description: Recupere uma lista dos conjuntos de condição que descrevem as condições sob as quais um evento de concessão de permissão está incluído em uma política de concessão de permissão.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: psignoret
ms.openlocfilehash: e85fdb159f275eb1dc4a7a31604b7d51e698288f
ms.sourcegitcommit: 6201b3a5646f640f25a68ab033eca9eb60ccd05e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/21/2020
ms.locfileid: "49377118"
---
# <a name="list-includes-collection-of-permissiongrantpolicy"></a><span data-ttu-id="9f542-103">List inclui coleção de permissionGrantPolicy</span><span class="sxs-lookup"><span data-stu-id="9f542-103">List includes collection of permissionGrantPolicy</span></span>

<span data-ttu-id="9f542-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9f542-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="9f542-105">Recupere os conjuntos de condições que estão *incluídos* em um [permissionGrantPolicy](../resources/permissiongrantpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="9f542-105">Retrieve the condition sets which are *included* in a [permissionGrantPolicy](../resources/permissiongrantpolicy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="9f542-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="9f542-106">Permissions</span></span>

<span data-ttu-id="9f542-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9f542-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9f542-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9f542-109">Permission type</span></span>      | <span data-ttu-id="9f542-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9f542-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9f542-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9f542-111">Delegated (work or school account)</span></span> | <span data-ttu-id="9f542-112">Policy. Read. PermissionGrant, Directory. Read. All</span><span class="sxs-lookup"><span data-stu-id="9f542-112">Policy.Read.PermissionGrant, Directory.Read.All</span></span> |
|<span data-ttu-id="9f542-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9f542-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9f542-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9f542-114">Not supported.</span></span>    |
|<span data-ttu-id="9f542-115">Application</span><span class="sxs-lookup"><span data-stu-id="9f542-115">Application</span></span> | <span data-ttu-id="9f542-116">Policy. Read. PermissionGrant, Directory. Read. All</span><span class="sxs-lookup"><span data-stu-id="9f542-116">Policy.Read.PermissionGrant, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9f542-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9f542-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /policies/permissionGrantPolicies/{id}/includes
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9f542-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="9f542-118">Optional query parameters</span></span>

<span data-ttu-id="9f542-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="9f542-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9f542-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9f542-120">Request headers</span></span>

| <span data-ttu-id="9f542-121">Nome</span><span class="sxs-lookup"><span data-stu-id="9f542-121">Name</span></span>           | <span data-ttu-id="9f542-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="9f542-122">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="9f542-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="9f542-123">Authorization</span></span>  | <span data-ttu-id="9f542-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9f542-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="9f542-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9f542-126">Request body</span></span>

<span data-ttu-id="9f542-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="9f542-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9f542-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="9f542-128">Response</span></span>

<span data-ttu-id="9f542-129">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [permissionGrantConditionSet](../resources/permissiongrantconditionset.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9f542-129">If successful, this method returns a `200 OK` response code and a collection of [permissionGrantConditionSet](../resources/permissiongrantconditionset.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9f542-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9f542-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="9f542-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9f542-131">Request</span></span>

<span data-ttu-id="9f542-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="9f542-132">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "permissiongrantpolicy_get_includes"
}-->

```http
GET https://graph.microsoft.com/v1.0/policies/permissionGrantPolicies/microsoft-application-admin/includes
```

### <a name="response"></a><span data-ttu-id="9f542-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="9f542-133">Response</span></span>

<span data-ttu-id="9f542-134">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="9f542-134">The following is an example of the response.</span></span>

> <span data-ttu-id="9f542-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9f542-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.permissionGrantConditionSet",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "811d2da7-443c-43da-96e7-28d285b234e9",
      "permissionClassification": "all",
      "permissionType": "application",
      "resourceApplication": "any",
      "permissions": [ "all" ],
      "clientApplicationIds": [ "all" ],
      "clientApplicationTenantIds": [ "all" ],
      "clientApplicationPublisherIds": [ "all" ],
      "clientApplicationsFromVerifiedPublisherOnly": false
    },
    {
      "id": "60461179-740e-4d8b-9e00-1456a338c44b",
      "permissionClassification": "all",
      "permissionType": "delegated",
      "resourceApplication": "any",
      "permissions": [ "all" ],
      "clientApplicationIds": [ "all" ],
      "clientApplicationTenantIds": [ "all" ],
      "clientApplicationPublisherIds": [ "all" ],
      "clientApplicationsFromVerifiedPublisherOnly": false
    }
  ]
}
```
