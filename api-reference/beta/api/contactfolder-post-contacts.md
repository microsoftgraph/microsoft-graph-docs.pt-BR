---
title: Criar contato
description: Adicione um contato na pasta de contatos raiz ou no ponto de extremidade de `contacts` de outra pasta de contatos.
author: angelgolfer-ms
ms.openlocfilehash: eb80ec34a5c4bb58aa1c401a19e1ab5632f089f8
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27350877"
---
# <a name="create-contact"></a><span data-ttu-id="a0dee-103">Criar contato</span><span class="sxs-lookup"><span data-stu-id="a0dee-103">Create Contact</span></span>

> <span data-ttu-id="a0dee-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="a0dee-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a0dee-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="a0dee-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a0dee-106">Adicione um contato na pasta de contatos raiz ou no ponto de extremidade de `contacts` de outra pasta de contatos.</span><span class="sxs-lookup"><span data-stu-id="a0dee-106">Add a contact to the root Contacts folder or to the `contacts` endpoint of another contact folder.</span></span>
## <a name="permissions"></a><span data-ttu-id="a0dee-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="a0dee-107">Permissions</span></span>
<span data-ttu-id="a0dee-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a0dee-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a0dee-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a0dee-110">Permission type</span></span>      | <span data-ttu-id="a0dee-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a0dee-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a0dee-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a0dee-112">Delegated (work or school account)</span></span> | <span data-ttu-id="a0dee-113">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a0dee-113">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="a0dee-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a0dee-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a0dee-115">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a0dee-115">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="a0dee-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a0dee-116">Application</span></span> | <span data-ttu-id="a0dee-117">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a0dee-117">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="a0dee-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a0dee-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/contacts
POST /users/{id | userPrincipalName}/contacts

POST /me/contactFolders/{id}/contacts
POST /users/{id | userPrincipalName}/contactFolders/{id}/contacts
```
## <a name="request-headers"></a><span data-ttu-id="a0dee-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a0dee-119">Request headers</span></span>
## <a name="request-headers"></a><span data-ttu-id="a0dee-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a0dee-120">Request headers</span></span>
| <span data-ttu-id="a0dee-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a0dee-121">Header</span></span>       | <span data-ttu-id="a0dee-122">Valor</span><span class="sxs-lookup"><span data-stu-id="a0dee-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="a0dee-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="a0dee-123">Authorization</span></span>  | <span data-ttu-id="a0dee-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a0dee-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="a0dee-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a0dee-126">Content-Type</span></span>  | <span data-ttu-id="a0dee-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a0dee-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a0dee-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a0dee-129">Request body</span></span>
<span data-ttu-id="a0dee-130">No corpo da solicitação, forneça uma representação JSON do objeto [Contact](../resources/contact.md).</span><span class="sxs-lookup"><span data-stu-id="a0dee-130">In the request body, supply a JSON representation of [Contact](../resources/contact.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="a0dee-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="a0dee-131">Response</span></span>

<span data-ttu-id="a0dee-132">Se bem-sucedido, este método retorna um código de resposta `201 Created` e um objeto [Contact](../resources/contact.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a0dee-132">If successful, this method returns `201 Created` response code and [Contact](../resources/contact.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a0dee-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a0dee-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a0dee-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a0dee-134">Request</span></span>
<span data-ttu-id="a0dee-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a0dee-135">Here is an example of the request.</span></span>
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
<span data-ttu-id="a0dee-136">No corpo da solicitação, forneça uma representação JSON do objeto [contact](../resources/contact.md).</span><span class="sxs-lookup"><span data-stu-id="a0dee-136">In the request body, supply a JSON representation of [contact](../resources/contact.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="a0dee-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="a0dee-137">Response</span></span>
<span data-ttu-id="a0dee-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a0dee-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Create Contact",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->