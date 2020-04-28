---
title: Listar se aplica
description: Obtenha uma lista de objetos directoryobject aos quais um objeto tokenIssuancePolicy foi aplicado.
localization_priority: Normal
author: luleonpla
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 44744f507131633c1c53c5922c4c068a76bf1ac8
ms.sourcegitcommit: 79988a42d91cc25bdd1c531b5f3261901d720a9a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/28/2020
ms.locfileid: "43917448"
---
# <a name="list-appliesto"></a><span data-ttu-id="62a79-103">Listar se aplica</span><span class="sxs-lookup"><span data-stu-id="62a79-103">List appliesTo</span></span>

<span data-ttu-id="62a79-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="62a79-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="62a79-105">Obtenha uma lista de objetos [directoryobject](../resources/directoryObject.md) aos quais um objeto [tokenIssuancePolicy](../resources/tokenissuancepolicy.md) foi aplicado.</span><span class="sxs-lookup"><span data-stu-id="62a79-105">Get a list of [directoryObject](../resources/directoryObject.md) objects that a [tokenIssuancePolicy](../resources/tokenissuancepolicy.md) object has been applied to.</span></span> <span data-ttu-id="62a79-106">O tokenIssuancePolicy só pode ser aplicado aos recursos [Application](../resources/application.md) e [servicePrincipalName](../resources/serviceprincipal.md) .</span><span class="sxs-lookup"><span data-stu-id="62a79-106">The tokenIssuancePolicy can only be applied to [application](../resources/application.md) and [servicePrincipal](../resources/serviceprincipal.md) resources.</span></span>

## <a name="permissions"></a><span data-ttu-id="62a79-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="62a79-107">Permissions</span></span>

<span data-ttu-id="62a79-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="62a79-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="62a79-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="62a79-110">Permission type</span></span>                        | <span data-ttu-id="62a79-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="62a79-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="62a79-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="62a79-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="62a79-113">Policy. Read. All e Application. Read. All, Policy. ReadWrite. ApplicationConfiguration e Application. Read. All, Directory. Read. All</span><span class="sxs-lookup"><span data-stu-id="62a79-113">Policy.Read.All and Application.Read.All, Policy.ReadWrite.ApplicationConfiguration and Application.Read.All, Directory.Read.All</span></span> |
| <span data-ttu-id="62a79-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="62a79-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="62a79-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="62a79-115">Not supported.</span></span> |
| <span data-ttu-id="62a79-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="62a79-116">Application</span></span>                            | <span data-ttu-id="62a79-117">Policy. Read. All e Application. Read. All, Policy. ReadWrite. ApplicationConfiguration e Application. Read. All, Directory. Read. All</span><span class="sxs-lookup"><span data-stu-id="62a79-117">Policy.Read.All and Application.Read.All, Policy.ReadWrite.ApplicationConfiguration and Application.Read.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="62a79-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="62a79-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /policies/tokenIssuancePolicies/{id}/appliesTo
```

## <a name="optional-query-parameters"></a><span data-ttu-id="62a79-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="62a79-119">Optional query parameters</span></span>

<span data-ttu-id="62a79-120">Este método oferece suporte `$expand`a `$select`, e `$top` a parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="62a79-120">This method supports the `$expand`, `$select`, and `$top` OData query parameters to help customize the response.</span></span> <span data-ttu-id="62a79-121">Para obter informações gerais, confira [parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="62a79-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span> <span data-ttu-id="62a79-122">Ao usar `$expand`o, certifique-se de que seu aplicativo solicite permissões para ler os objetos expandidos.</span><span class="sxs-lookup"><span data-stu-id="62a79-122">When using `$expand`, make sure your app requests permissions to read the expanded objects.</span></span>

## <a name="request-headers"></a><span data-ttu-id="62a79-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="62a79-123">Request headers</span></span>

| <span data-ttu-id="62a79-124">Nome</span><span class="sxs-lookup"><span data-stu-id="62a79-124">Name</span></span>      |<span data-ttu-id="62a79-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="62a79-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="62a79-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="62a79-126">Authorization</span></span> | <span data-ttu-id="62a79-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="62a79-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="62a79-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="62a79-129">Request body</span></span>

<span data-ttu-id="62a79-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="62a79-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="62a79-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="62a79-131">Response</span></span>

<span data-ttu-id="62a79-132">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="62a79-132">If successful, this method returns a `200 OK` response code and a collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="62a79-133">Exemplos</span><span class="sxs-lookup"><span data-stu-id="62a79-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="62a79-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="62a79-134">Request</span></span>

<span data-ttu-id="62a79-135">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="62a79-135">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_appliesto"
}-->

```http
GET https://graph.microsoft.com/beta/tokenIssuancePolicies/{id}/appliesTo
```

### <a name="response"></a><span data-ttu-id="62a79-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="62a79-136">Response</span></span>

<span data-ttu-id="62a79-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="62a79-137">The following is an example of the response.</span></span>

> <span data-ttu-id="62a79-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="62a79-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
