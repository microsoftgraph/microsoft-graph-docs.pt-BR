---
title: Listar contatos
description: Obter todos os contatos na caixa de correio do usuário conectado (. ../me/Contacts) ou a pasta de contatos especificada.
localization_priority: Normal
author: kevinbellinger
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 5d3013bef0b24e48c850af9b664d829d6ce792c4
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43381912"
---
# <a name="list-contacts"></a><span data-ttu-id="adad9-103">Listar contatos</span><span class="sxs-lookup"><span data-stu-id="adad9-103">List contacts</span></span>

<span data-ttu-id="adad9-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="adad9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="adad9-105">Obter todos os contatos na caixa de correio do usuário conectado (. ../me/Contacts) ou a pasta de contatos especificada.</span><span class="sxs-lookup"><span data-stu-id="adad9-105">Get all the contacts in the signed-in user's mailbox (.../me/contacts), or from the specified contact folder.</span></span>

## <a name="permissions"></a><span data-ttu-id="adad9-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="adad9-106">Permissions</span></span>
<span data-ttu-id="adad9-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="adad9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="adad9-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="adad9-109">Permission type</span></span>      | <span data-ttu-id="adad9-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="adad9-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="adad9-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="adad9-111">Delegated (work or school account)</span></span> | <span data-ttu-id="adad9-112">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="adad9-112">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="adad9-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="adad9-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="adad9-114">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="adad9-114">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="adad9-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="adad9-115">Application</span></span> | <span data-ttu-id="adad9-116">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="adad9-116">Contacts.Read, Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="adad9-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="adad9-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contacts
GET /users/{id | userPrincipalName}/contacts

GET /me/contactFolders/{id}/contacts
GET /users/{id | userPrincipalName}/contactFolders/{id}/contacts
```
## <a name="optional-query-parameters"></a><span data-ttu-id="adad9-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="adad9-118">Optional query parameters</span></span>
<span data-ttu-id="adad9-119">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="adad9-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="adad9-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="adad9-120">Request headers</span></span>
| <span data-ttu-id="adad9-121">Nome</span><span class="sxs-lookup"><span data-stu-id="adad9-121">Name</span></span>       | <span data-ttu-id="adad9-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="adad9-122">Type</span></span> | <span data-ttu-id="adad9-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="adad9-123">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="adad9-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="adad9-124">Authorization</span></span>  | <span data-ttu-id="adad9-125">string</span><span class="sxs-lookup"><span data-stu-id="adad9-125">string</span></span>  | <span data-ttu-id="adad9-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="adad9-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="adad9-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="adad9-128">Request body</span></span>
<span data-ttu-id="adad9-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="adad9-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="adad9-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="adad9-130">Response</span></span>

<span data-ttu-id="adad9-131">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [Contact](../resources/contact.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="adad9-131">If successful, this method returns a `200 OK` response code and collection of [Contact](../resources/contact.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="adad9-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="adad9-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="adad9-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="adad9-133">Request</span></span>
<span data-ttu-id="adad9-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="adad9-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="adad9-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="adad9-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "contactfolder_get_contacts"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/contactFolders/{id}/contacts
```
# <a name="c"></a>[<span data-ttu-id="adad9-136">C#</span><span class="sxs-lookup"><span data-stu-id="adad9-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/contactfolder-get-contacts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="adad9-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="adad9-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/contactfolder-get-contacts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="adad9-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="adad9-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/contactfolder-get-contacts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="adad9-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="adad9-139">Response</span></span>
<span data-ttu-id="adad9-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="adad9-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
