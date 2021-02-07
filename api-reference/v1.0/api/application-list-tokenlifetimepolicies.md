---
title: Listar tokenLifetimePolicies atribuído
description: Listar tokenLifetimePolicies que são atribuídos a um aplicativo.
localization_priority: Normal
author: sureshja
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: df91b09be98e20245acf9c4f5957631868c11a13
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50129693"
---
# <a name="list-assigned-tokenlifetimepolicy"></a><span data-ttu-id="945b6-103">Listar tokenLifetimePolicy atribuído</span><span class="sxs-lookup"><span data-stu-id="945b6-103">List assigned tokenLifetimePolicy</span></span>

<span data-ttu-id="945b6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="945b6-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="945b6-105">Listar [os objetos tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) atribuídos a um [aplicativo.](../resources/application.md)</span><span class="sxs-lookup"><span data-stu-id="945b6-105">List the [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) objects that are assigned to an [application](../resources/application.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="945b6-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="945b6-106">Permissions</span></span>

<span data-ttu-id="945b6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="945b6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="945b6-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="945b6-109">Permission type</span></span>                        | <span data-ttu-id="945b6-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="945b6-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="945b6-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="945b6-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="945b6-112">Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="945b6-112">Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |
| <span data-ttu-id="945b6-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="945b6-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="945b6-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="945b6-114">Not supported.</span></span> |
| <span data-ttu-id="945b6-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="945b6-115">Application</span></span>                            | <span data-ttu-id="945b6-116">Policy.Read.All and Application.ReadWrite.OwnedBy, Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.OwnedBy, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="945b6-116">Policy.Read.All and Application.ReadWrite.OwnedBy, Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.OwnedBy, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="945b6-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="945b6-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /applications/{id}/tokenLifetimePolicies
```

## <a name="request-headers"></a><span data-ttu-id="945b6-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="945b6-118">Request headers</span></span>

| <span data-ttu-id="945b6-119">Nome</span><span class="sxs-lookup"><span data-stu-id="945b6-119">Name</span></span>          | <span data-ttu-id="945b6-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="945b6-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="945b6-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="945b6-121">Authorization</span></span> | <span data-ttu-id="945b6-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="945b6-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="945b6-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="945b6-124">Request body</span></span>

<span data-ttu-id="945b6-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="945b6-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="945b6-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="945b6-126">Response</span></span>

<span data-ttu-id="945b6-127">Se bem-sucedido, este método retorna um código de resposta e uma coleção de `200 OK` [objetos tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="945b6-127">If successful, this method returns a `200 OK` response code and a collection of [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="945b6-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="945b6-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="945b6-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="945b6-129">Request</span></span>

<span data-ttu-id="945b6-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="945b6-130">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="945b6-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="945b6-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_tokenlifetimepolicies_on_application"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/applications/{id}/tokenLifetimePolicies
```
# <a name="c"></a>[<span data-ttu-id="945b6-132">C#</span><span class="sxs-lookup"><span data-stu-id="945b6-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-tokenlifetimepolicies-on-application-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="945b6-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="945b6-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-tokenlifetimepolicies-on-application-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="945b6-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="945b6-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-tokenlifetimepolicies-on-application-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="945b6-135">Java</span><span class="sxs-lookup"><span data-stu-id="945b6-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-tokenlifetimepolicies-on-application-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="945b6-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="945b6-136">Response</span></span>

<span data-ttu-id="945b6-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="945b6-137">The following is an example of the response.</span></span>

> <span data-ttu-id="945b6-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="945b6-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.tokenLifetimePolicy",
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
  "description": "List assigned tokenLifetimePolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

