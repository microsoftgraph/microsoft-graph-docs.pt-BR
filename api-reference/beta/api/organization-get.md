---
title: Obter organização
description: Recupere as propriedades e os relacionamentos da organização autenticada no momento.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 92305dc6e4caffd2deccb8902b68e24d4fbde51d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35988808"
---
# <a name="get-organization"></a><span data-ttu-id="852a3-103">Obter organização</span><span class="sxs-lookup"><span data-stu-id="852a3-103">Get organization</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="852a3-104">Obtenha as propriedades e os relacionamentos da organização autenticada no momento.</span><span class="sxs-lookup"><span data-stu-id="852a3-104">Get the properties and relationships of the currently authenticated organization.</span></span>

<span data-ttu-id="852a3-105">Como o recurso de **organização** suporta [extensões](/graph/extensibility-overview), você também pode usar `GET` a operação para obter propriedades personalizadas e dados de extensão em uma instância de **organização** .</span><span class="sxs-lookup"><span data-stu-id="852a3-105">Since the **organization** resource supports [extensions](/graph/extensibility-overview), you can also use the `GET` operation to get custom properties and extension data in an **organization** instance.</span></span>

## <a name="permissions"></a><span data-ttu-id="852a3-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="852a3-106">Permissions</span></span>

<span data-ttu-id="852a3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="852a3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="852a3-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="852a3-109">Permission type</span></span> | <span data-ttu-id="852a3-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="852a3-110">Permissions (from least to most privileged)</span></span> |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="852a3-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="852a3-111">Delegated (work or school account)</span></span> | <span data-ttu-id="852a3-112">User. Read, Organization. Read. All, Directory. Read. All, Organization. ReadWrite. All, Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="852a3-112">User.Read, Organization.Read.All, Directory.Read.All, Organization.ReadWrite.All, Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="852a3-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="852a3-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="852a3-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="852a3-114">Not supported.</span></span> |
|<span data-ttu-id="852a3-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="852a3-115">Application</span></span> | <span data-ttu-id="852a3-116">Organization. Read. All, Directory. Read. All, Organization. ReadWrite. All, Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="852a3-116">Organization.Read.All, Directory.Read.All, Organization.ReadWrite.All, Directory.ReadWrite.All</span></span> |

> <span data-ttu-id="852a3-117">**Observação**: os aplicativos que receberam a permissão User. Read podem ler apenas as propriedades **ID**, **DisplayName**e **verifiedDomains** da organização.</span><span class="sxs-lookup"><span data-stu-id="852a3-117">**Note**: Applications granted the User.Read permission are able to read only the **id**, **displayName**, and **verifiedDomains** properties of the organization.</span></span>  <span data-ttu-id="852a3-118">Todas as outras propriedades retornarão valores `null`.</span><span class="sxs-lookup"><span data-stu-id="852a3-118">All other properties will return with `null` values.</span></span> <span data-ttu-id="852a3-119">Para ler todas as propriedades, use Organization. Read. All.</span><span class="sxs-lookup"><span data-stu-id="852a3-119">To read all properties, use Organization.Read.All.</span></span>

## <a name="http-request"></a><span data-ttu-id="852a3-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="852a3-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /organization
```

## <a name="optional-query-parameters"></a><span data-ttu-id="852a3-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="852a3-121">Optional query parameters</span></span>

<span data-ttu-id="852a3-122">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="852a3-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="852a3-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="852a3-123">Request headers</span></span>

| <span data-ttu-id="852a3-124">Nome</span><span class="sxs-lookup"><span data-stu-id="852a3-124">Name</span></span>       | <span data-ttu-id="852a3-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="852a3-125">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="852a3-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="852a3-126">Authorization</span></span>  | <span data-ttu-id="852a3-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="852a3-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="852a3-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="852a3-129">Request body</span></span>

<span data-ttu-id="852a3-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="852a3-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="852a3-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="852a3-131">Response</span></span>

<span data-ttu-id="852a3-132">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [organization](../resources/organization.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="852a3-132">If successful, this method returns a `200 OK` response code and [organization](../resources/organization.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="852a3-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="852a3-133">Example</span></span>

##### <a name="request"></a><span data-ttu-id="852a3-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="852a3-134">Request</span></span>

<span data-ttu-id="852a3-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="852a3-135">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="852a3-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="852a3-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_organization"
}-->

```http
GET https://graph.microsoft.com/beta/organization
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="852a3-137">C#</span><span class="sxs-lookup"><span data-stu-id="852a3-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-organization-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="852a3-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="852a3-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-organization-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="852a3-139">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="852a3-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-organization-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="852a3-140">Java</span><span class="sxs-lookup"><span data-stu-id="852a3-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-organization-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="852a3-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="852a3-141">Response</span></span>

<span data-ttu-id="852a3-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="852a3-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="852a3-145">Confira também</span><span class="sxs-lookup"><span data-stu-id="852a3-145">See also</span></span>

- [<span data-ttu-id="852a3-146">Adicionar dados personalizados a recursos usando extensões</span><span class="sxs-lookup"><span data-stu-id="852a3-146">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="852a3-147">Adicionar dados personalizados aos usuários usando extensões abertas (visualização)</span><span class="sxs-lookup"><span data-stu-id="852a3-147">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
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
