---
title: Excluir contato
description: Exclui um contato.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 43e7518958a2352fa44b988d96a37e781ad88f75
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27967193"
---
# <a name="delete-contact"></a><span data-ttu-id="72141-103">Excluir contato</span><span class="sxs-lookup"><span data-stu-id="72141-103">Delete contact</span></span>

<span data-ttu-id="72141-104">Exclui um contato.</span><span class="sxs-lookup"><span data-stu-id="72141-104">Delete a contact.</span></span>
## <a name="permissions"></a><span data-ttu-id="72141-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="72141-105">Permissions</span></span>
<span data-ttu-id="72141-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="72141-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="72141-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="72141-108">Permission type</span></span>      | <span data-ttu-id="72141-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="72141-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="72141-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="72141-110">Delegated (work or school account)</span></span> | <span data-ttu-id="72141-111">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="72141-111">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="72141-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="72141-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="72141-113">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="72141-113">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="72141-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="72141-114">Application</span></span> | <span data-ttu-id="72141-115">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="72141-115">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="72141-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="72141-116">HTTP request</span></span>
<span data-ttu-id="72141-117"><!-- { "blockType": "ignored" } -->Um [contato](../resources/contact.md) do padrão de um usuário [contactFolder](../resources/contactfolder.md).</span><span class="sxs-lookup"><span data-stu-id="72141-117"><!-- { "blockType": "ignored" } --> A [contact](../resources/contact.md) from a user's default [contactFolder](../resources/contactfolder.md).</span></span>
```http
DELETE /me/contacts/{id}
DELETE /users/{id | userPrincipalName}/contacts/{id}
```
<span data-ttu-id="72141-118">Um [contact](../resources/contact.md) da [contactFolder](../resources/contactfolder.md) de nível superior do usuário.</span><span class="sxs-lookup"><span data-stu-id="72141-118">A [contact](../resources/contact.md) from a user's top level [contactFolder](../resources/contactfolder.md).</span></span>
```http
DELETE /me/contactFolders/{id}/contacts/{id}
DELETE /users/{id | userPrincipalName}/contactFolders/{id}/contacts/{id}
```
<span data-ttu-id="72141-p102">Um [contact](../resources/contact.md) incluso em uma pasta filha de uma [contactFolder](../resources/mailfolder.md). O exemplo a seguir mostra um nível de aninhamento, mas um contato pode estar localizado em um filho de um filho, e assim por diante.</span><span class="sxs-lookup"><span data-stu-id="72141-p102">A [contact](../resources/contact.md) contained in a child folder of a [contactFolder](../resources/mailfolder.md). The example below shows one level of nesting, but a contact can be located in a child of a child and so on.</span></span>
```http
DELETE /me/contactFolder/{id}/childFolders/{id}/.../contacts/{id}
DELETE /users/{id | userPrincipalName}/contactFolders/{id}/childFolders/{id}/contacts/{id}
```
## <a name="request-headers"></a><span data-ttu-id="72141-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="72141-121">Request headers</span></span>
| <span data-ttu-id="72141-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="72141-122">Header</span></span>       | <span data-ttu-id="72141-123">Valor</span><span class="sxs-lookup"><span data-stu-id="72141-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="72141-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="72141-124">Authorization</span></span>  | <span data-ttu-id="72141-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="72141-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="72141-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="72141-127">Request body</span></span>
<span data-ttu-id="72141-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="72141-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="72141-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="72141-129">Response</span></span>

<span data-ttu-id="72141-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="72141-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="72141-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="72141-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="72141-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="72141-133">Request</span></span>
<span data-ttu-id="72141-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="72141-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_contact"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/contacts/{id}
```
##### <a name="response"></a><span data-ttu-id="72141-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="72141-135">Response</span></span>
<span data-ttu-id="72141-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="72141-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete contact",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
