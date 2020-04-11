---
title: Lista atribuída tokenIssuancePolicies
description: Listar tokenIssuancePolicies atribuídos a um aplicativo.
localization_priority: Normal
author: sureshja
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 3e116d5938ebc8575b4c4664156e6c7ab194b276
ms.sourcegitcommit: 9a6ce4ddf75beead19b7c35a1949cf4d105b9b29
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2020
ms.locfileid: "43227765"
---
# <a name="list-assigned-tokenissuancepolicies"></a><span data-ttu-id="0215a-103">Lista atribuída tokenIssuancePolicies</span><span class="sxs-lookup"><span data-stu-id="0215a-103">List assigned tokenIssuancePolicies</span></span>

<span data-ttu-id="0215a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0215a-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="0215a-105">Lista os objetos [tokenIssuancePolicy](../resources/tokenissuancepolicy.md) que são atribuídos a um [aplicativo](../resources/application.md).</span><span class="sxs-lookup"><span data-stu-id="0215a-105">List the [tokenIssuancePolicy](../resources/tokenissuancepolicy.md) objects that are assigned to an [application](../resources/application.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="0215a-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="0215a-106">Permissions</span></span>

<span data-ttu-id="0215a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0215a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0215a-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0215a-109">Permission type</span></span>                        | <span data-ttu-id="0215a-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0215a-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="0215a-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0215a-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="0215a-112">Policy. Read. All e Application. ReadWrite. All, Policy. ReadWrite. ApplicationConfiguration e Application. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="0215a-112">Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |
| <span data-ttu-id="0215a-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0215a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0215a-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0215a-114">Not supported.</span></span> |
| <span data-ttu-id="0215a-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0215a-115">Application</span></span>                            | <span data-ttu-id="0215a-116">Policy. Read. All e Application. ReadWrite. OwnedBy, Policy. Read. All e Application. ReadWrite. All, Policy. ReadWrite. ApplicationConfiguration e Application. ReadWrite. OwnedBy, Policy. ReadWrite. ApplicationConfiguration e Application. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="0215a-116">Policy.Read.All and Application.ReadWrite.OwnedBy, Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.OwnedBy, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0215a-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0215a-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /applications/{id}/tokenIssuancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="0215a-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0215a-118">Request headers</span></span>

| <span data-ttu-id="0215a-119">Nome</span><span class="sxs-lookup"><span data-stu-id="0215a-119">Name</span></span>          | <span data-ttu-id="0215a-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="0215a-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="0215a-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="0215a-121">Authorization</span></span> | <span data-ttu-id="0215a-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0215a-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0215a-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0215a-124">Request body</span></span>

<span data-ttu-id="0215a-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="0215a-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0215a-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="0215a-126">Response</span></span>

<span data-ttu-id="0215a-127">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [tokenIssuancePolicy](../resources/tokenissuancepolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0215a-127">If successful, this method returns a `200 OK` response code and a collection of [tokenIssuancePolicy](../resources/tokenissuancepolicy.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="0215a-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="0215a-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="0215a-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0215a-129">Request</span></span>

<span data-ttu-id="0215a-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="0215a-130">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "list_tokenissuancepolicies_on_application"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/applications/{id}/tokenIssuancePolicies
```

### <a name="response"></a><span data-ttu-id="0215a-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="0215a-131">Response</span></span>

<span data-ttu-id="0215a-132">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="0215a-132">The following is an example of the response.</span></span>

> <span data-ttu-id="0215a-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0215a-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.tokenIssuancePolicy",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "definition": [
        "definition-value"
      ],
      "displayName": "displayName-value",
      "isOrganizationDefault": true,
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List assigned tokenIssuancePolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
