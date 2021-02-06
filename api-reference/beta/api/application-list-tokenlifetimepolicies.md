---
title: Listar tokenLifetimePolicies atribuído
description: Listar tokenLifetimePolicies que são atribuídos a um aplicativo ou servicePrincipal.
localization_priority: Normal
author: sureshja
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: 2ff6e58bf42dd6e78282a9f12d16b8025077c526
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50129146"
---
# <a name="list-assigned-tokenlifetimepolicy"></a><span data-ttu-id="ddb79-103">Listar tokenLifetimePolicy atribuído</span><span class="sxs-lookup"><span data-stu-id="ddb79-103">List assigned tokenLifetimePolicy</span></span>

<span data-ttu-id="ddb79-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ddb79-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ddb79-105">Listar [os objetos tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) que são atribuídos a um [aplicativo](../resources/application.md) ou [servicePrincipal](../resources/servicePrincipal.md)..</span><span class="sxs-lookup"><span data-stu-id="ddb79-105">List the [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) objects that are assigned to an [application](../resources/application.md) or [servicePrincipal](../resources/servicePrincipal.md)..</span></span>

## <a name="permissions"></a><span data-ttu-id="ddb79-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="ddb79-106">Permissions</span></span>

<span data-ttu-id="ddb79-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ddb79-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ddb79-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ddb79-109">Permission type</span></span>                        | <span data-ttu-id="ddb79-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ddb79-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="ddb79-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ddb79-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="ddb79-112">Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ddb79-112">Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |
| <span data-ttu-id="ddb79-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ddb79-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ddb79-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ddb79-114">Not supported.</span></span> |
| <span data-ttu-id="ddb79-115">Application</span><span class="sxs-lookup"><span data-stu-id="ddb79-115">Application</span></span>                            | <span data-ttu-id="ddb79-116">Policy.Read.All and Application.ReadWrite.OwnedBy, Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.OwnedBy, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ddb79-116">Policy.Read.All and Application.ReadWrite.OwnedBy, Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.OwnedBy, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ddb79-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ddb79-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /applications/{id}/tokenLifetimePolicies
GET /servicePrincipals/{id}/tokenLifetimePolicies
```

## <a name="request-headers"></a><span data-ttu-id="ddb79-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ddb79-118">Request headers</span></span>

| <span data-ttu-id="ddb79-119">Nome</span><span class="sxs-lookup"><span data-stu-id="ddb79-119">Name</span></span>          | <span data-ttu-id="ddb79-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="ddb79-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="ddb79-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="ddb79-121">Authorization</span></span> | <span data-ttu-id="ddb79-122">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="ddb79-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="ddb79-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ddb79-123">Request body</span></span>

<span data-ttu-id="ddb79-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ddb79-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ddb79-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="ddb79-125">Response</span></span>

<span data-ttu-id="ddb79-126">Se tiver êxito, este método retornará um código de resposta e uma coleção de `200 OK` [objetos tokenLifetimePolicy](../resources/tokenLifetimePolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ddb79-126">If successful, this method returns a `200 OK` response code and a collection of [tokenLifetimePolicy](../resources/tokenLifetimePolicy.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ddb79-127">Exemplos</span><span class="sxs-lookup"><span data-stu-id="ddb79-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ddb79-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ddb79-128">Request</span></span>

<span data-ttu-id="ddb79-129">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="ddb79-129">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ddb79-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="ddb79-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_tokenlifetimepolicies_on_application"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/applications/{id}/tokenLifetimePolicies
```
# <a name="c"></a>[<span data-ttu-id="ddb79-131">C#</span><span class="sxs-lookup"><span data-stu-id="ddb79-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-tokenlifetimepolicies-on-application-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ddb79-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ddb79-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-tokenlifetimepolicies-on-application-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ddb79-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ddb79-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-tokenlifetimepolicies-on-application-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ddb79-134">Java</span><span class="sxs-lookup"><span data-stu-id="ddb79-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-tokenlifetimepolicies-on-application-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="ddb79-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="ddb79-135">Response</span></span>

<span data-ttu-id="ddb79-136">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="ddb79-136">The following is an example of the response.</span></span>

> <span data-ttu-id="ddb79-p102">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ddb79-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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



