---
title: Listar transitiveMemberOf
description: Obter grupos dos quais o contato do organziational é membro. Essa solicitação de API é transitiva e também retorna todos os grupos dos quais o usuário é um membro aninhado.
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 2387bf17583869f8b5a043d0a8318a424f37af15
ms.sourcegitcommit: d9457ac1b8c2e8ac4b9604dd9e116fd547d2bfbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/29/2020
ms.locfileid: "48797141"
---
# <a name="list-transitivememberof"></a><span data-ttu-id="f4010-104">Listar transitiveMemberOf</span><span class="sxs-lookup"><span data-stu-id="f4010-104">List transitiveMemberOf</span></span>

<span data-ttu-id="f4010-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f4010-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f4010-106">Obter grupos dos quais esse [contato organizacional](../resources/orgcontact.md) é membro.</span><span class="sxs-lookup"><span data-stu-id="f4010-106">Get groups that this [organizational contact](../resources/orgcontact.md) is a member of.</span></span> <span data-ttu-id="f4010-107">A solicitação de API é transitiva e retorna todos os grupos dos quais o contato organizacional é um membro aninhado.</span><span class="sxs-lookup"><span data-stu-id="f4010-107">The API request is transitive, and returns all groups the organizational contact is a nested member of.</span></span>

## <a name="permissions"></a><span data-ttu-id="f4010-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="f4010-108">Permissions</span></span>

<span data-ttu-id="f4010-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f4010-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f4010-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f4010-111">Permission type</span></span>      | <span data-ttu-id="f4010-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f4010-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f4010-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f4010-113">Delegated (work or school account)</span></span> | <span data-ttu-id="f4010-114">OrgContact. Read. All e Group. Read. All, Directory. Read. All</span><span class="sxs-lookup"><span data-stu-id="f4010-114">OrgContact.Read.All and Group.Read.All, Directory.Read.All</span></span>  |
|<span data-ttu-id="f4010-115">Delegada (conta Microsoft pessoal)</span><span class="sxs-lookup"><span data-stu-id="f4010-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f4010-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f4010-116">Not supported.</span></span>    |
|<span data-ttu-id="f4010-117">Application</span><span class="sxs-lookup"><span data-stu-id="f4010-117">Application</span></span> | <span data-ttu-id="f4010-118">OrgContact. Read. All e Group. Read. All, Directory. Read. All</span><span class="sxs-lookup"><span data-stu-id="f4010-118">OrgContact.Read.All and Group.Read.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f4010-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f4010-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /contacts/{id}/transitiveMemberOf
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f4010-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="f4010-120">Optional query parameters</span></span>

<span data-ttu-id="f4010-121">Este método dá suporte a `$select` [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="f4010-121">This method supports the `$select` [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f4010-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f4010-122">Request headers</span></span>

| <span data-ttu-id="f4010-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f4010-123">Header</span></span>       | <span data-ttu-id="f4010-124">Valor</span><span class="sxs-lookup"><span data-stu-id="f4010-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="f4010-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="f4010-125">Authorization</span></span>  | <span data-ttu-id="f4010-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f4010-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="f4010-128">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f4010-128">Accept</span></span>  | <span data-ttu-id="f4010-129">application/json</span><span class="sxs-lookup"><span data-stu-id="f4010-129">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f4010-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f4010-130">Request body</span></span>

<span data-ttu-id="f4010-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f4010-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f4010-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="f4010-132">Response</span></span>

<span data-ttu-id="f4010-133">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f4010-133">If successful, this method returns a `200 OK` response code and a collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f4010-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f4010-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="f4010-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f4010-135">Request</span></span>

<span data-ttu-id="f4010-136">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="f4010-136">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "orgcontact_list_transitivememberof"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/{id}/transitiveMemberOf
```

### <a name="response"></a><span data-ttu-id="f4010-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="f4010-137">Response</span></span>

<span data-ttu-id="f4010-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="f4010-138">The following is an example of the response.</span></span>
><span data-ttu-id="f4010-139">**Observação** : o objeto de resposta mostrado aqui pode ser encurtado com fins de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="f4010-139">**Note** : The response object shown here might be shortened for readability.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.group",
      "id": "id-value",
      "createdDateTime": null,
      "description": "All users at the company",
      "displayName": "All Users",
      "groupTypes": [],
      "mailEnabled": false,
      "securityEnabled": true,
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List orgContact transitiveMemberOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

