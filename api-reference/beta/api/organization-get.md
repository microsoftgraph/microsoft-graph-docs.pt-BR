---
title: Obter organização
description: Recupere as propriedades e os relacionamentos da organização autenticada no momento.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 4e0105a5a81a754beab637fe2199dd7e5bf5d6a7
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35450566"
---
# <a name="get-organization"></a><span data-ttu-id="509da-103">Obter organização</span><span class="sxs-lookup"><span data-stu-id="509da-103">Get organization</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="509da-104">Recupere as propriedades e os relacionamentos da organização autenticada no momento.</span><span class="sxs-lookup"><span data-stu-id="509da-104">Retrieve the properties and relationships of currently authenticated organization.</span></span>

<span data-ttu-id="509da-105">Como o recurso de **organização** suporta [extensões](/graph/extensibility-overview), você também pode usar `GET` a operação para obter propriedades personalizadas e dados de extensão em uma instância de **organização** .</span><span class="sxs-lookup"><span data-stu-id="509da-105">Since the **organization** resource supports [extensions](/graph/extensibility-overview), you can also use the `GET` operation to get custom properties and extension data in an **organization** instance.</span></span>

## <a name="permissions"></a><span data-ttu-id="509da-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="509da-106">Permissions</span></span>

<span data-ttu-id="509da-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="509da-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="509da-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="509da-109">Permission type</span></span> | <span data-ttu-id="509da-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="509da-110">Permissions (from least to most privileged)</span></span> |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="509da-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="509da-111">Delegated (work or school account)</span></span> | <span data-ttu-id="509da-112">User. Read, Directory. Read. All</span><span class="sxs-lookup"><span data-stu-id="509da-112">User.Read, Directory.Read.All</span></span> |
|<span data-ttu-id="509da-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="509da-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="509da-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="509da-114">Not supported.</span></span> |
|<span data-ttu-id="509da-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="509da-115">Application</span></span> | <span data-ttu-id="509da-116">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="509da-116">Directory.Read.All</span></span> |

> <span data-ttu-id="509da-117">Observação: os aplicativos que têm a permissão User.Read só conseguem ler as propriedades *id*, *displayName* e *verifiedDomains* da organização.</span><span class="sxs-lookup"><span data-stu-id="509da-117">Note: Applications granted the User.Read permission are able to read only the *id*, *displayName*, and *verifiedDomains* properties of the organization.</span></span>  <span data-ttu-id="509da-118">Todas as outras propriedades retornarão valores `null`.</span><span class="sxs-lookup"><span data-stu-id="509da-118">All other properties will return with `null` values.</span></span> <span data-ttu-id="509da-119">Para ler todas as propriedades, use Directory.Read.All.</span><span class="sxs-lookup"><span data-stu-id="509da-119">To read all properties, use Directory.Read.All.</span></span>

## <a name="http-request"></a><span data-ttu-id="509da-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="509da-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /organization
```

## <a name="optional-query-parameters"></a><span data-ttu-id="509da-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="509da-121">Optional query parameters</span></span>

<span data-ttu-id="509da-122">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="509da-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="509da-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="509da-123">Request headers</span></span>

| <span data-ttu-id="509da-124">Nome</span><span class="sxs-lookup"><span data-stu-id="509da-124">Name</span></span>       | <span data-ttu-id="509da-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="509da-125">Type</span></span> | <span data-ttu-id="509da-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="509da-126">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="509da-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="509da-127">Authorization</span></span>  | <span data-ttu-id="509da-128">string</span><span class="sxs-lookup"><span data-stu-id="509da-128">string</span></span>  | <span data-ttu-id="509da-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="509da-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="509da-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="509da-131">Request body</span></span>

<span data-ttu-id="509da-132">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="509da-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="509da-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="509da-133">Response</span></span>

<span data-ttu-id="509da-134">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [organization](../resources/organization.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="509da-134">If successful, this method returns a `200 OK` response code and [organization](../resources/organization.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="509da-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="509da-135">Example</span></span>

##### <a name="request"></a><span data-ttu-id="509da-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="509da-136">Request</span></span>

<span data-ttu-id="509da-137">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="509da-137">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="509da-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="509da-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_organization"
}-->

```http
GET https://graph.microsoft.com/beta/organization
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="509da-139">C#</span><span class="sxs-lookup"><span data-stu-id="509da-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-organization-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="509da-140">Javascript</span><span class="sxs-lookup"><span data-stu-id="509da-140">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-organization-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="509da-141">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="509da-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-organization-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="509da-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="509da-142">Response</span></span>

<span data-ttu-id="509da-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="509da-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#organization",
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

## <a name="see-also"></a><span data-ttu-id="509da-146">Confira também</span><span class="sxs-lookup"><span data-stu-id="509da-146">See also</span></span>

- [<span data-ttu-id="509da-147">Adicionar dados personalizados a recursos usando extensões</span><span class="sxs-lookup"><span data-stu-id="509da-147">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="509da-148">Adicionar dados personalizados aos usuários usando extensões abertas (visualização)</span><span class="sxs-lookup"><span data-stu-id="509da-148">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
<!--
- [Add custom data to groups using schema extensions (preview)](/graph/extensibility-schema-groups)
-->

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get organization",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
