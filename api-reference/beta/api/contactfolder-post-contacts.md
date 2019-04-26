---
title: Criar contato
description: Adicione um contato na pasta de contatos raiz ou no ponto de extremidade do `contacts` de outra pasta de contatos.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 6e00631e03579455207d962a7fe2857756257386
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33327181"
---
# <a name="create-contact"></a><span data-ttu-id="59cd5-103">Criar contato</span><span class="sxs-lookup"><span data-stu-id="59cd5-103">Create Contact</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="59cd5-104">Adicione um contato na pasta de contatos raiz ou no ponto de extremidade do `contacts` de outra pasta de contatos.</span><span class="sxs-lookup"><span data-stu-id="59cd5-104">Add a contact to the root Contacts folder or to the `contacts` endpoint of another contact folder.</span></span>
## <a name="permissions"></a><span data-ttu-id="59cd5-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="59cd5-105">Permissions</span></span>
<span data-ttu-id="59cd5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="59cd5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="59cd5-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="59cd5-108">Permission type</span></span>      | <span data-ttu-id="59cd5-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="59cd5-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="59cd5-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="59cd5-110">Delegated (work or school account)</span></span> | <span data-ttu-id="59cd5-111">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="59cd5-111">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="59cd5-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="59cd5-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="59cd5-113">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="59cd5-113">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="59cd5-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="59cd5-114">Application</span></span> | <span data-ttu-id="59cd5-115">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="59cd5-115">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="59cd5-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="59cd5-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/contacts
POST /users/{id | userPrincipalName}/contacts

POST /me/contactFolders/{id}/contacts
POST /users/{id | userPrincipalName}/contactFolders/{id}/contacts
```
## <a name="request-headers"></a><span data-ttu-id="59cd5-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="59cd5-117">Request headers</span></span>
## <a name="request-headers"></a><span data-ttu-id="59cd5-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="59cd5-118">Request headers</span></span>
| <span data-ttu-id="59cd5-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="59cd5-119">Header</span></span>       | <span data-ttu-id="59cd5-120">Valor</span><span class="sxs-lookup"><span data-stu-id="59cd5-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="59cd5-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="59cd5-121">Authorization</span></span>  | <span data-ttu-id="59cd5-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="59cd5-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="59cd5-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="59cd5-124">Content-Type</span></span>  | <span data-ttu-id="59cd5-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="59cd5-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="59cd5-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="59cd5-127">Request body</span></span>
<span data-ttu-id="59cd5-128">No corpo da solicitação, forneça uma representação JSON do objeto [Contact](../resources/contact.md).</span><span class="sxs-lookup"><span data-stu-id="59cd5-128">In the request body, supply a JSON representation of [Contact](../resources/contact.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="59cd5-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="59cd5-129">Response</span></span>

<span data-ttu-id="59cd5-130">Se bem-sucedido, este método retorna um código de resposta `201 Created` e um objeto [Contact](../resources/contact.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="59cd5-130">If successful, this method returns `201 Created` response code and [Contact](../resources/contact.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="59cd5-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="59cd5-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="59cd5-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="59cd5-132">Request</span></span>
<span data-ttu-id="59cd5-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="59cd5-133">Here is an example of the request.</span></span>
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
<span data-ttu-id="59cd5-134">No corpo da solicitação, forneça uma representação JSON do objeto [contact](../resources/contact.md).</span><span class="sxs-lookup"><span data-stu-id="59cd5-134">In the request body, supply a JSON representation of [contact](../resources/contact.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="59cd5-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="59cd5-135">Response</span></span>
<span data-ttu-id="59cd5-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="59cd5-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "suppressions": []
}
-->
