---
title: Listar contatos
description: Obter todos os contatos na caixa de correio do usuário conectado (. ../me/Contacts) ou a pasta de contatos especificada.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 83a555d123888854bd1c2ca301a999ce5e401f06
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35437602"
---
# <a name="list-contacts"></a><span data-ttu-id="b03b2-103">Listar contatos</span><span class="sxs-lookup"><span data-stu-id="b03b2-103">List contacts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b03b2-104">Obter todos os contatos na caixa de correio do usuário conectado (. ../me/Contacts) ou a pasta de contatos especificada.</span><span class="sxs-lookup"><span data-stu-id="b03b2-104">Get all the contacts in the signed-in user's mailbox (.../me/contacts), or from the specified contact folder.</span></span>

## <a name="permissions"></a><span data-ttu-id="b03b2-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="b03b2-105">Permissions</span></span>
<span data-ttu-id="b03b2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b03b2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b03b2-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b03b2-108">Permission type</span></span>      | <span data-ttu-id="b03b2-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b03b2-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b03b2-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b03b2-110">Delegated (work or school account)</span></span> | <span data-ttu-id="b03b2-111">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b03b2-111">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="b03b2-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b03b2-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b03b2-113">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b03b2-113">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="b03b2-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b03b2-114">Application</span></span> | <span data-ttu-id="b03b2-115">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b03b2-115">Contacts.Read, Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="b03b2-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b03b2-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contacts
GET /users/{id | userPrincipalName}/contacts

GET /me/contactFolders/{id}/contacts
GET /users/{id | userPrincipalName}/contactFolders/{id}/contacts
```
## <a name="optional-query-parameters"></a><span data-ttu-id="b03b2-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="b03b2-117">Optional query parameters</span></span>
<span data-ttu-id="b03b2-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="b03b2-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="b03b2-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b03b2-119">Request headers</span></span>
| <span data-ttu-id="b03b2-120">Nome</span><span class="sxs-lookup"><span data-stu-id="b03b2-120">Name</span></span>       | <span data-ttu-id="b03b2-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="b03b2-121">Type</span></span> | <span data-ttu-id="b03b2-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="b03b2-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="b03b2-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="b03b2-123">Authorization</span></span>  | <span data-ttu-id="b03b2-124">string</span><span class="sxs-lookup"><span data-stu-id="b03b2-124">string</span></span>  | <span data-ttu-id="b03b2-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b03b2-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b03b2-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b03b2-127">Request body</span></span>
<span data-ttu-id="b03b2-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b03b2-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b03b2-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="b03b2-129">Response</span></span>

<span data-ttu-id="b03b2-130">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [Contact](../resources/contact.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b03b2-130">If successful, this method returns a `200 OK` response code and collection of [Contact](../resources/contact.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b03b2-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b03b2-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b03b2-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b03b2-132">Request</span></span>
<span data-ttu-id="b03b2-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b03b2-133">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="b03b2-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="b03b2-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_contacts"
}-->
```http
GET https://graph.microsoft.com/beta/me/contactFolders/{id}/contacts
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="b03b2-135">C#</span><span class="sxs-lookup"><span data-stu-id="b03b2-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-contacts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b03b2-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="b03b2-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-contacts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="b03b2-137">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="b03b2-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-contacts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="b03b2-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="b03b2-138">Response</span></span>
<span data-ttu-id="b03b2-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b03b2-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contact",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 263

{
  "value": [
    {
      "parentFolderId": "parentFolderId-value",
      "birthday": "2016-10-19T10:37:00Z",
      "fileAs": "fileAs-value",
      "displayName": "displayName-value",
      "givenName": "givenName-value",
      "initials": "initials-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List contacts",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
