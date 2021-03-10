---
title: Lista appliesTo
description: Obter uma lista de objetos directoryObject aos qual um objeto tokenIssuancePolicy foi aplicado.
localization_priority: Normal
author: luleonpla
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: d3d007b0f137e03df1401f00c23a636eccfec9d9
ms.sourcegitcommit: cde4a3386b08a67cb476df6d46b51885c643d94f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/10/2021
ms.locfileid: "50626220"
---
# <a name="list-appliesto"></a><span data-ttu-id="31815-103">Lista appliesTo</span><span class="sxs-lookup"><span data-stu-id="31815-103">List appliesTo</span></span>

<span data-ttu-id="31815-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="31815-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="31815-105">Obter uma lista de [objetos directoryObject](../resources/directoryObject.md) aos qual [um objeto tokenIssuancePolicy](../resources/tokenissuancepolicy.md) foi aplicado.</span><span class="sxs-lookup"><span data-stu-id="31815-105">Get a list of [directoryObject](../resources/directoryObject.md) objects that a [tokenIssuancePolicy](../resources/tokenissuancepolicy.md) object has been applied to.</span></span> <span data-ttu-id="31815-106">O tokenIssuancePolicy só pode ser aplicado aos recursos [application](../resources/application.md) e [servicePrincipal.](../resources/serviceprincipal.md)</span><span class="sxs-lookup"><span data-stu-id="31815-106">The tokenIssuancePolicy can only be applied to [application](../resources/application.md) and [servicePrincipal](../resources/serviceprincipal.md) resources.</span></span>

## <a name="permissions"></a><span data-ttu-id="31815-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="31815-107">Permissions</span></span>

<span data-ttu-id="31815-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="31815-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="31815-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="31815-110">Permission type</span></span>                        | <span data-ttu-id="31815-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="31815-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="31815-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="31815-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="31815-113">Policy.Read.All e Application.Read.All, Policy.ReadWrite.ApplicationConfiguration e Application.Read.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="31815-113">Policy.Read.All and Application.Read.All, Policy.ReadWrite.ApplicationConfiguration and Application.Read.All, Directory.Read.All</span></span> |
| <span data-ttu-id="31815-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="31815-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="31815-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="31815-115">Not supported.</span></span> |
| <span data-ttu-id="31815-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="31815-116">Application</span></span>                            | <span data-ttu-id="31815-117">Policy.Read.All e Application.Read.All, Policy.ReadWrite.ApplicationConfiguration e Application.Read.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="31815-117">Policy.Read.All and Application.Read.All, Policy.ReadWrite.ApplicationConfiguration and Application.Read.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="31815-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="31815-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /policies/tokenIssuancePolicies/{id}/appliesTo
```

## <a name="optional-query-parameters"></a><span data-ttu-id="31815-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="31815-119">Optional query parameters</span></span>

<span data-ttu-id="31815-120">Este método dá suporte `$expand` aos `$select` parâmetros de consulta , e OData para ajudar a personalizar `$top` a resposta.</span><span class="sxs-lookup"><span data-stu-id="31815-120">This method supports the `$expand`, `$select`, and `$top` OData query parameters to help customize the response.</span></span> <span data-ttu-id="31815-121">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="31815-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span> <span data-ttu-id="31815-122">Ao usar `$expand` , certifique-se de que seu aplicativo solicita permissões para ler os objetos expandidos.</span><span class="sxs-lookup"><span data-stu-id="31815-122">When using `$expand`, make sure your app requests permissions to read the expanded objects.</span></span>

## <a name="request-headers"></a><span data-ttu-id="31815-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="31815-123">Request headers</span></span>

| <span data-ttu-id="31815-124">Nome</span><span class="sxs-lookup"><span data-stu-id="31815-124">Name</span></span>      |<span data-ttu-id="31815-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="31815-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="31815-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="31815-126">Authorization</span></span> | <span data-ttu-id="31815-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="31815-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="31815-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="31815-129">Request body</span></span>

<span data-ttu-id="31815-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="31815-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="31815-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="31815-131">Response</span></span>

<span data-ttu-id="31815-132">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="31815-132">If successful, this method returns a `200 OK` response code and a collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="31815-133">Exemplos</span><span class="sxs-lookup"><span data-stu-id="31815-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="31815-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="31815-134">Request</span></span>

<span data-ttu-id="31815-135">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="31815-135">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_appliesto"
}-->

```http
GET https://graph.microsoft.com/beta/policies/tokenIssuancePolicies/{id}/appliesTo
```

### <a name="response"></a><span data-ttu-id="31815-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="31815-136">Response</span></span>

<span data-ttu-id="31815-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="31815-137">The following is an example of the response.</span></span>

> <span data-ttu-id="31815-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="31815-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


