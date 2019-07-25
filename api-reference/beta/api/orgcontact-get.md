---
title: Obter orgContact
description: Recupere as propriedades e os relacionamentos do objeto orgcontact.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 9bf4704135dcc66cb38281f131abbe9bbc51110c
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35877916"
---
# <a name="get-orgcontact"></a><span data-ttu-id="e5b8b-103">Obter orgContact</span><span class="sxs-lookup"><span data-stu-id="e5b8b-103">Get orgContact</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e5b8b-104">Recupere as propriedades e os relacionamentos do objeto orgcontact.</span><span class="sxs-lookup"><span data-stu-id="e5b8b-104">Retrieve the properties and relationships of orgcontact object.</span></span>
## <a name="permissions"></a><span data-ttu-id="e5b8b-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="e5b8b-105">Permissions</span></span>
<span data-ttu-id="e5b8b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e5b8b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e5b8b-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e5b8b-108">Permission type</span></span>      | <span data-ttu-id="e5b8b-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e5b8b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e5b8b-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e5b8b-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e5b8b-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="e5b8b-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="e5b8b-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e5b8b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e5b8b-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e5b8b-113">Not supported.</span></span>    |
|<span data-ttu-id="e5b8b-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e5b8b-114">Application</span></span> | <span data-ttu-id="e5b8b-115">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e5b8b-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e5b8b-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e5b8b-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /contacts/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="e5b8b-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="e5b8b-117">Optional query parameters</span></span>
<span data-ttu-id="e5b8b-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="e5b8b-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e5b8b-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e5b8b-119">Request headers</span></span>
| <span data-ttu-id="e5b8b-120">Nome</span><span class="sxs-lookup"><span data-stu-id="e5b8b-120">Name</span></span>       | <span data-ttu-id="e5b8b-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="e5b8b-121">Type</span></span> | <span data-ttu-id="e5b8b-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="e5b8b-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="e5b8b-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="e5b8b-123">Authorization</span></span>  | <span data-ttu-id="e5b8b-124">string</span><span class="sxs-lookup"><span data-stu-id="e5b8b-124">string</span></span>  | <span data-ttu-id="e5b8b-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e5b8b-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e5b8b-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e5b8b-127">Request body</span></span>
<span data-ttu-id="e5b8b-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e5b8b-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e5b8b-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="e5b8b-129">Response</span></span>

<span data-ttu-id="e5b8b-130">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [orgContact](../resources/orgcontact.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e5b8b-130">If successful, this method returns a `200 OK` response code and [orgContact](../resources/orgcontact.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e5b8b-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e5b8b-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e5b8b-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e5b8b-132">Request</span></span>
<span data-ttu-id="e5b8b-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e5b8b-133">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="e5b8b-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="e5b8b-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_orgcontact"
}-->
```http
GET https://graph.microsoft.com/beta/contacts/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="e5b8b-135">C#</span><span class="sxs-lookup"><span data-stu-id="e5b8b-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-orgcontact-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e5b8b-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="e5b8b-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-orgcontact-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="e5b8b-137">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="e5b8b-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-orgcontact-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="e5b8b-138">Java</span><span class="sxs-lookup"><span data-stu-id="e5b8b-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-orgcontact-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="e5b8b-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="e5b8b-139">Response</span></span>
<span data-ttu-id="e5b8b-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e5b8b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.orgcontact"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 222

{
  "addresses":[
      {
        "city": "string",
        "countryOrRegion": "string",
        "officeLocation": "string",
        "postalCode": "string",
        "state": "string",
        "street": "string"
      }
  ],
  "companyName": "companyName-value",
  "department": "department-value",
  "displayName": "displayName-value",
  "phones":[
      {
        "type": "string",
        "number": "string"
      }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get orgContact",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
