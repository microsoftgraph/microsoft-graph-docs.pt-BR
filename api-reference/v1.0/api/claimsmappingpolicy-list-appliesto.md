---
title: Listar se aplica
description: Obtenha uma lista de objetos directoryobject aos quais um objeto claimsMappingPolicy foi aplicado.
localization_priority: Normal
author: paulgarn
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 99ac68ed7e44f690e7bd298b0e883a538892ff0e
ms.sourcegitcommit: 82da4012294b046416c9ae93d2294d80dab217f6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/04/2020
ms.locfileid: "48904914"
---
# <a name="list-appliesto"></a><span data-ttu-id="bb251-103">Listar se aplica</span><span class="sxs-lookup"><span data-stu-id="bb251-103">List appliesTo</span></span>

<span data-ttu-id="bb251-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bb251-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="bb251-105">Obtenha uma lista de objetos [directoryobject](../resources/directoryObject.md) aos quais um objeto [claimsMappingPolicy](../resources/claimsmappingpolicy.md) foi aplicado.</span><span class="sxs-lookup"><span data-stu-id="bb251-105">Get a list of [directoryObject](../resources/directoryObject.md) objects that a [claimsMappingPolicy](../resources/claimsmappingpolicy.md) object has been applied to.</span></span> <span data-ttu-id="bb251-106">O claimsMappingPolicy só pode ser aplicado aos recursos [Application](../resources/application.md) e [servicePrincipalName](../resources/serviceprincipal.md) .</span><span class="sxs-lookup"><span data-stu-id="bb251-106">The claimsMappingPolicy can only be applied to [application](../resources/application.md) and [servicePrincipal](../resources/serviceprincipal.md) resources.</span></span>

## <a name="permissions"></a><span data-ttu-id="bb251-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="bb251-107">Permissions</span></span>

<span data-ttu-id="bb251-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bb251-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="bb251-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bb251-110">Permission type</span></span>                        | <span data-ttu-id="bb251-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="bb251-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="bb251-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bb251-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="bb251-113">Policy. Read. All e Application. Read. All, Policy. ReadWrite. ApplicationConfiguration e Application. Read. All, Directory. Read. All</span><span class="sxs-lookup"><span data-stu-id="bb251-113">Policy.Read.All and Application.Read.All, Policy.ReadWrite.ApplicationConfiguration and Application.Read.All, Directory.Read.All</span></span> |
| <span data-ttu-id="bb251-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bb251-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bb251-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bb251-115">Not supported.</span></span> |
| <span data-ttu-id="bb251-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bb251-116">Application</span></span>                            | <span data-ttu-id="bb251-117">Policy. Read. All e Application. Read. All, Policy. ReadWrite. ApplicationConfiguration e Application. Read. All, Directory. Read. All</span><span class="sxs-lookup"><span data-stu-id="bb251-117">Policy.Read.All and Application.Read.All, Policy.ReadWrite.ApplicationConfiguration and Application.Read.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="bb251-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bb251-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /policies/claimsMappingPolicies/{id}/appliesTo
```

## <a name="optional-query-parameters"></a><span data-ttu-id="bb251-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="bb251-119">Optional query parameters</span></span>

<span data-ttu-id="bb251-120">Este método oferece suporte `$expand` ao `$select` e `$top` aos parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="bb251-120">This method supports the `$expand`, `$select` and `$top` OData query parameters to help customize the response.</span></span> <span data-ttu-id="bb251-121">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="bb251-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span> <span data-ttu-id="bb251-122">Ao usar `$expand` certifique-se de que seu aplicativo solicite permissões para ler os objetos expandidos.</span><span class="sxs-lookup"><span data-stu-id="bb251-122">When using `$expand` make sure your app requests permissions to read the expanded objects.</span></span>

## <a name="request-headers"></a><span data-ttu-id="bb251-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bb251-123">Request headers</span></span>

| <span data-ttu-id="bb251-124">Nome</span><span class="sxs-lookup"><span data-stu-id="bb251-124">Name</span></span>      |<span data-ttu-id="bb251-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="bb251-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="bb251-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="bb251-126">Authorization</span></span> | <span data-ttu-id="bb251-127">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="bb251-127">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="bb251-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bb251-128">Request body</span></span>

<span data-ttu-id="bb251-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="bb251-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bb251-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="bb251-130">Response</span></span>

<span data-ttu-id="bb251-131">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bb251-131">If successful, this method returns a `200 OK` response code and a collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="bb251-132">Exemplos</span><span class="sxs-lookup"><span data-stu-id="bb251-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="bb251-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bb251-133">Request</span></span>

<span data-ttu-id="bb251-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="bb251-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="bb251-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="bb251-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_appliesto"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/claimsMappingPolicies/{id}/appliesTo
```
# <a name="c"></a>[<span data-ttu-id="bb251-136">C#</span><span class="sxs-lookup"><span data-stu-id="bb251-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-appliesto-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="bb251-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bb251-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-appliesto-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="bb251-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bb251-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-appliesto-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="bb251-139">Java</span><span class="sxs-lookup"><span data-stu-id="bb251-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-appliesto-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="bb251-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="bb251-140">Response</span></span>

<span data-ttu-id="bb251-141">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="bb251-141">The following is an example of the response.</span></span>

> <span data-ttu-id="bb251-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="bb251-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
