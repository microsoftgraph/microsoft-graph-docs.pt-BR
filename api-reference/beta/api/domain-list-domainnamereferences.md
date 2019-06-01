---
title: Listar domainNameReferences
description: Recupere uma lista de directoryobject com uma referência ao domínio. A lista retornada conterá todos os objetos de diretório que têm uma dependência no domínio.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: cee100f73fafe39078ef011c509fb94be07fe282
ms.sourcegitcommit: 33f1cf5b3b79bfba6a06b52d34e558a6ba327d21
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2019
ms.locfileid: "34655716"
---
# <a name="list-domainnamereferences"></a><span data-ttu-id="d27eb-104">Listar domainNameReferences</span><span class="sxs-lookup"><span data-stu-id="d27eb-104">List domainNameReferences</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d27eb-105">Recupere uma lista de [directoryobject](../resources/directoryobject.md) com uma referência ao domínio.</span><span class="sxs-lookup"><span data-stu-id="d27eb-105">Retrieve a list of [directoryObject](../resources/directoryobject.md) with a reference to the domain.</span></span> <span data-ttu-id="d27eb-106">A lista retornada conterá todos os objetos de diretório que têm uma dependência no domínio.</span><span class="sxs-lookup"><span data-stu-id="d27eb-106">The returned list will contain all directory objects that have a dependency on the domain.</span></span>

## <a name="permissions"></a><span data-ttu-id="d27eb-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="d27eb-107">Permissions</span></span>

<span data-ttu-id="d27eb-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d27eb-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="d27eb-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d27eb-110">Permission type</span></span>      | <span data-ttu-id="d27eb-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d27eb-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d27eb-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d27eb-112">Delegated (work or school account)</span></span> | <span data-ttu-id="d27eb-113">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="d27eb-113">Directory.Read.All</span></span>    |
|<span data-ttu-id="d27eb-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d27eb-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d27eb-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d27eb-115">Not supported.</span></span>    |
|<span data-ttu-id="d27eb-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d27eb-116">Application</span></span> | <span data-ttu-id="d27eb-117">Directory.Read.All, Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d27eb-117">Directory.Read.All, Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d27eb-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d27eb-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /domains/{id}/domainNameReferences
```

> <span data-ttu-id="d27eb-119">Para {id}, especifique o domínio com seu nome de domínio totalmente qualificado.</span><span class="sxs-lookup"><span data-stu-id="d27eb-119">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="d27eb-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="d27eb-120">Optional query parameters</span></span>

<span data-ttu-id="d27eb-121">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="d27eb-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d27eb-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d27eb-122">Request headers</span></span>

| <span data-ttu-id="d27eb-123">Nome</span><span class="sxs-lookup"><span data-stu-id="d27eb-123">Name</span></span>      |<span data-ttu-id="d27eb-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="d27eb-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="d27eb-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="d27eb-125">Authorization</span></span>  | <span data-ttu-id="d27eb-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d27eb-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d27eb-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d27eb-128">Request body</span></span>

<span data-ttu-id="d27eb-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d27eb-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d27eb-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="d27eb-130">Response</span></span>

<span data-ttu-id="d27eb-131">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d27eb-131">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d27eb-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d27eb-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d27eb-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d27eb-133">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_domainnamereferences"
}-->
```http
GET https://graph.microsoft.com/beta/domains/contoso.com/domainNameReferences
```

##### <a name="response"></a><span data-ttu-id="d27eb-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="d27eb-134">Response</span></span>
<span data-ttu-id="d27eb-p105">Observação: O objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d27eb-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="d27eb-137">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="d27eb-137">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="d27eb-138">C#</span><span class="sxs-lookup"><span data-stu-id="d27eb-138">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_domainnamereferences-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d27eb-139">Javascript</span><span class="sxs-lookup"><span data-stu-id="d27eb-139">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_domainnamereferences-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List domainNameReferences",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/domain-list-domainnamereferences.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/domain-list-domainnamereferences.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
