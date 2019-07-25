---
title: 'orgContact: obter gerente'
description: Obter o gerente do contato
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 16e5da17cc0cd4d1cc6e52c6eaeca04cd5c6fe14
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35877967"
---
# <a name="orgcontact-get-manager"></a><span data-ttu-id="309ba-103">orgContact: obter gerente</span><span class="sxs-lookup"><span data-stu-id="309ba-103">orgContact: Get manager</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="309ba-104">Obter o gerente do contato</span><span class="sxs-lookup"><span data-stu-id="309ba-104">Get the contact's manager</span></span>

## <a name="permissions"></a><span data-ttu-id="309ba-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="309ba-105">Permissions</span></span>
<span data-ttu-id="309ba-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="309ba-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="309ba-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="309ba-108">Permission type</span></span>      | <span data-ttu-id="309ba-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="309ba-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="309ba-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="309ba-110">Delegated (work or school account)</span></span> | <span data-ttu-id="309ba-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="309ba-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="309ba-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="309ba-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="309ba-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="309ba-113">Not supported.</span></span>    |
|<span data-ttu-id="309ba-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="309ba-114">Application</span></span> | <span data-ttu-id="309ba-115">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="309ba-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="309ba-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="309ba-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /contacts/{id}/manager
```

## <a name="optional-query-parameters"></a><span data-ttu-id="309ba-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="309ba-117">Optional query parameters</span></span>
<span data-ttu-id="309ba-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="309ba-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="309ba-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="309ba-119">Request headers</span></span>
| <span data-ttu-id="309ba-120">Nome</span><span class="sxs-lookup"><span data-stu-id="309ba-120">Name</span></span>       | <span data-ttu-id="309ba-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="309ba-121">Type</span></span> | <span data-ttu-id="309ba-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="309ba-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="309ba-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="309ba-123">Authorization</span></span>  | <span data-ttu-id="309ba-124">string</span><span class="sxs-lookup"><span data-stu-id="309ba-124">string</span></span>  | <span data-ttu-id="309ba-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="309ba-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="309ba-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="309ba-127">Request body</span></span>
<span data-ttu-id="309ba-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="309ba-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="309ba-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="309ba-129">Response</span></span>

<span data-ttu-id="309ba-130">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="309ba-130">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="309ba-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="309ba-131">Example</span></span>

#### <a name="request"></a><span data-ttu-id="309ba-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="309ba-132">Request</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="309ba-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="309ba-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_manager"
}-->

```http
GET https://graph.microsoft.com/beta/contacts/{id}/manager
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="309ba-134">C#</span><span class="sxs-lookup"><span data-stu-id="309ba-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-manager-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="309ba-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="309ba-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-manager-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="309ba-136">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="309ba-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-manager-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="309ba-137">Java</span><span class="sxs-lookup"><span data-stu-id="309ba-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-manager-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="309ba-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="309ba-138">Response</span></span>

<span data-ttu-id="309ba-p103">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="309ba-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": false
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 455

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#directoryObjects/$entity",
    "@odata.type": "#microsoft.graph.user",
    "id": "24fcbca3-c3e2-48bf-9ffc-c7f81b81483d",
    "businessPhones": [
        "+1 205 555 0108"
    ],
    "displayName": "Diego Siciliani",
    "givenName": "Diego",
    "jobTitle": "CVP Finance",
    "mail": "DiegoS@contoso.com",
    "mobilePhone": null,
    "officeLocation": "14/1108",
    "preferredLanguage": "en-US",
    "surname": "Siciliani",
    "userPrincipalName": "DiegoS@contoso.com"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get manager",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
