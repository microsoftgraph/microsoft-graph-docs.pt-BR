---
title: Listar domainNameReferences
description: Recupere uma lista de directoryobject com uma referência ao domínio. A lista retornada conterá todos os objetos de diretório que têm uma dependência no domínio.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: f1854882ce78084bfda3f428a19e4bc4cd02d78c
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33589192"
---
# <a name="list-domainnamereferences"></a><span data-ttu-id="70531-104">Listar domainNameReferences</span><span class="sxs-lookup"><span data-stu-id="70531-104">List domainNameReferences</span></span>

<span data-ttu-id="70531-105">Recupere uma lista de [directoryobject](../resources/directoryobject.md) com uma referência ao domínio.</span><span class="sxs-lookup"><span data-stu-id="70531-105">Retrieve a list of [directoryObject](../resources/directoryobject.md) with a reference to the domain.</span></span> <span data-ttu-id="70531-106">A lista retornada conterá todos os objetos de diretório que têm uma dependência no domínio.</span><span class="sxs-lookup"><span data-stu-id="70531-106">The returned list will contain all directory objects that have a dependency on the domain.</span></span>

## <a name="permissions"></a><span data-ttu-id="70531-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="70531-107">Permissions</span></span>

<span data-ttu-id="70531-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="70531-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="70531-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="70531-110">Permission type</span></span>      | <span data-ttu-id="70531-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="70531-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="70531-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="70531-112">Delegated (work or school account)</span></span> | <span data-ttu-id="70531-113">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="70531-113">Directory.Read.All</span></span>    |
|<span data-ttu-id="70531-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="70531-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="70531-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="70531-115">Not supported.</span></span>    |
|<span data-ttu-id="70531-116">Application</span><span class="sxs-lookup"><span data-stu-id="70531-116">Application</span></span> | <span data-ttu-id="70531-117">Directory.Read.All, Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="70531-117">Directory.Read.All, Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="70531-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="70531-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /domains/{id}/domainNameReferences
```

> <span data-ttu-id="70531-119">Para {id}, especifique o domínio com seu nome de domínio totalmente qualificado.</span><span class="sxs-lookup"><span data-stu-id="70531-119">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="70531-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="70531-120">Optional query parameters</span></span>

<span data-ttu-id="70531-121">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="70531-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="70531-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="70531-122">Request headers</span></span>

| <span data-ttu-id="70531-123">Nome</span><span class="sxs-lookup"><span data-stu-id="70531-123">Name</span></span>      |<span data-ttu-id="70531-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="70531-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="70531-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="70531-125">Authorization</span></span>  | <span data-ttu-id="70531-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="70531-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="70531-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="70531-128">Request body</span></span>

<span data-ttu-id="70531-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="70531-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="70531-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="70531-130">Response</span></span>

<span data-ttu-id="70531-131">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="70531-131">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="70531-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="70531-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="70531-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="70531-133">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_domainnamereferences"
}-->
```http
GET https://graph.microsoft.com/v1.0/domains/{domain-name}/domainNameReferences
```

##### <a name="response"></a><span data-ttu-id="70531-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="70531-134">Response</span></span>
<span data-ttu-id="70531-p105">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="70531-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
        "odata.type": "Microsoft.DirectoryServices.User",
        "objectType": "User",
        "objectId": "567a0db6-289c-43f7-a650-2645c03cbbbb",
        "accountEnabled": true,
        "displayName": "TestUser1",
        "facsimileTelephoneNumber": null,
        "mailNickname": "testuser1",
        "mobile": null,
        "userPrincipalName": "testuser1@contoso.com"
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="70531-137">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="70531-137">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="70531-138">Basic</span><span class="sxs-lookup"><span data-stu-id="70531-138">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_domainnamereferences-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="70531-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="70531-139">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_domainnamereferences-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List domainNameReferences",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/domain-list-domainnamereferences.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/domain-list-domainnamereferences.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
