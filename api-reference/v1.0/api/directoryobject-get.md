---
title: Obter directoryObject
description: Recupere as propriedades e os relacionamentos do objeto directoryObject.
author: davidmu1
localization_priority: Priority
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 737c5d9d6abb4164d3df5509cc2e6d0577e6fbe2
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35882740"
---
# <a name="get-directoryobject"></a><span data-ttu-id="7fcae-103">Obter directoryObject</span><span class="sxs-lookup"><span data-stu-id="7fcae-103">Get directoryObject</span></span>

<span data-ttu-id="7fcae-104">Recupere as propriedades e os relacionamentos do objeto directoryObject.</span><span class="sxs-lookup"><span data-stu-id="7fcae-104">Retrieve the properties and relationships of directoryObject object.</span></span>
## <a name="permissions"></a><span data-ttu-id="7fcae-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="7fcae-105">Permissions</span></span>
<span data-ttu-id="7fcae-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7fcae-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7fcae-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7fcae-108">Permission type</span></span>      | <span data-ttu-id="7fcae-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7fcae-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7fcae-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7fcae-110">Delegated (work or school account)</span></span> | <span data-ttu-id="7fcae-111">Directory.Read.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="7fcae-111">Directory.Read.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="7fcae-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7fcae-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7fcae-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7fcae-113">Not supported.</span></span>    |
|<span data-ttu-id="7fcae-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7fcae-114">Application</span></span> | <span data-ttu-id="7fcae-115">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="7fcae-115">Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7fcae-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7fcae-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directoryObjects/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="7fcae-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="7fcae-117">Optional query parameters</span></span>
<span data-ttu-id="7fcae-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="7fcae-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="7fcae-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7fcae-119">Request headers</span></span>
| <span data-ttu-id="7fcae-120">Nome</span><span class="sxs-lookup"><span data-stu-id="7fcae-120">Name</span></span>       | <span data-ttu-id="7fcae-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="7fcae-121">Type</span></span> | <span data-ttu-id="7fcae-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="7fcae-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="7fcae-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="7fcae-123">Authorization</span></span>  | <span data-ttu-id="7fcae-124">string</span><span class="sxs-lookup"><span data-stu-id="7fcae-124">string</span></span>  | <span data-ttu-id="7fcae-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7fcae-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7fcae-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7fcae-127">Request body</span></span>
<span data-ttu-id="7fcae-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7fcae-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7fcae-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="7fcae-129">Response</span></span>

<span data-ttu-id="7fcae-130">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7fcae-130">If successful, this method returns a `200 OK` response code and [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="7fcae-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7fcae-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7fcae-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7fcae-132">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="7fcae-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="7fcae-133">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_directoryobject"
}-->
```http
GET https://graph.microsoft.com/v1.0/directoryObjects/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="7fcae-134">C#</span><span class="sxs-lookup"><span data-stu-id="7fcae-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-directoryobject-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7fcae-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="7fcae-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-directoryobject-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="7fcae-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7fcae-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-directoryobject-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="7fcae-137">Java</span><span class="sxs-lookup"><span data-stu-id="7fcae-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-directoryobject-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="7fcae-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="7fcae-138">Response</span></span>
<span data-ttu-id="7fcae-p103">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7fcae-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get directoryObject",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
