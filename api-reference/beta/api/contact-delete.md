---
title: Excluir contato
description: Excluir contato
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: be83bb8f655190d2da6aace13def579e371ef024
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29514765"
---
# <a name="delete-contact"></a><span data-ttu-id="474ef-103">Excluir contato</span><span class="sxs-lookup"><span data-stu-id="474ef-103">Delete contact</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="474ef-104">Excluir contato</span><span class="sxs-lookup"><span data-stu-id="474ef-104">Delete contact.</span></span>
## <a name="permissions"></a><span data-ttu-id="474ef-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="474ef-105">Permissions</span></span>
<span data-ttu-id="474ef-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="474ef-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="474ef-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="474ef-108">Permission type</span></span>      | <span data-ttu-id="474ef-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="474ef-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="474ef-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="474ef-110">Delegated (work or school account)</span></span> | <span data-ttu-id="474ef-111">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="474ef-111">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="474ef-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="474ef-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="474ef-113">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="474ef-113">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="474ef-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="474ef-114">Application</span></span> | <span data-ttu-id="474ef-115">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="474ef-115">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="474ef-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="474ef-116">HTTP request</span></span>
<span data-ttu-id="474ef-117"><!-- { "blockType": "ignored" } -->Um [contato](../resources/contact.md) de de padrão do usuário [contactFolder](../resources/contactfolder.md).</span><span class="sxs-lookup"><span data-stu-id="474ef-117"><!-- { "blockType": "ignored" } --> A [contact](../resources/contact.md) from user's default [contactFolder](../resources/contactfolder.md).</span></span>
```http
DELETE /me/contacts/{id}
DELETE /users/{id | userPrincipalName}/contacts/{id}
```
<span data-ttu-id="474ef-118">Um [contact](../resources/contact.md) da [contactFolder](../resources/contactfolder.md) de nível superior do usuário.</span><span class="sxs-lookup"><span data-stu-id="474ef-118">A [contact](../resources/contact.md) from a user's top level [contactFolder](../resources/contactfolder.md).</span></span>
```http
DELETE /me/contactFolders/{id}/contacts/{id}
DELETE /users/{id | userPrincipalName}/contactFolders/{id}/contacts/{id}
```
<span data-ttu-id="474ef-119">Um [contato](../resources/contact.md) contidos em uma pasta filho de um [contactFolder](../resources/mailfolder.md).</span><span class="sxs-lookup"><span data-stu-id="474ef-119">A [contact](../resources/contact.md) contained in a child folder of a [contactFolder](../resources/mailfolder.md).</span></span>  <span data-ttu-id="474ef-120">O exemplo a seguir mostra um nível de aninhamento, mas um contato pode estar localizado no filho de um filho e assim por diante.</span><span class="sxs-lookup"><span data-stu-id="474ef-120">The example below shows one level of nesting, but a contact can be located in a child of a child and so on.</span></span>
```http
DELETE /me/contactFolder/{id}/childFolders/{id}/.../contacts/{id}
DELETE /users/{id | userPrincipalName}/contactFolders/{id}/childFolders/{id}/contacts/{id}
```
## <a name="request-headers"></a><span data-ttu-id="474ef-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="474ef-121">Request headers</span></span>
| <span data-ttu-id="474ef-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="474ef-122">Header</span></span>       | <span data-ttu-id="474ef-123">Valor</span><span class="sxs-lookup"><span data-stu-id="474ef-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="474ef-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="474ef-124">Authorization</span></span>  | <span data-ttu-id="474ef-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="474ef-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="474ef-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="474ef-127">Request body</span></span>
<span data-ttu-id="474ef-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="474ef-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="474ef-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="474ef-129">Response</span></span>

<span data-ttu-id="474ef-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="474ef-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="474ef-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="474ef-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="474ef-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="474ef-133">Request</span></span>
<span data-ttu-id="474ef-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="474ef-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_contact"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/contacts/{id}
```
##### <a name="response"></a><span data-ttu-id="474ef-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="474ef-135">Response</span></span>
<span data-ttu-id="474ef-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="474ef-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete contact",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/contact-delete.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
