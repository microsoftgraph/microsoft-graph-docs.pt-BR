---
title: Criar contato
description: Adicione um contato na pasta de contatos raiz ou no ponto de extremidade do `contacts` de outra pasta de contatos.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 55d5e907125642c99074f42c4025e8b304f5ad08
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35437625"
---
# <a name="create-contact"></a><span data-ttu-id="33c88-103">Criar contato</span><span class="sxs-lookup"><span data-stu-id="33c88-103">Create Contact</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="33c88-104">Adicione um contato na pasta de contatos raiz ou no ponto de extremidade do `contacts` de outra pasta de contatos.</span><span class="sxs-lookup"><span data-stu-id="33c88-104">Add a contact to the root Contacts folder or to the `contacts` endpoint of another contact folder.</span></span>
## <a name="permissions"></a><span data-ttu-id="33c88-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="33c88-105">Permissions</span></span>
<span data-ttu-id="33c88-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="33c88-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="33c88-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="33c88-108">Permission type</span></span>      | <span data-ttu-id="33c88-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="33c88-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="33c88-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="33c88-110">Delegated (work or school account)</span></span> | <span data-ttu-id="33c88-111">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="33c88-111">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="33c88-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="33c88-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="33c88-113">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="33c88-113">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="33c88-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="33c88-114">Application</span></span> | <span data-ttu-id="33c88-115">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="33c88-115">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="33c88-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="33c88-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/contacts
POST /users/{id | userPrincipalName}/contacts

POST /me/contactFolders/{id}/contacts
POST /users/{id | userPrincipalName}/contactFolders/{id}/contacts
```
## <a name="request-headers"></a><span data-ttu-id="33c88-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="33c88-117">Request headers</span></span>
## <a name="request-headers"></a><span data-ttu-id="33c88-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="33c88-118">Request headers</span></span>
| <span data-ttu-id="33c88-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="33c88-119">Header</span></span>       | <span data-ttu-id="33c88-120">Valor</span><span class="sxs-lookup"><span data-stu-id="33c88-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="33c88-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="33c88-121">Authorization</span></span>  | <span data-ttu-id="33c88-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="33c88-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="33c88-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="33c88-124">Content-Type</span></span>  | <span data-ttu-id="33c88-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="33c88-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="33c88-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="33c88-127">Request body</span></span>
<span data-ttu-id="33c88-128">No corpo da solicitação, forneça uma representação JSON do objeto [Contact](../resources/contact.md).</span><span class="sxs-lookup"><span data-stu-id="33c88-128">In the request body, supply a JSON representation of [Contact](../resources/contact.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="33c88-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="33c88-129">Response</span></span>

<span data-ttu-id="33c88-130">Se bem-sucedido, este método retorna um código de resposta `201 Created` e um objeto [Contact](../resources/contact.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="33c88-130">If successful, this method returns `201 Created` response code and [Contact](../resources/contact.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="33c88-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="33c88-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="33c88-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="33c88-132">Request</span></span>
<span data-ttu-id="33c88-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="33c88-133">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="33c88-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="33c88-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_contact_from_contactfolder"
}-->
```http
POST https://graph.microsoft.com/beta/me/contactFolders/{id}/contacts
Content-type: application/json
Content-length: 210

{
  "parentFolderId": "parentFolderId-value",
  "birthday": "2016-10-19T10:37:00Z",
  "fileAs": "fileAs-value",
  "displayName": "displayName-value",
  "givenName": "givenName-value",
  "initials": "initials-value"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="33c88-135">C#</span><span class="sxs-lookup"><span data-stu-id="33c88-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-contact-from-contactfolder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="33c88-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="33c88-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-contact-from-contactfolder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="33c88-137">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="33c88-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-contact-from-contactfolder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="33c88-138">No corpo da solicitação, forneça uma representação JSON do objeto [contact](../resources/contact.md).</span><span class="sxs-lookup"><span data-stu-id="33c88-138">In the request body, supply a JSON representation of [contact](../resources/contact.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="33c88-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="33c88-139">Response</span></span>
<span data-ttu-id="33c88-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="33c88-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contact"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 210

{
  "parentFolderId": "parentFolderId-value",
  "birthday": "2016-10-19T10:37:00Z",
  "fileAs": "fileAs-value",
  "displayName": "displayName-value",
  "givenName": "givenName-value",
  "initials": "initials-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create Contact",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
