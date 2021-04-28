---
title: Lista appliesTo
description: Obter uma lista de objetos directoryObject aos qual um objeto tokenLifetimePolicy foi aplicado.
localization_priority: Normal
author: lujiangfeng666
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 37926ca3c92e1ad44cba9aaa0951ceb6568ede2b
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52054333"
---
# <a name="list-appliesto"></a><span data-ttu-id="a9892-103">Lista appliesTo</span><span class="sxs-lookup"><span data-stu-id="a9892-103">List appliesTo</span></span>

<span data-ttu-id="a9892-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a9892-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="a9892-105">Obter uma lista de [objetos directoryObject](../resources/directoryObject.md) aos qual [um objeto tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) foi aplicado.</span><span class="sxs-lookup"><span data-stu-id="a9892-105">Get a list of [directoryObject](../resources/directoryObject.md) objects that a [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) object has been applied to.</span></span> <span data-ttu-id="a9892-106">O tokenLifetimePolicy só pode ser aplicado ao [aplicativo](../resources/application.md).</span><span class="sxs-lookup"><span data-stu-id="a9892-106">The tokenLifetimePolicy can only be applied to [application](../resources/application.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="a9892-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="a9892-107">Permissions</span></span>

<span data-ttu-id="a9892-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a9892-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a9892-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a9892-110">Permission type</span></span>                        | <span data-ttu-id="a9892-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a9892-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="a9892-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a9892-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="a9892-113">Policy.Read.All e Application.Read.All, Policy.ReadWrite.ApplicationConfiguration e Application.Read.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="a9892-113">Policy.Read.All and Application.Read.All, Policy.ReadWrite.ApplicationConfiguration and Application.Read.All, Directory.Read.All</span></span> |
| <span data-ttu-id="a9892-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a9892-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a9892-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a9892-115">Not supported.</span></span> |
| <span data-ttu-id="a9892-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a9892-116">Application</span></span>                            | <span data-ttu-id="a9892-117">Policy.Read.All e Application.Read.All, Policy.ReadWrite.ApplicationConfiguration e Application.Read.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="a9892-117">Policy.Read.All and Application.Read.All, Policy.ReadWrite.ApplicationConfiguration and Application.Read.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a9892-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a9892-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /policies/tokenLifetimePolicies/{id}/appliesTo
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a9892-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="a9892-119">Optional query parameters</span></span>

<span data-ttu-id="a9892-120">Este método dá suporte aos `$expand` parâmetros de consulta , `$select` e `$top` OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="a9892-120">This method supports the `$expand`, `$select` and `$top` OData query parameters to help customize the response.</span></span> <span data-ttu-id="a9892-121">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="a9892-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span> <span data-ttu-id="a9892-122">Ao `$expand` usar, certifique-se de que seu aplicativo solicita permissões para ler os objetos expandidos.</span><span class="sxs-lookup"><span data-stu-id="a9892-122">When using `$expand` make sure your app requests permissions to read the expanded objects.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a9892-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a9892-123">Request headers</span></span>

| <span data-ttu-id="a9892-124">Nome</span><span class="sxs-lookup"><span data-stu-id="a9892-124">Name</span></span>      |<span data-ttu-id="a9892-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="a9892-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="a9892-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="a9892-126">Authorization</span></span> | <span data-ttu-id="a9892-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a9892-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a9892-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a9892-129">Request body</span></span>

<span data-ttu-id="a9892-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a9892-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a9892-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="a9892-131">Response</span></span>

<span data-ttu-id="a9892-132">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a9892-132">If successful, this method returns a `200 OK` response code and a collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a9892-133">Exemplos</span><span class="sxs-lookup"><span data-stu-id="a9892-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a9892-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a9892-134">Request</span></span>

<span data-ttu-id="a9892-135">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="a9892-135">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a9892-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="a9892-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_appliesto_4"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/policies/tokenLifetimePolicies/{id}/appliesTo
```
# <a name="c"></a>[<span data-ttu-id="a9892-137">C#</span><span class="sxs-lookup"><span data-stu-id="a9892-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-appliesto-4-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a9892-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a9892-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-appliesto-4-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a9892-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a9892-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-appliesto-4-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a9892-140">Java</span><span class="sxs-lookup"><span data-stu-id="a9892-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-appliesto-4-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="a9892-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="a9892-141">Response</span></span>

<span data-ttu-id="a9892-142">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="a9892-142">The following is an example of the response.</span></span>

> <span data-ttu-id="a9892-143">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="a9892-143">**Note:** The response object shown here might be shortened for readability.</span></span>

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

