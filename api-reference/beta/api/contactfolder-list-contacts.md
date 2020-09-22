---
title: Listar contatos
description: Obter todos os contatos na caixa de correio do usuário conectado (. ../me/Contacts) ou a pasta de contatos especificada.
localization_priority: Normal
author: kevinbellinger
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: fa660186ea9cdb34ba6586a1e932f740d51e5d26
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48002923"
---
# <a name="list-contacts"></a><span data-ttu-id="63be2-103">Listar contatos</span><span class="sxs-lookup"><span data-stu-id="63be2-103">List contacts</span></span>

<span data-ttu-id="63be2-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="63be2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="63be2-105">Obter todos os contatos na caixa de correio do usuário conectado (. ../me/Contacts) ou a pasta de contatos especificada.</span><span class="sxs-lookup"><span data-stu-id="63be2-105">Get all the contacts in the signed-in user's mailbox (.../me/contacts), or from the specified contact folder.</span></span>

## <a name="permissions"></a><span data-ttu-id="63be2-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="63be2-106">Permissions</span></span>
<span data-ttu-id="63be2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="63be2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="63be2-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="63be2-109">Permission type</span></span>      | <span data-ttu-id="63be2-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="63be2-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="63be2-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="63be2-111">Delegated (work or school account)</span></span> | <span data-ttu-id="63be2-112">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="63be2-112">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="63be2-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="63be2-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="63be2-114">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="63be2-114">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="63be2-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="63be2-115">Application</span></span> | <span data-ttu-id="63be2-116">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="63be2-116">Contacts.Read, Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="63be2-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="63be2-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contacts
GET /users/{id | userPrincipalName}/contacts

GET /me/contactFolders/{id}/contacts
GET /users/{id | userPrincipalName}/contactFolders/{id}/contacts
```
## <a name="optional-query-parameters"></a><span data-ttu-id="63be2-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="63be2-118">Optional query parameters</span></span>
<span data-ttu-id="63be2-119">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="63be2-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="63be2-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="63be2-120">Request headers</span></span>
| <span data-ttu-id="63be2-121">Nome</span><span class="sxs-lookup"><span data-stu-id="63be2-121">Name</span></span>       | <span data-ttu-id="63be2-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="63be2-122">Type</span></span> | <span data-ttu-id="63be2-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="63be2-123">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="63be2-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="63be2-124">Authorization</span></span>  | <span data-ttu-id="63be2-125">string</span><span class="sxs-lookup"><span data-stu-id="63be2-125">string</span></span>  | <span data-ttu-id="63be2-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="63be2-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="63be2-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="63be2-128">Request body</span></span>
<span data-ttu-id="63be2-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="63be2-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="63be2-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="63be2-130">Response</span></span>

<span data-ttu-id="63be2-131">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [Contact](../resources/contact.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="63be2-131">If successful, this method returns a `200 OK` response code and collection of [Contact](../resources/contact.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="63be2-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="63be2-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="63be2-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="63be2-133">Request</span></span>
<span data-ttu-id="63be2-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="63be2-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="63be2-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="63be2-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "contactfolder_get_contacts"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/contactFolders/{id}/contacts
```
# <a name="c"></a>[<span data-ttu-id="63be2-136">C#</span><span class="sxs-lookup"><span data-stu-id="63be2-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/contactfolder-get-contacts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="63be2-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="63be2-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/contactfolder-get-contacts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="63be2-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="63be2-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/contactfolder-get-contacts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="63be2-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="63be2-139">Response</span></span>
<span data-ttu-id="63be2-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="63be2-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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


