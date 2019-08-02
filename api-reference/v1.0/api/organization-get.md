---
title: Obter organização
description: Recupere as propriedades e os relacionamentos da organização autenticada no momento.
localization_priority: Priority
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 87b4284416e68b411bd772a86b9984f18848c6b9
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36022681"
---
# <a name="get-organization"></a><span data-ttu-id="92a01-103">Obter organização</span><span class="sxs-lookup"><span data-stu-id="92a01-103">Get organization</span></span>

<span data-ttu-id="92a01-104">Obtenha as propriedades e relações da organização autenticada no momento.</span><span class="sxs-lookup"><span data-stu-id="92a01-104">Retrieve the properties and relationships of currently authenticated organization.</span></span>

<span data-ttu-id="92a01-105">Como o recurso da **organização** tem suporte para [extensões](/graph/extensibility-overview), você também pode usar a operação `GET` para obter propriedades personalizadas e dados de extensão em uma instância de **organização**.</span><span class="sxs-lookup"><span data-stu-id="92a01-105">Since the **event** resource supports [extensions](/graph/extensibility-overview), you can also use the `GET` operation to get custom properties and extension data in an **event** instance.</span></span>

## <a name="permissions"></a><span data-ttu-id="92a01-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="92a01-106">Permissions</span></span>

<span data-ttu-id="92a01-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="92a01-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="92a01-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="92a01-109">Permission type</span></span>      | <span data-ttu-id="92a01-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="92a01-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="92a01-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="92a01-111">Delegated (work or school account)</span></span> | <span data-ttu-id="92a01-112">User.Read, Organization.Read.All, Directory.Read.All, Organization.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="92a01-112">User.Read, Group.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>   |
|<span data-ttu-id="92a01-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="92a01-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="92a01-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="92a01-114">Not supported.</span></span>    |
|<span data-ttu-id="92a01-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="92a01-115">Application</span></span> | <span data-ttu-id="92a01-116">Organization.Read.All, Directory.Read.All, Organization.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="92a01-116">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

> <span data-ttu-id="92a01-117">**Observação**: Os aplicativos que tem a permissão User.Read só conseguem ler as propriedades **id**, **displayName** e **verifiedDomains** da organização.</span><span class="sxs-lookup"><span data-stu-id="92a01-117">Note: Applications granted the User.Read permission are able to read only the id, displayName, and verifiedDomains properties of the organization.</span></span>  <span data-ttu-id="92a01-118">Todas as outras propriedades retornarão valores `null`.</span><span class="sxs-lookup"><span data-stu-id="92a01-118">All other properties will return with `null` values.</span></span> <span data-ttu-id="92a01-119">Para ler todas as propriedades, use Organization.Read.All.</span><span class="sxs-lookup"><span data-stu-id="92a01-119">To read all properties, use Directory.Read.All.</span></span>

## <a name="http-request"></a><span data-ttu-id="92a01-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="92a01-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /organization
```

## <a name="optional-query-parameters"></a><span data-ttu-id="92a01-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="92a01-121">Optional query parameters</span></span>

<span data-ttu-id="92a01-122">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="92a01-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="92a01-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="92a01-123">Request headers</span></span>

| <span data-ttu-id="92a01-124">Nome</span><span class="sxs-lookup"><span data-stu-id="92a01-124">Name</span></span>       | <span data-ttu-id="92a01-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="92a01-125">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="92a01-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="92a01-126">Authorization</span></span>  | <span data-ttu-id="92a01-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="92a01-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="92a01-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="92a01-129">Request body</span></span>

<span data-ttu-id="92a01-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="92a01-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="92a01-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="92a01-131">Response</span></span>

<span data-ttu-id="92a01-132">Se bem sucedido, este método retorna um código de resposta `200 OK` e uma coleção de um objeto de [organização](../resources/organization.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="92a01-132">If successful, this method returns a `200 OK` response code and a collection of one [organization](../resources/organization.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="92a01-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="92a01-133">Example</span></span>

##### <a name="request"></a><span data-ttu-id="92a01-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="92a01-134">Request</span></span>

<span data-ttu-id="92a01-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="92a01-135">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="92a01-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="92a01-136">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_organization"
}-->

```http
GET https://graph.microsoft.com/v1.0/organization
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="92a01-137">C#</span><span class="sxs-lookup"><span data-stu-id="92a01-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-organization-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="92a01-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="92a01-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-organization-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="92a01-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="92a01-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-organization-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="92a01-140">Java</span><span class="sxs-lookup"><span data-stu-id="92a01-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-organization-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="92a01-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="92a01-141">Response</span></span>

<span data-ttu-id="92a01-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="92a01-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organization"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 411

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#organization",
  "value": [
    {
      "assignedPlans": [
        {
          "assignedDateTime": "datetime-value",
          "capabilityStatus": "capabilityStatus-value",
          "service": "service-value",
          "servicePlanId": "servicePlanId-value"
        }
      ],
      "businessPhones": [
        "businessPhones-value"
      ],
      "city": "city-value",
      "country": "country-value",
      "countryLetterCode": "countryLetterCode-value",
      "displayName": "displayName-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get organization",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
