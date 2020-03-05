---
title: Listar domainNameReferences
description: Recupere uma lista de directoryobject com uma referência ao domínio. A lista retornada conterá todos os objetos de diretório que têm uma dependência no domínio.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 132a0449e2c8b586f9d42f818dbfc90d6e25957a
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42433605"
---
# <a name="list-domainnamereferences"></a><span data-ttu-id="ea803-104">Listar domainNameReferences</span><span class="sxs-lookup"><span data-stu-id="ea803-104">List domainNameReferences</span></span>

<span data-ttu-id="ea803-105">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="ea803-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ea803-106">Recupere uma lista de [directoryobject](../resources/directoryobject.md) com uma referência ao domínio.</span><span class="sxs-lookup"><span data-stu-id="ea803-106">Retrieve a list of [directoryObject](../resources/directoryobject.md) with a reference to the domain.</span></span> <span data-ttu-id="ea803-107">A lista retornada conterá todos os objetos de diretório que têm uma dependência no domínio.</span><span class="sxs-lookup"><span data-stu-id="ea803-107">The returned list will contain all directory objects that have a dependency on the domain.</span></span>

## <a name="permissions"></a><span data-ttu-id="ea803-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="ea803-108">Permissions</span></span>

<span data-ttu-id="ea803-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ea803-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="ea803-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ea803-111">Permission type</span></span>      | <span data-ttu-id="ea803-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ea803-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ea803-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ea803-113">Delegated (work or school account)</span></span> | <span data-ttu-id="ea803-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ea803-114">Not supported.</span></span> |
|<span data-ttu-id="ea803-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ea803-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ea803-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ea803-116">Not supported.</span></span>    |
|<span data-ttu-id="ea803-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ea803-117">Application</span></span> | <span data-ttu-id="ea803-118">Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ea803-118">Domain.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="ea803-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ea803-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /domains/{id}/domainNameReferences
```

> <span data-ttu-id="ea803-120">Para {id}, especifique o domínio com seu nome de domínio totalmente qualificado.</span><span class="sxs-lookup"><span data-stu-id="ea803-120">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="ea803-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="ea803-121">Optional query parameters</span></span>

<span data-ttu-id="ea803-122">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="ea803-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ea803-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ea803-123">Request headers</span></span>

| <span data-ttu-id="ea803-124">Nome</span><span class="sxs-lookup"><span data-stu-id="ea803-124">Name</span></span>      |<span data-ttu-id="ea803-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="ea803-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="ea803-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="ea803-126">Authorization</span></span>  | <span data-ttu-id="ea803-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ea803-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ea803-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ea803-129">Request body</span></span>

<span data-ttu-id="ea803-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ea803-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ea803-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="ea803-131">Response</span></span>

<span data-ttu-id="ea803-132">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ea803-132">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ea803-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ea803-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ea803-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ea803-134">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="ea803-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="ea803-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_domainnamereferences"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/domains/contoso.com/domainNameReferences
```
# <a name="c"></a>[<span data-ttu-id="ea803-136">C#</span><span class="sxs-lookup"><span data-stu-id="ea803-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-domainnamereferences-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ea803-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ea803-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-domainnamereferences-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ea803-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ea803-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-domainnamereferences-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="ea803-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="ea803-139">Response</span></span>
<span data-ttu-id="ea803-p105">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ea803-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  ]
}
-->
