---
title: Listar memberOf
description: Listar os grupos dos que esse contato organizaitonal é membro.
localization_priority: Normal
author: dkershaw10
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 5eec725428c80c79ef15e195c9d9459a9b97571d
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52039255"
---
# <a name="list-memberof"></a><span data-ttu-id="dcc44-103">Listar memberOf</span><span class="sxs-lookup"><span data-stu-id="dcc44-103">List memberOf</span></span>

<span data-ttu-id="dcc44-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dcc44-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="dcc44-105">Listar os grupos dos que [esse contato](../resources/orgcontact.md) organizacional é membro.</span><span class="sxs-lookup"><span data-stu-id="dcc44-105">List the groups that this [organizational contact](../resources/orgcontact.md) is a member of.</span></span>

## <a name="permissions"></a><span data-ttu-id="dcc44-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="dcc44-106">Permissions</span></span>
<span data-ttu-id="dcc44-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dcc44-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dcc44-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="dcc44-109">Permission type</span></span>      | <span data-ttu-id="dcc44-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="dcc44-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dcc44-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="dcc44-111">Delegated (work or school account)</span></span> | <span data-ttu-id="dcc44-112">OrgContact.Read.All e Group.Read.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="dcc44-112">OrgContact.Read.All and Group.Read.All, Directory.Read.All</span></span>  |
|<span data-ttu-id="dcc44-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="dcc44-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dcc44-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dcc44-114">Not supported.</span></span>    |
|<span data-ttu-id="dcc44-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="dcc44-115">Application</span></span> | <span data-ttu-id="dcc44-116">OrgContact.Read.All e Group.Read.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="dcc44-116">OrgContact.Read.All and Group.Read.All, Directory.Read.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="dcc44-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="dcc44-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /contacts/{id}/memberOf
```
## <a name="optional-query-parameters"></a><span data-ttu-id="dcc44-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="dcc44-118">Optional query parameters</span></span>
<span data-ttu-id="dcc44-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) `$select` para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="dcc44-119">This method supports the [OData Query Parameters](/graph/query-parameters) `$select` to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="dcc44-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="dcc44-120">Request headers</span></span>
| <span data-ttu-id="dcc44-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="dcc44-121">Header</span></span>       | <span data-ttu-id="dcc44-122">Valor</span><span class="sxs-lookup"><span data-stu-id="dcc44-122">Value</span></span> |
|:-----------|:----------|
| <span data-ttu-id="dcc44-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="dcc44-123">Authorization</span></span>  | <span data-ttu-id="dcc44-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dcc44-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="dcc44-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="dcc44-126">Request body</span></span>
<span data-ttu-id="dcc44-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="dcc44-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dcc44-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="dcc44-128">Response</span></span>

<span data-ttu-id="dcc44-129">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="dcc44-129">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="dcc44-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="dcc44-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="dcc44-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dcc44-131">Request</span></span>
<span data-ttu-id="dcc44-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="dcc44-132">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="dcc44-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="dcc44-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "contact_get_memberof"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/contacts/{id}/memberOf
```
# <a name="c"></a>[<span data-ttu-id="dcc44-134">C#</span><span class="sxs-lookup"><span data-stu-id="dcc44-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/contact-get-memberof-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="dcc44-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="dcc44-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/contact-get-memberof-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="dcc44-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="dcc44-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/contact-get-memberof-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="dcc44-137">Java</span><span class="sxs-lookup"><span data-stu-id="dcc44-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/contact-get-memberof-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="dcc44-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="dcc44-138">Response</span></span>
<span data-ttu-id="dcc44-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="dcc44-139">The following is an example of the response.</span></span>
><span data-ttu-id="dcc44-140">**Observação**: o objeto de resposta mostrado aqui pode ser encurtado com fins de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="dcc44-140">**Note**: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 155

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.group",
      "id": "024bbfa0-fe5a-4fce-9227-bd6ccf1324bb",
      "createdDateTime": "2018-01-18T18:54:43Z",
      "description": "Best group ever created",
      "displayName": "Best Group",
      "groupTypes": [],
      "isAssignableToRole": null,
      "onPremisesProvisioningErrors": []
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List memberOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
