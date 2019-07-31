---
title: Listar contatos
description: Obter todos os contatos na caixa de correio do usuário conectado (. ../me/Contacts) ou a pasta de contatos especificada.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 230fa87233dfb5bfc2fc22cf2d64a4f6131b1ef0
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35943243"
---
# <a name="list-contacts"></a><span data-ttu-id="b1dbf-103">Listar contatos</span><span class="sxs-lookup"><span data-stu-id="b1dbf-103">List contacts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b1dbf-104">Obter todos os contatos na caixa de correio do usuário conectado (. ../me/Contacts) ou a pasta de contatos especificada.</span><span class="sxs-lookup"><span data-stu-id="b1dbf-104">Get all the contacts in the signed-in user's mailbox (.../me/contacts), or from the specified contact folder.</span></span>

## <a name="permissions"></a><span data-ttu-id="b1dbf-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="b1dbf-105">Permissions</span></span>
<span data-ttu-id="b1dbf-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b1dbf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b1dbf-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b1dbf-108">Permission type</span></span>      | <span data-ttu-id="b1dbf-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b1dbf-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b1dbf-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b1dbf-110">Delegated (work or school account)</span></span> | <span data-ttu-id="b1dbf-111">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b1dbf-111">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="b1dbf-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b1dbf-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b1dbf-113">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b1dbf-113">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="b1dbf-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b1dbf-114">Application</span></span> | <span data-ttu-id="b1dbf-115">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b1dbf-115">Contacts.Read, Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="b1dbf-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b1dbf-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contacts
GET /users/{id | userPrincipalName}/contacts

GET /me/contactFolders/{id}/contacts
GET /users/{id | userPrincipalName}/contactFolders/{id}/contacts
```
## <a name="optional-query-parameters"></a><span data-ttu-id="b1dbf-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="b1dbf-117">Optional query parameters</span></span>
<span data-ttu-id="b1dbf-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="b1dbf-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="b1dbf-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b1dbf-119">Request headers</span></span>
| <span data-ttu-id="b1dbf-120">Nome</span><span class="sxs-lookup"><span data-stu-id="b1dbf-120">Name</span></span>       | <span data-ttu-id="b1dbf-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="b1dbf-121">Type</span></span> | <span data-ttu-id="b1dbf-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="b1dbf-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="b1dbf-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="b1dbf-123">Authorization</span></span>  | <span data-ttu-id="b1dbf-124">string</span><span class="sxs-lookup"><span data-stu-id="b1dbf-124">string</span></span>  | <span data-ttu-id="b1dbf-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b1dbf-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b1dbf-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b1dbf-127">Request body</span></span>
<span data-ttu-id="b1dbf-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b1dbf-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b1dbf-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="b1dbf-129">Response</span></span>

<span data-ttu-id="b1dbf-130">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [Contact](../resources/contact.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b1dbf-130">If successful, this method returns a `200 OK` response code and collection of [Contact](../resources/contact.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b1dbf-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b1dbf-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b1dbf-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b1dbf-132">Request</span></span>
<span data-ttu-id="b1dbf-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b1dbf-133">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="b1dbf-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="b1dbf-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "contactfolder_get_contacts"
}-->
```http
GET https://graph.microsoft.com/beta/me/contactFolders/{id}/contacts
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="b1dbf-135">C#</span><span class="sxs-lookup"><span data-stu-id="b1dbf-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/contactfolder-get-contacts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b1dbf-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="b1dbf-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/contactfolder-get-contacts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="b1dbf-137">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="b1dbf-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/contactfolder-get-contacts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="b1dbf-138">Java</span><span class="sxs-lookup"><span data-stu-id="b1dbf-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/contactfolder-get-contacts-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="b1dbf-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="b1dbf-139">Response</span></span>
<span data-ttu-id="b1dbf-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b1dbf-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
