---
title: Excluir contato
description: Exclua contato.
author: angelgolfer-ms
localization_priority: Normal
ms.openlocfilehash: 6e0fd4dcf7abc1b52b0a99d4220e313bef11a6b1
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27813374"
---
# <a name="delete-contact"></a><span data-ttu-id="7a395-103">Excluir contato</span><span class="sxs-lookup"><span data-stu-id="7a395-103">Delete contact</span></span>

> <span data-ttu-id="7a395-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="7a395-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7a395-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="7a395-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="7a395-106">Exclua contato.</span><span class="sxs-lookup"><span data-stu-id="7a395-106">Delete contact.</span></span>
## <a name="permissions"></a><span data-ttu-id="7a395-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="7a395-107">Permissions</span></span>
<span data-ttu-id="7a395-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7a395-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7a395-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7a395-110">Permission type</span></span>      | <span data-ttu-id="7a395-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7a395-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7a395-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7a395-112">Delegated (work or school account)</span></span> | <span data-ttu-id="7a395-113">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7a395-113">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="7a395-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7a395-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7a395-115">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7a395-115">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="7a395-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7a395-116">Application</span></span> | <span data-ttu-id="7a395-117">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7a395-117">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="7a395-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7a395-118">HTTP request</span></span>
<span data-ttu-id="7a395-119"><!-- { "blockType": "ignored" } -->Um [contato](../resources/contact.md) de de padrão do usuário [contactFolder](../resources/contactfolder.md).</span><span class="sxs-lookup"><span data-stu-id="7a395-119"><!-- { "blockType": "ignored" } --> A [contact](../resources/contact.md) from user's default [contactFolder](../resources/contactfolder.md).</span></span>
```http
DELETE /me/contacts/{id}
DELETE /users/{id | userPrincipalName}/contacts/{id}
```
<span data-ttu-id="7a395-120">Um [contact](../resources/contact.md) da [contactFolder](../resources/contactfolder.md) de nível superior do usuário.</span><span class="sxs-lookup"><span data-stu-id="7a395-120">A [contact](../resources/contact.md) from a user's top level [contactFolder](../resources/contactfolder.md).</span></span>
```http
DELETE /me/contactFolders/{id}/contacts/{id}
DELETE /users/{id | userPrincipalName}/contactFolders/{id}/contacts/{id}
```
<span data-ttu-id="7a395-121">Um [contato](../resources/contact.md) contidos em uma pasta filho de um [contactFolder](../resources/mailfolder.md).</span><span class="sxs-lookup"><span data-stu-id="7a395-121">A [contact](../resources/contact.md) contained in a child folder of a [contactFolder](../resources/mailfolder.md).</span></span>  <span data-ttu-id="7a395-122">O exemplo a seguir mostra um nível de aninhamento, mas um contato pode estar localizado no filho de um filho e assim por diante.</span><span class="sxs-lookup"><span data-stu-id="7a395-122">The example below shows one level of nesting, but a contact can be located in a child of a child and so on.</span></span>
```http
DELETE /me/contactFolder/{id}/childFolders/{id}/.../contacts/{id}
DELETE /users/{id | userPrincipalName}/contactFolders/{id}/childFolders/{id}/contacts/{id}
```
## <a name="request-headers"></a><span data-ttu-id="7a395-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7a395-123">Request headers</span></span>
| <span data-ttu-id="7a395-124">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="7a395-124">Header</span></span>       | <span data-ttu-id="7a395-125">Valor</span><span class="sxs-lookup"><span data-stu-id="7a395-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="7a395-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="7a395-126">Authorization</span></span>  | <span data-ttu-id="7a395-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7a395-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="7a395-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7a395-129">Request body</span></span>
<span data-ttu-id="7a395-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7a395-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7a395-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="7a395-131">Response</span></span>

<span data-ttu-id="7a395-p105">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7a395-p105">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7a395-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7a395-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7a395-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7a395-135">Request</span></span>
<span data-ttu-id="7a395-136">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7a395-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_contact"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/contacts/{id}
```
##### <a name="response"></a><span data-ttu-id="7a395-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="7a395-137">Response</span></span>
<span data-ttu-id="7a395-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7a395-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
