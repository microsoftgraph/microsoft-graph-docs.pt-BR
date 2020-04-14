---
title: Listar orgContacts
description: Recupere a lista de contatos organizacionais desta organização.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 87669fb0665a11d1f3bc6f1bf923cd55e1ee3af3
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43474727"
---
# <a name="list-orgcontacts"></a><span data-ttu-id="f3986-103">Listar orgContacts</span><span class="sxs-lookup"><span data-stu-id="f3986-103">List orgContacts</span></span>

<span data-ttu-id="f3986-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f3986-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f3986-105">Obtenha a lista de contatos organizacionais para esta organização.</span><span class="sxs-lookup"><span data-stu-id="f3986-105">Get the list of organizational contacts for this organization.</span></span>

## <a name="permissions"></a><span data-ttu-id="f3986-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="f3986-106">Permissions</span></span>
<span data-ttu-id="f3986-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f3986-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f3986-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f3986-109">Permission type</span></span>      | <span data-ttu-id="f3986-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f3986-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f3986-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f3986-111">Delegated (work or school account)</span></span> | <span data-ttu-id="f3986-112">OrgContact. Read. All, Directory. Read. All, Directory. ReadWrite. All, Directory. AccessAsUser. All</span><span class="sxs-lookup"><span data-stu-id="f3986-112">OrgContact.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="f3986-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f3986-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f3986-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f3986-114">Not supported.</span></span>    |
|<span data-ttu-id="f3986-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f3986-115">Application</span></span> | <span data-ttu-id="f3986-116">OrgContact. Read. All, Directory. Read. All, Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="f3986-116">OrgContact.Read.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f3986-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f3986-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /contacts
```
## <a name="optional-query-parameters"></a><span data-ttu-id="f3986-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="f3986-118">Optional query parameters</span></span>
<span data-ttu-id="f3986-119">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="f3986-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f3986-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f3986-120">Request headers</span></span>
| <span data-ttu-id="f3986-121">Nome</span><span class="sxs-lookup"><span data-stu-id="f3986-121">Name</span></span>       | <span data-ttu-id="f3986-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="f3986-122">Type</span></span> | <span data-ttu-id="f3986-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="f3986-123">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="f3986-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="f3986-124">Authorization</span></span>  | <span data-ttu-id="f3986-125">string</span><span class="sxs-lookup"><span data-stu-id="f3986-125">string</span></span>  | <span data-ttu-id="f3986-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f3986-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f3986-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f3986-128">Request body</span></span>
<span data-ttu-id="f3986-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f3986-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f3986-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="f3986-130">Response</span></span>

<span data-ttu-id="f3986-131">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [orgContact](../resources/orgcontact.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f3986-131">If successful, this method returns a `200 OK` response code and a collection of [orgContact](../resources/orgcontact.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f3986-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f3986-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f3986-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f3986-133">Request</span></span>
<span data-ttu-id="f3986-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f3986-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="f3986-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="f3986-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_orgcontact"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/contacts
```
# <a name="c"></a>[<span data-ttu-id="f3986-136">C#</span><span class="sxs-lookup"><span data-stu-id="f3986-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-orgcontact-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f3986-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f3986-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-orgcontact-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f3986-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f3986-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-orgcontact-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="f3986-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="f3986-139">Response</span></span>
<span data-ttu-id="f3986-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f3986-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.orgcontact",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 222

{
  "value": [
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
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List orgContact",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
