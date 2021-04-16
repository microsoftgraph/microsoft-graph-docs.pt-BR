---
title: Listar organização
description: Recupere uma lista de objetos de organização.
localization_priority: Normal
author: adimitui
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 6eeb6c421f677e31b68d9d5f7de38823883b04e7
ms.sourcegitcommit: be09568fa07ab793cd1db500f537ca94ca9e5b4a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51836946"
---
# <a name="list-organization"></a><span data-ttu-id="97b29-103">Listar organização</span><span class="sxs-lookup"><span data-stu-id="97b29-103">List organization</span></span>

<span data-ttu-id="97b29-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="97b29-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="97b29-105">Recupere uma lista de objetos de organização.</span><span class="sxs-lookup"><span data-stu-id="97b29-105">Retrieve a list of organization objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="97b29-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="97b29-106">Permissions</span></span>
<span data-ttu-id="97b29-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="97b29-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="97b29-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="97b29-109">Permission type</span></span>      | <span data-ttu-id="97b29-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="97b29-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="97b29-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="97b29-111">Delegated (work or school account)</span></span> | <span data-ttu-id="97b29-112">User.Read, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="97b29-112">User.Read, Directory.Read.All, Directory.ReadWrite.All</span></span>   |
|<span data-ttu-id="97b29-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="97b29-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="97b29-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="97b29-114">Not supported.</span></span>    |
|<span data-ttu-id="97b29-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="97b29-115">Application</span></span> | <span data-ttu-id="97b29-116">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="97b29-116">Directory.Read.All, Directory.ReadWrite.All</span></span> |

> <span data-ttu-id="97b29-117">Observação: os aplicativos que têm a permissão User.Read só conseguem ler as propriedades *id*, *displayName* e *verifiedDomains* da organização.</span><span class="sxs-lookup"><span data-stu-id="97b29-117">Note: Applications granted the User.Read permission are able to read only the *id*, *displayName*, and *verifiedDomains* properties of the organization.</span></span>  <span data-ttu-id="97b29-118">Todas as outras propriedades retornarão valores `null`.</span><span class="sxs-lookup"><span data-stu-id="97b29-118">All other properties will return with `null` values.</span></span> <span data-ttu-id="97b29-119">Para ler todas as propriedades, use Directory.Read.All.</span><span class="sxs-lookup"><span data-stu-id="97b29-119">To read all properties, use Directory.Read.All.</span></span>

## <a name="http-request"></a><span data-ttu-id="97b29-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="97b29-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /organization
```
## <a name="optional-query-parameters"></a><span data-ttu-id="97b29-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="97b29-121">Optional query parameters</span></span>
<span data-ttu-id="97b29-122">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="97b29-122">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="97b29-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="97b29-123">Request headers</span></span>
| <span data-ttu-id="97b29-124">Nome</span><span class="sxs-lookup"><span data-stu-id="97b29-124">Name</span></span>       | <span data-ttu-id="97b29-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="97b29-125">Type</span></span> | <span data-ttu-id="97b29-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="97b29-126">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="97b29-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="97b29-127">Authorization</span></span>  | <span data-ttu-id="97b29-128">string</span><span class="sxs-lookup"><span data-stu-id="97b29-128">string</span></span>  | <span data-ttu-id="97b29-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="97b29-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="97b29-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="97b29-131">Request body</span></span>
<span data-ttu-id="97b29-132">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="97b29-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="97b29-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="97b29-133">Response</span></span>

<span data-ttu-id="97b29-134">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [organization](../resources/organization.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="97b29-134">If successful, this method returns a `200 OK` response code and collection of [organization](../resources/organization.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="97b29-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="97b29-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="97b29-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="97b29-136">Request</span></span>
<span data-ttu-id="97b29-137">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="97b29-137">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="97b29-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="97b29-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_organization_2"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/organization
```
# <a name="c"></a>[<span data-ttu-id="97b29-139">C#</span><span class="sxs-lookup"><span data-stu-id="97b29-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-organization-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="97b29-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="97b29-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-organization-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="97b29-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="97b29-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-organization-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="97b29-142">Java</span><span class="sxs-lookup"><span data-stu-id="97b29-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-organization-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="97b29-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="97b29-143">Response</span></span>
<span data-ttu-id="97b29-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="97b29-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organization",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 500

{
  "value": [
    {
      "assignedPlans": [
        {
          "assignedDateTime": "2017-07-29T02:16:28Z",
          "capabilityStatus": "Enabled",
          "service": "SharePoint",
          "servicePlanId": "5dbe027f-2339-4123-9542-606e4d348a72"
        }
      ],
      "businessPhones": [
        "8006427676"
      ],
      "city": "redmond",
      "country": null,
      "countryLetterCode": "US",
      "displayName": "Contoso"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List organization",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
