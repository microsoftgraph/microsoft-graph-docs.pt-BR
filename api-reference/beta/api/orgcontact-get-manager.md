---
title: 'orgContact: Obter gerente'
description: Obter o gerente do contato
localization_priority: Normal
author: dkershaw10
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 6df291504286729737765d375a74fdfd1a725b2e
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50447798"
---
# <a name="orgcontact-get-manager"></a><span data-ttu-id="2d5ac-103">orgContact: Obter gerente</span><span class="sxs-lookup"><span data-stu-id="2d5ac-103">orgContact: Get manager</span></span>

<span data-ttu-id="2d5ac-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2d5ac-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2d5ac-105">Obter o gerente do contato</span><span class="sxs-lookup"><span data-stu-id="2d5ac-105">Get the contact's manager</span></span>

## <a name="permissions"></a><span data-ttu-id="2d5ac-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="2d5ac-106">Permissions</span></span>
<span data-ttu-id="2d5ac-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2d5ac-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2d5ac-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2d5ac-109">Permission type</span></span>      | <span data-ttu-id="2d5ac-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2d5ac-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2d5ac-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2d5ac-111">Delegated (work or school account)</span></span> | <span data-ttu-id="2d5ac-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="2d5ac-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="2d5ac-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2d5ac-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2d5ac-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2d5ac-114">Not supported.</span></span>    |
|<span data-ttu-id="2d5ac-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2d5ac-115">Application</span></span> | <span data-ttu-id="2d5ac-116">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2d5ac-116">Directory.Read.All, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="2d5ac-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2d5ac-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /contacts/{id}/manager
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2d5ac-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="2d5ac-118">Optional query parameters</span></span>
<span data-ttu-id="2d5ac-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="2d5ac-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2d5ac-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2d5ac-120">Request headers</span></span>
| <span data-ttu-id="2d5ac-121">Nome</span><span class="sxs-lookup"><span data-stu-id="2d5ac-121">Name</span></span>       | <span data-ttu-id="2d5ac-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="2d5ac-122">Type</span></span> | <span data-ttu-id="2d5ac-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="2d5ac-123">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="2d5ac-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="2d5ac-124">Authorization</span></span>  | <span data-ttu-id="2d5ac-125">string</span><span class="sxs-lookup"><span data-stu-id="2d5ac-125">string</span></span>  | <span data-ttu-id="2d5ac-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2d5ac-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2d5ac-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2d5ac-128">Request body</span></span>
<span data-ttu-id="2d5ac-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="2d5ac-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2d5ac-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="2d5ac-130">Response</span></span>

<span data-ttu-id="2d5ac-131">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2d5ac-131">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="2d5ac-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2d5ac-132">Example</span></span>

#### <a name="request"></a><span data-ttu-id="2d5ac-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2d5ac-133">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="2d5ac-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="2d5ac-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_manager"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/contacts/{id}/manager
```
# <a name="c"></a>[<span data-ttu-id="2d5ac-135">C#</span><span class="sxs-lookup"><span data-stu-id="2d5ac-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-manager-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2d5ac-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2d5ac-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-manager-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2d5ac-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2d5ac-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-manager-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2d5ac-138">Java</span><span class="sxs-lookup"><span data-stu-id="2d5ac-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-manager-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="2d5ac-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="2d5ac-139">Response</span></span>

<span data-ttu-id="2d5ac-p103">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2d5ac-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
