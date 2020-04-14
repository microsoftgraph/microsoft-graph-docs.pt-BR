---
title: Obter orgContact
description: Recupere as propriedades e os relacionamentos do objeto orgcontact.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 50cb6d85b7bda47a14cbbb58439881c1126e15fc
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43467006"
---
# <a name="get-orgcontact"></a><span data-ttu-id="12a42-103">Obter orgContact</span><span class="sxs-lookup"><span data-stu-id="12a42-103">Get orgContact</span></span>

<span data-ttu-id="12a42-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="12a42-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="12a42-105">Obtenha as propriedades e os relacionamentos de um objeto de contato organizacional.</span><span class="sxs-lookup"><span data-stu-id="12a42-105">Get the properties and relationships of an organizational contact object.</span></span>

## <a name="permissions"></a><span data-ttu-id="12a42-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="12a42-106">Permissions</span></span>
<span data-ttu-id="12a42-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="12a42-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="12a42-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="12a42-109">Permission type</span></span>      | <span data-ttu-id="12a42-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="12a42-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="12a42-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="12a42-111">Delegated (work or school account)</span></span> | <span data-ttu-id="12a42-112">OrgContact. Read. All, Directory. Read. All, Directory. ReadWrite. All, Directory. AccessAsUser. All</span><span class="sxs-lookup"><span data-stu-id="12a42-112">OrgContact.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="12a42-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="12a42-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="12a42-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="12a42-114">Not supported.</span></span>    |
|<span data-ttu-id="12a42-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="12a42-115">Application</span></span> | <span data-ttu-id="12a42-116">OrgContact. Read. All, Directory. Read. All, Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="12a42-116">OrgContact.Read.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="12a42-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="12a42-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /contacts/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="12a42-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="12a42-118">Optional query parameters</span></span>
<span data-ttu-id="12a42-119">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="12a42-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="12a42-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="12a42-120">Request headers</span></span>
| <span data-ttu-id="12a42-121">Nome</span><span class="sxs-lookup"><span data-stu-id="12a42-121">Name</span></span>       | <span data-ttu-id="12a42-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="12a42-122">Type</span></span> | <span data-ttu-id="12a42-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="12a42-123">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="12a42-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="12a42-124">Authorization</span></span>  | <span data-ttu-id="12a42-125">string</span><span class="sxs-lookup"><span data-stu-id="12a42-125">string</span></span>  | <span data-ttu-id="12a42-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="12a42-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="12a42-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="12a42-128">Request body</span></span>
<span data-ttu-id="12a42-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="12a42-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="12a42-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="12a42-130">Response</span></span>

<span data-ttu-id="12a42-131">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [orgContact](../resources/orgcontact.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="12a42-131">If successful, this method returns a `200 OK` response code and [orgContact](../resources/orgcontact.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="12a42-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="12a42-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="12a42-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="12a42-133">Request</span></span>
<span data-ttu-id="12a42-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="12a42-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="12a42-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="12a42-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_orgcontact"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/contacts/{id}
```
# <a name="c"></a>[<span data-ttu-id="12a42-136">C#</span><span class="sxs-lookup"><span data-stu-id="12a42-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-orgcontact-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="12a42-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="12a42-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-orgcontact-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="12a42-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="12a42-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-orgcontact-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="12a42-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="12a42-139">Response</span></span>
<span data-ttu-id="12a42-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="12a42-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
