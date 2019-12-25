---
title: Listar memberOf
description: Lista os grupos dos quais este contato do organizaitonal é membro.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 8a9727f19f8c108203f4341fb864d4776cf24101
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "40865542"
---
# <a name="list-memberof"></a><span data-ttu-id="8e89e-103">Listar memberOf</span><span class="sxs-lookup"><span data-stu-id="8e89e-103">List memberOf</span></span>

<span data-ttu-id="8e89e-104">Lista os grupos dos quais esse [contato organizacional](../resources/orgcontact.md) é membro.</span><span class="sxs-lookup"><span data-stu-id="8e89e-104">List the groups that this [organizational contact](../resources/orgcontact.md) is a member of.</span></span>

## <a name="permissions"></a><span data-ttu-id="8e89e-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="8e89e-105">Permissions</span></span>
<span data-ttu-id="8e89e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8e89e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8e89e-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8e89e-108">Permission type</span></span>      | <span data-ttu-id="8e89e-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8e89e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8e89e-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8e89e-110">Delegated (work or school account)</span></span> | <span data-ttu-id="8e89e-111">OrgContact. Read. All e Group. Read. All, Directory. Read. All</span><span class="sxs-lookup"><span data-stu-id="8e89e-111">OrgContact.Read.All and Group.Read.All, Directory.Read.All</span></span>  |
|<span data-ttu-id="8e89e-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8e89e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8e89e-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8e89e-113">Not supported.</span></span>    |
|<span data-ttu-id="8e89e-114">Application</span><span class="sxs-lookup"><span data-stu-id="8e89e-114">Application</span></span> | <span data-ttu-id="8e89e-115">OrgContact. Read. All e Group. Read. All, Directory. Read. All</span><span class="sxs-lookup"><span data-stu-id="8e89e-115">OrgContact.Read.All and Group.Read.All, Directory.Read.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="8e89e-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8e89e-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /contacts/{id}/memberOf
```
## <a name="optional-query-parameters"></a><span data-ttu-id="8e89e-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="8e89e-117">Optional query parameters</span></span>
<span data-ttu-id="8e89e-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) `$select` para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="8e89e-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) `$select` to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8e89e-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8e89e-119">Request headers</span></span>
| <span data-ttu-id="8e89e-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8e89e-120">Header</span></span>       | <span data-ttu-id="8e89e-121">Valor</span><span class="sxs-lookup"><span data-stu-id="8e89e-121">Value</span></span> |
|:-----------|:----------|
| <span data-ttu-id="8e89e-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="8e89e-122">Authorization</span></span>  | <span data-ttu-id="8e89e-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8e89e-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8e89e-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8e89e-125">Request body</span></span>
<span data-ttu-id="8e89e-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="8e89e-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8e89e-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="8e89e-127">Response</span></span>

<span data-ttu-id="8e89e-128">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8e89e-128">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="8e89e-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8e89e-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8e89e-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8e89e-130">Request</span></span>
<span data-ttu-id="8e89e-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="8e89e-131">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="8e89e-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="8e89e-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "contact_get_memberof"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/contacts/{id}/memberOf
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="8e89e-133">C#</span><span class="sxs-lookup"><span data-stu-id="8e89e-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/contact-get-memberof-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8e89e-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8e89e-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/contact-get-memberof-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="8e89e-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8e89e-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/contact-get-memberof-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="8e89e-136">Java</span><span class="sxs-lookup"><span data-stu-id="8e89e-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/contact-get-memberof-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="8e89e-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="8e89e-137">Response</span></span>
<span data-ttu-id="8e89e-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="8e89e-138">The following is an example of the response.</span></span>
><span data-ttu-id="8e89e-139">**Observação**: o objeto de resposta mostrado aqui pode ser encurtado com fins de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="8e89e-139">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="8e89e-140">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8e89e-140">All the properties will be returned from an actual call.</span></span>
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
