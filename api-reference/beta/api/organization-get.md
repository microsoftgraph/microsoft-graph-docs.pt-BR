---
title: Obter organização
description: Recupere as propriedades e os relacionamentos da organização autenticada no momento.
localization_priority: Normal
author: adimitui
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 5ce4fef8055c06e8575132efafc9fe2a80601ff6
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50955840"
---
# <a name="get-organization"></a><span data-ttu-id="613ac-103">Obter organização</span><span class="sxs-lookup"><span data-stu-id="613ac-103">Get organization</span></span>

<span data-ttu-id="613ac-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="613ac-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="613ac-105">Obtenha as propriedades e relações da organização autenticada no momento.</span><span class="sxs-lookup"><span data-stu-id="613ac-105">Get the properties and relationships of the currently authenticated organization.</span></span>

<span data-ttu-id="613ac-106">Como o recurso da **organização** tem suporte para [extensões](/graph/extensibility-overview), você também pode usar a operação `GET` para obter propriedades personalizadas e dados de extensão em uma instância de **organização**.</span><span class="sxs-lookup"><span data-stu-id="613ac-106">Since the **organization** resource supports [extensions](/graph/extensibility-overview), you can also use the `GET` operation to get custom properties and extension data in an **organization** instance.</span></span>

## <a name="permissions"></a><span data-ttu-id="613ac-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="613ac-107">Permissions</span></span>

<span data-ttu-id="613ac-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="613ac-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="613ac-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="613ac-110">Permission type</span></span> | <span data-ttu-id="613ac-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="613ac-111">Permissions (from least to most privileged)</span></span> |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="613ac-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="613ac-112">Delegated (work or school account)</span></span> | <span data-ttu-id="613ac-113">User.Read, Organization.Read.All, Directory.Read.All, Organization.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="613ac-113">User.Read, Organization.Read.All, Directory.Read.All, Organization.ReadWrite.All, Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="613ac-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="613ac-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="613ac-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="613ac-115">Not supported.</span></span> |
|<span data-ttu-id="613ac-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="613ac-116">Application</span></span> | <span data-ttu-id="613ac-117">Organization.Read.All, Directory.Read.All, Organization.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="613ac-117">Organization.Read.All, Directory.Read.All, Organization.ReadWrite.All, Directory.ReadWrite.All</span></span> |

> <span data-ttu-id="613ac-118">**Observação**: Os aplicativos que tem a permissão User.Read só conseguem ler as propriedades **id**, **displayName** e **verifiedDomains** da organização.</span><span class="sxs-lookup"><span data-stu-id="613ac-118">**Note**: Applications granted the User.Read permission are able to read only the **id**, **displayName**, and **verifiedDomains** properties of the organization.</span></span>  <span data-ttu-id="613ac-119">Todas as outras propriedades retornarão valores `null`.</span><span class="sxs-lookup"><span data-stu-id="613ac-119">All other properties will return with `null` values.</span></span> <span data-ttu-id="613ac-120">Para ler todas as propriedades, use Organization.Read.All.</span><span class="sxs-lookup"><span data-stu-id="613ac-120">To read all properties, use Organization.Read.All.</span></span>

## <a name="http-request"></a><span data-ttu-id="613ac-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="613ac-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /organization
```

## <a name="optional-query-parameters"></a><span data-ttu-id="613ac-122">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="613ac-122">Optional query parameters</span></span>

<span data-ttu-id="613ac-123">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="613ac-123">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="613ac-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="613ac-124">Request headers</span></span>

| <span data-ttu-id="613ac-125">Nome</span><span class="sxs-lookup"><span data-stu-id="613ac-125">Name</span></span>       | <span data-ttu-id="613ac-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="613ac-126">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="613ac-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="613ac-127">Authorization</span></span>  | <span data-ttu-id="613ac-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="613ac-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="613ac-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="613ac-130">Request body</span></span>

<span data-ttu-id="613ac-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="613ac-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="613ac-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="613ac-132">Response</span></span>

<span data-ttu-id="613ac-133">Se bem sucedido, este método retorna um código de resposta `200 OK` e uma coleção de um objeto de [organização](../resources/organization.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="613ac-133">If successful, this method returns a `200 OK` response code and a collection of one [organization](../resources/organization.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="613ac-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="613ac-134">Example</span></span>

##### <a name="request"></a><span data-ttu-id="613ac-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="613ac-135">Request</span></span>

<span data-ttu-id="613ac-136">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="613ac-136">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="613ac-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="613ac-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_organization_1"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/organization
```
# <a name="c"></a>[<span data-ttu-id="613ac-138">C#</span><span class="sxs-lookup"><span data-stu-id="613ac-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-organization-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="613ac-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="613ac-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-organization-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="613ac-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="613ac-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-organization-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="613ac-141">Java</span><span class="sxs-lookup"><span data-stu-id="613ac-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-organization-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="613ac-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="613ac-142">Response</span></span>

<span data-ttu-id="613ac-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="613ac-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="613ac-146">Confira também</span><span class="sxs-lookup"><span data-stu-id="613ac-146">See also</span></span>

- [<span data-ttu-id="613ac-147">Adicionar dados personalizados a recursos usando extensões</span><span class="sxs-lookup"><span data-stu-id="613ac-147">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="613ac-148">Adicionar dados personalizados aos usuários usando extensões abertas (visualização)</span><span class="sxs-lookup"><span data-stu-id="613ac-148">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
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
