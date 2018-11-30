---
title: Criar contato
description: Adicione um contato na pasta de contatos raiz ou no ponto de extremidade do `contacts` de outra pasta de contatos.
ms.openlocfilehash: d17072285b52a70a8d30533c073678d9bf2ec95d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27004297"
---
# <a name="create-contact"></a><span data-ttu-id="12e52-103">Criar contato</span><span class="sxs-lookup"><span data-stu-id="12e52-103">Create contact</span></span>

<span data-ttu-id="12e52-104">Adicione um contato na pasta de contatos raiz ou no ponto de extremidade do `contacts` de outra pasta de contatos.</span><span class="sxs-lookup"><span data-stu-id="12e52-104">Add a contact to the root Contacts folder or to the `contacts` endpoint of another contact folder.</span></span>

## <a name="permissions"></a><span data-ttu-id="12e52-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="12e52-105">Permissions</span></span>

<span data-ttu-id="12e52-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="12e52-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="12e52-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="12e52-108">Permission type</span></span>      | <span data-ttu-id="12e52-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="12e52-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="12e52-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="12e52-110">Delegated (work or school account)</span></span> | <span data-ttu-id="12e52-111">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="12e52-111">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="12e52-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="12e52-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="12e52-113">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="12e52-113">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="12e52-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="12e52-114">Application</span></span> | <span data-ttu-id="12e52-115">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="12e52-115">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="12e52-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="12e52-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/contacts
POST /users/{id | userPrincipalName}/contacts

POST /me/contactFolders/{id}/contacts
POST /users/{id | userPrincipalName}/contactFolders/{id}/contacts
```

<br/>

## <a name="request-headers"></a><span data-ttu-id="12e52-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="12e52-117">Request headers</span></span>

| <span data-ttu-id="12e52-118">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="12e52-118">Header</span></span>       | <span data-ttu-id="12e52-119">Valor</span><span class="sxs-lookup"><span data-stu-id="12e52-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="12e52-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="12e52-120">Authorization</span></span>  | <span data-ttu-id="12e52-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="12e52-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="12e52-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="12e52-123">Content-Type</span></span>  | <span data-ttu-id="12e52-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="12e52-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="12e52-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="12e52-126">Request body</span></span>
<span data-ttu-id="12e52-127">No corpo da solicitação, forneça uma representação JSON do objeto [Contact](../resources/contact.md).</span><span class="sxs-lookup"><span data-stu-id="12e52-127">In the request body, supply a JSON representation of the [Contact](../resources/contact.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="12e52-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="12e52-128">Response</span></span>

<span data-ttu-id="12e52-129">Se bem-sucedido, este método retorna um código de resposta `201 Created` e um objeto [Contact](../resources/contact.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="12e52-129">If successful, this method returns `201 Created` response code and the [Contact](../resources/contact.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="12e52-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="12e52-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="12e52-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="12e52-131">Request</span></span>

<span data-ttu-id="12e52-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="12e52-132">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "create_contact_from_contactfolder"
}-->

```http
POST https://graph.microsoft.com/v1.0/me/contactFolders/{id}/contacts
Content-type: application/json
Content-length: 210

{
  "parentFolderId": "parentFolderId-value",
  "birthday": "datetime-value",
  "fileAs": "fileAs-value",
  "displayName": "displayName-value",
  "givenName": "givenName-value",
  "initials": "initials-value"
}
```

<br/>

<span data-ttu-id="12e52-133">No corpo da solicitação, forneça uma representação JSON do objeto [Contact](../resources/contact.md).</span><span class="sxs-lookup"><span data-stu-id="12e52-133">In the request body, supply a JSON representation of the [Contact](../resources/contact.md) object.</span></span>

### <a name="response"></a><span data-ttu-id="12e52-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="12e52-134">Response</span></span>

<span data-ttu-id="12e52-135">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="12e52-135">Here is an example of the response.</span></span> <span data-ttu-id="12e52-136">**Observação:** O objeto da resposta mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="12e52-136">**Note:** The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="12e52-137">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="12e52-137">All the properties will be returned from an actual call.</span></span>

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
  "birthday": "datetime-value",
  "fileAs": "fileAs-value",
  "displayName": "displayName-value",
  "givenName": "givenName-value",
  "initials": "initials-value"
}
```

<br/>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create Contact",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
