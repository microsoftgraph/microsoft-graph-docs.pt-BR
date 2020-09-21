---
title: Listar se aplica
description: Obtenha uma lista de objetos directoryobject aos quais um objeto homeRealmDiscoveryPolicy foi aplicado.
localization_priority: Normal
author: hpsin
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 8f1973e90283b00175b013b7658bc2b2278845a8
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47973313"
---
# <a name="list-appliesto"></a><span data-ttu-id="19a4b-103">Listar se aplica</span><span class="sxs-lookup"><span data-stu-id="19a4b-103">List appliesTo</span></span>

<span data-ttu-id="19a4b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="19a4b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="19a4b-105">Obtenha uma lista de objetos [directoryobject](../resources/directoryObject.md) aos quais um objeto [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) foi aplicado.</span><span class="sxs-lookup"><span data-stu-id="19a4b-105">Get a list of [directoryObject](../resources/directoryObject.md) objects that a [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) object has been applied to.</span></span>

## <a name="permissions"></a><span data-ttu-id="19a4b-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="19a4b-106">Permissions</span></span>

<span data-ttu-id="19a4b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="19a4b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="19a4b-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="19a4b-109">Permission type</span></span>                        | <span data-ttu-id="19a4b-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="19a4b-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="19a4b-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="19a4b-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="19a4b-112">Policy. Read. All e Application. Read. All, Policy. ReadWrite. ApplicationConfiguration e Application. Read. All, Directory. Read. All</span><span class="sxs-lookup"><span data-stu-id="19a4b-112">Policy.Read.All and Application.Read.All, Policy.ReadWrite.ApplicationConfiguration and Application.Read.All, Directory.Read.All</span></span> |
| <span data-ttu-id="19a4b-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="19a4b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="19a4b-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="19a4b-114">Not supported.</span></span> |
| <span data-ttu-id="19a4b-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="19a4b-115">Application</span></span>                            | <span data-ttu-id="19a4b-116">Policy. Read. All e Application. Read. All, Policy. ReadWrite. ApplicationConfiguration e Application. Read. All, Directory. Read. All</span><span class="sxs-lookup"><span data-stu-id="19a4b-116">Policy.Read.All and Application.Read.All, Policy.ReadWrite.ApplicationConfiguration and Application.Read.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="19a4b-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="19a4b-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /policies/homeRealmDiscoveryPolicies/{id}/appliesTo
```

## <a name="optional-query-parameters"></a><span data-ttu-id="19a4b-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="19a4b-118">Optional query parameters</span></span>

<span data-ttu-id="19a4b-119">Este método oferece suporte `$select` aos `$top` parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="19a4b-119">This method supports the `$select` and `$top` OData query parameters to help customize the response.</span></span> <span data-ttu-id="19a4b-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="19a4b-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="19a4b-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="19a4b-121">Request headers</span></span>

| <span data-ttu-id="19a4b-122">Nome</span><span class="sxs-lookup"><span data-stu-id="19a4b-122">Name</span></span>      |<span data-ttu-id="19a4b-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="19a4b-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="19a4b-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="19a4b-124">Authorization</span></span> | <span data-ttu-id="19a4b-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="19a4b-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="19a4b-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="19a4b-127">Request body</span></span>

<span data-ttu-id="19a4b-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="19a4b-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="19a4b-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="19a4b-129">Response</span></span>

<span data-ttu-id="19a4b-130">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="19a4b-130">If successful, this method returns a `200 OK` response code and a collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="19a4b-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="19a4b-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="19a4b-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="19a4b-132">Request</span></span>

<span data-ttu-id="19a4b-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="19a4b-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_appliesto"
}-->

```http
GET https://graph.microsoft.com/v1.0/homeRealmDiscoveryPolicies/{id}/appliesTo
```

### <a name="response"></a><span data-ttu-id="19a4b-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="19a4b-134">Response</span></span>

<span data-ttu-id="19a4b-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="19a4b-135">The following is an example of the response.</span></span>

> <span data-ttu-id="19a4b-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="19a4b-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
      "id": "id-value",
      "deletedDateTime": "datetime-value"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List appliesTo",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
