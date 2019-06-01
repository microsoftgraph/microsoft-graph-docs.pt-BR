---
title: Obter organização
description: Recupere as propriedades e os relacionamentos da organização autenticada no momento.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 54e5db4b3c8c0c279ef618e27911b8460a5669eb
ms.sourcegitcommit: 33f1cf5b3b79bfba6a06b52d34e558a6ba327d21
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2019
ms.locfileid: "34657298"
---
# <a name="get-organization"></a><span data-ttu-id="23045-103">Obter organização</span><span class="sxs-lookup"><span data-stu-id="23045-103">Get organization</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="23045-104">Recupere as propriedades e os relacionamentos da organização autenticada no momento.</span><span class="sxs-lookup"><span data-stu-id="23045-104">Retrieve the properties and relationships of currently authenticated organization.</span></span>

<span data-ttu-id="23045-105">Como o recurso de **organização** suporta [extensões](/graph/extensibility-overview), você também pode usar `GET` a operação para obter propriedades personalizadas e dados de extensão em uma instância de **organização** .</span><span class="sxs-lookup"><span data-stu-id="23045-105">Since the **organization** resource supports [extensions](/graph/extensibility-overview), you can also use the `GET` operation to get custom properties and extension data in an **organization** instance.</span></span>

## <a name="permissions"></a><span data-ttu-id="23045-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="23045-106">Permissions</span></span>

<span data-ttu-id="23045-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="23045-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="23045-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="23045-109">Permission type</span></span> | <span data-ttu-id="23045-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="23045-110">Permissions (from least to most privileged)</span></span> |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="23045-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="23045-111">Delegated (work or school account)</span></span> | <span data-ttu-id="23045-112">User. Read, Directory. Read. All</span><span class="sxs-lookup"><span data-stu-id="23045-112">User.Read, Directory.Read.All</span></span> |
|<span data-ttu-id="23045-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="23045-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="23045-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="23045-114">Not supported.</span></span> |
|<span data-ttu-id="23045-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="23045-115">Application</span></span> | <span data-ttu-id="23045-116">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="23045-116">Directory.Read.All</span></span> |

> <span data-ttu-id="23045-117">Observação: os aplicativos que têm a permissão User.Read só conseguem ler as propriedades *id*, *displayName* e *verifiedDomains* da organização.</span><span class="sxs-lookup"><span data-stu-id="23045-117">Note: Applications granted the User.Read permission are able to read only the *id*, *displayName*, and *verifiedDomains* properties of the organization.</span></span>  <span data-ttu-id="23045-118">Todas as outras propriedades retornarão valores `null`.</span><span class="sxs-lookup"><span data-stu-id="23045-118">All other properties will return with `null` values.</span></span> <span data-ttu-id="23045-119">Para ler todas as propriedades, use Directory.Read.All.</span><span class="sxs-lookup"><span data-stu-id="23045-119">To read all properties, use Directory.Read.All.</span></span>

## <a name="http-request"></a><span data-ttu-id="23045-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="23045-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /organization
```

## <a name="optional-query-parameters"></a><span data-ttu-id="23045-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="23045-121">Optional query parameters</span></span>

<span data-ttu-id="23045-122">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="23045-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="23045-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="23045-123">Request headers</span></span>

| <span data-ttu-id="23045-124">Nome</span><span class="sxs-lookup"><span data-stu-id="23045-124">Name</span></span>       | <span data-ttu-id="23045-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="23045-125">Type</span></span> | <span data-ttu-id="23045-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="23045-126">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="23045-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="23045-127">Authorization</span></span>  | <span data-ttu-id="23045-128">string</span><span class="sxs-lookup"><span data-stu-id="23045-128">string</span></span>  | <span data-ttu-id="23045-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="23045-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="23045-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="23045-131">Request body</span></span>

<span data-ttu-id="23045-132">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="23045-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="23045-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="23045-133">Response</span></span>

<span data-ttu-id="23045-134">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [organization](../resources/organization.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="23045-134">If successful, this method returns a `200 OK` response code and [organization](../resources/organization.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="23045-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="23045-135">Example</span></span>

##### <a name="request"></a><span data-ttu-id="23045-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="23045-136">Request</span></span>

<span data-ttu-id="23045-137">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="23045-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_organization"
}-->

```http
GET https://graph.microsoft.com/beta/organization
```

##### <a name="response"></a><span data-ttu-id="23045-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="23045-138">Response</span></span>

<span data-ttu-id="23045-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="23045-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="23045-142">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="23045-142">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="23045-143">C#</span><span class="sxs-lookup"><span data-stu-id="23045-143">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_organization-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="23045-144">Javascript</span><span class="sxs-lookup"><span data-stu-id="23045-144">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_organization-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="see-also"></a><span data-ttu-id="23045-145">Confira também</span><span class="sxs-lookup"><span data-stu-id="23045-145">See also</span></span>

- [<span data-ttu-id="23045-146">Adicionar dados personalizados a recursos usando extensões</span><span class="sxs-lookup"><span data-stu-id="23045-146">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="23045-147">Adicionar dados personalizados aos usuários usando extensões abertas (visualização)</span><span class="sxs-lookup"><span data-stu-id="23045-147">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
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
    "Error: /api-reference/beta/api/organization-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/organization-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
