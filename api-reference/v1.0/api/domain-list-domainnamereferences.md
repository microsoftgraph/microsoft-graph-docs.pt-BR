---
title: Listar domainNameReferences
description: Recupere uma lista de directoryObject com uma referência ao domínio.
author: adimitui
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 82b406604740adf85a161068565482f263295718
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50434388"
---
# <a name="list-domainnamereferences"></a><span data-ttu-id="99fb8-103">Listar domainNameReferences</span><span class="sxs-lookup"><span data-stu-id="99fb8-103">List domainNameReferences</span></span>

<span data-ttu-id="99fb8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="99fb8-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="99fb8-105">Recupere uma lista [de directoryObject](../resources/directoryobject.md) com uma referência ao domínio.</span><span class="sxs-lookup"><span data-stu-id="99fb8-105">Retrieve a list of [directoryObject](../resources/directoryobject.md) with a reference to the domain.</span></span> <span data-ttu-id="99fb8-106">A lista retornada conterá todos os objetos de diretório que tenham uma dependência no domínio.</span><span class="sxs-lookup"><span data-stu-id="99fb8-106">The returned list will contain all directory objects that have a dependency on the domain.</span></span>

## <a name="permissions"></a><span data-ttu-id="99fb8-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="99fb8-107">Permissions</span></span>

<span data-ttu-id="99fb8-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="99fb8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="99fb8-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="99fb8-110">Permission type</span></span>      | <span data-ttu-id="99fb8-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="99fb8-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="99fb8-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="99fb8-112">Delegated (work or school account)</span></span> | <span data-ttu-id="99fb8-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="99fb8-113">Not supported.</span></span> |
|<span data-ttu-id="99fb8-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="99fb8-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="99fb8-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="99fb8-115">Not supported.</span></span>    |
|<span data-ttu-id="99fb8-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="99fb8-116">Application</span></span> | <span data-ttu-id="99fb8-117">Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="99fb8-117">Domain.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="99fb8-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="99fb8-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /domains/{id}/domainNameReferences
```

> <span data-ttu-id="99fb8-119">Para {id}, especifique o domínio com seu nome de domínio totalmente qualificado.</span><span class="sxs-lookup"><span data-stu-id="99fb8-119">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="99fb8-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="99fb8-120">Optional query parameters</span></span>

<span data-ttu-id="99fb8-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="99fb8-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="99fb8-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="99fb8-122">Request headers</span></span>

| <span data-ttu-id="99fb8-123">Nome</span><span class="sxs-lookup"><span data-stu-id="99fb8-123">Name</span></span>      |<span data-ttu-id="99fb8-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="99fb8-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="99fb8-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="99fb8-125">Authorization</span></span>  | <span data-ttu-id="99fb8-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="99fb8-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="99fb8-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="99fb8-128">Request body</span></span>

<span data-ttu-id="99fb8-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="99fb8-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="99fb8-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="99fb8-130">Response</span></span>

<span data-ttu-id="99fb8-131">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="99fb8-131">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="99fb8-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="99fb8-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="99fb8-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="99fb8-133">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="99fb8-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="99fb8-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_domainnamereferences"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/domains/{domain-name}/domainNameReferences
```
# <a name="c"></a>[<span data-ttu-id="99fb8-135">C#</span><span class="sxs-lookup"><span data-stu-id="99fb8-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-domainnamereferences-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="99fb8-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="99fb8-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-domainnamereferences-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="99fb8-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="99fb8-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-domainnamereferences-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="99fb8-138">Java</span><span class="sxs-lookup"><span data-stu-id="99fb8-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-domainnamereferences-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="99fb8-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="99fb8-139">Response</span></span>
<span data-ttu-id="99fb8-p104">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="99fb8-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
