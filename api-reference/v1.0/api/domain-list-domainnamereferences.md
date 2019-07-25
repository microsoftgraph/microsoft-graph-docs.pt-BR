---
title: Listar domainNameReferences
description: Recupere uma lista de directoryobject com uma referência ao domínio. A lista retornada conterá todos os objetos de diretório que têm uma dependência no domínio.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 66d60f512310455c51d36e7a0ba685ae2a245010
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35889893"
---
# <a name="list-domainnamereferences"></a><span data-ttu-id="b64ac-104">Listar domainNameReferences</span><span class="sxs-lookup"><span data-stu-id="b64ac-104">List domainNameReferences</span></span>

<span data-ttu-id="b64ac-105">Recupere uma lista de [directoryobject](../resources/directoryobject.md) com uma referência ao domínio.</span><span class="sxs-lookup"><span data-stu-id="b64ac-105">Retrieve a list of [directoryObject](../resources/directoryobject.md) with a reference to the domain.</span></span> <span data-ttu-id="b64ac-106">A lista retornada conterá todos os objetos de diretório que têm uma dependência no domínio.</span><span class="sxs-lookup"><span data-stu-id="b64ac-106">The returned list will contain all directory objects that have a dependency on the domain.</span></span>

## <a name="permissions"></a><span data-ttu-id="b64ac-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="b64ac-107">Permissions</span></span>

<span data-ttu-id="b64ac-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b64ac-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="b64ac-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b64ac-110">Permission type</span></span>      | <span data-ttu-id="b64ac-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b64ac-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b64ac-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b64ac-112">Delegated (work or school account)</span></span> | <span data-ttu-id="b64ac-113">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="b64ac-113">Directory.Read.All</span></span>    |
|<span data-ttu-id="b64ac-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b64ac-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b64ac-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b64ac-115">Not supported.</span></span>    |
|<span data-ttu-id="b64ac-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b64ac-116">Application</span></span> | <span data-ttu-id="b64ac-117">Directory.Read.All, Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b64ac-117">Directory.Read.All, Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b64ac-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b64ac-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /domains/{id}/domainNameReferences
```

> <span data-ttu-id="b64ac-119">Para {id}, especifique o domínio com seu nome de domínio totalmente qualificado.</span><span class="sxs-lookup"><span data-stu-id="b64ac-119">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="b64ac-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="b64ac-120">Optional query parameters</span></span>

<span data-ttu-id="b64ac-121">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="b64ac-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b64ac-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b64ac-122">Request headers</span></span>

| <span data-ttu-id="b64ac-123">Nome</span><span class="sxs-lookup"><span data-stu-id="b64ac-123">Name</span></span>      |<span data-ttu-id="b64ac-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="b64ac-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="b64ac-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="b64ac-125">Authorization</span></span>  | <span data-ttu-id="b64ac-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b64ac-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b64ac-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b64ac-128">Request body</span></span>

<span data-ttu-id="b64ac-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b64ac-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b64ac-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="b64ac-130">Response</span></span>

<span data-ttu-id="b64ac-131">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b64ac-131">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b64ac-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b64ac-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b64ac-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b64ac-133">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="b64ac-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="b64ac-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_domainnamereferences"
}-->
```http
GET https://graph.microsoft.com/v1.0/domains/{domain-name}/domainNameReferences
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="b64ac-135">C#</span><span class="sxs-lookup"><span data-stu-id="b64ac-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-domainnamereferences-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b64ac-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="b64ac-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-domainnamereferences-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="b64ac-137">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="b64ac-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-domainnamereferences-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="b64ac-138">Java</span><span class="sxs-lookup"><span data-stu-id="b64ac-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-domainnamereferences-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="b64ac-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="b64ac-139">Response</span></span>
<span data-ttu-id="b64ac-p105">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b64ac-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "List domainNameReferences",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
