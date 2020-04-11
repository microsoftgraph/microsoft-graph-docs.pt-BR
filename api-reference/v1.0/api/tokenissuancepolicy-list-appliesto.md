---
title: Listar se aplica
description: Obtenha uma lista de objetos directoryobject aos quais um objeto tokenIssuancePolicy foi aplicado.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 2c2f2f47243f2f38d5cc7d183f5ac8654d0dd451
ms.sourcegitcommit: 9a6ce4ddf75beead19b7c35a1949cf4d105b9b29
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2020
ms.locfileid: "43229679"
---
# <a name="list-appliesto"></a><span data-ttu-id="4c711-103">Listar se aplica</span><span class="sxs-lookup"><span data-stu-id="4c711-103">List appliesTo</span></span>

<span data-ttu-id="4c711-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4c711-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="4c711-105">Obtenha uma lista de objetos [directoryobject](../resources/directoryObject.md) aos quais um objeto [tokenIssuancePolicy](../resources/tokenissuancepolicy.md) foi aplicado.</span><span class="sxs-lookup"><span data-stu-id="4c711-105">Get a list of [directoryObject](../resources/directoryObject.md) objects that a [tokenIssuancePolicy](../resources/tokenissuancepolicy.md) object has been applied to.</span></span> <span data-ttu-id="4c711-106">O tokenIssuancePolicy só pode ser aplicado ao [aplicativo](../resources/application.md).</span><span class="sxs-lookup"><span data-stu-id="4c711-106">The tokenIssuancePolicy can only be applied to [application](../resources/application.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="4c711-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="4c711-107">Permissions</span></span>

<span data-ttu-id="4c711-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4c711-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4c711-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4c711-110">Permission type</span></span>                        | <span data-ttu-id="4c711-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4c711-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="4c711-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4c711-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="4c711-113">Policy. Read. All e Application. Read. All, Policy. ReadWrite. ApplicationConfiguration e Application. Read. All, Directory. Read. All</span><span class="sxs-lookup"><span data-stu-id="4c711-113">Policy.Read.All and Application.Read.All, Policy.ReadWrite.ApplicationConfiguration and Application.Read.All, Directory.Read.All</span></span> |
| <span data-ttu-id="4c711-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4c711-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4c711-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4c711-115">Not supported.</span></span> |
| <span data-ttu-id="4c711-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4c711-116">Application</span></span>                            | <span data-ttu-id="4c711-117">Policy. Read. All e Application. Read. All, Policy. ReadWrite. ApplicationConfiguration e Application. Read. All, Directory. Read. All</span><span class="sxs-lookup"><span data-stu-id="4c711-117">Policy.Read.All and Application.Read.All, Policy.ReadWrite.ApplicationConfiguration and Application.Read.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4c711-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4c711-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /policies/tokenIssuancePolicies/{id}/appliesTo
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4c711-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="4c711-119">Optional query parameters</span></span>

<span data-ttu-id="4c711-120">Este método oferece suporte `$expand`a `$select`, e `$top` a parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="4c711-120">This method supports the `$expand`, `$select`, and `$top` OData query parameters to help customize the response.</span></span> <span data-ttu-id="4c711-121">Para obter informações gerais, confira [parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="4c711-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span> <span data-ttu-id="4c711-122">Ao usar `$expand`o, certifique-se de que seu aplicativo solicite permissões para ler os objetos expandidos.</span><span class="sxs-lookup"><span data-stu-id="4c711-122">When using `$expand`, make sure your app requests permissions to read the expanded objects.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4c711-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4c711-123">Request headers</span></span>

| <span data-ttu-id="4c711-124">Nome</span><span class="sxs-lookup"><span data-stu-id="4c711-124">Name</span></span>      |<span data-ttu-id="4c711-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="4c711-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="4c711-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="4c711-126">Authorization</span></span> | <span data-ttu-id="4c711-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4c711-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4c711-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4c711-129">Request body</span></span>

<span data-ttu-id="4c711-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="4c711-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4c711-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="4c711-131">Response</span></span>

<span data-ttu-id="4c711-132">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4c711-132">If successful, this method returns a `200 OK` response code and a collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="4c711-133">Exemplos</span><span class="sxs-lookup"><span data-stu-id="4c711-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="4c711-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4c711-134">Request</span></span>

<span data-ttu-id="4c711-135">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="4c711-135">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_appliesto"
}-->

```http
GET https://graph.microsoft.com/v1.0/policies/tokenIssuancePolicies/{id}/appliesTo
```

### <a name="response"></a><span data-ttu-id="4c711-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="4c711-136">Response</span></span>

<span data-ttu-id="4c711-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="4c711-137">The following is an example of the response.</span></span>

> <span data-ttu-id="4c711-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4c711-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
