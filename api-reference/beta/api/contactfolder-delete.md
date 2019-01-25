---
title: Excluir contactFolder
description: Exclui uma contactFolder que não a padrão.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 01b8303723c4a59b8fdc4ac3f5d7d4f6cb491fd1
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29523915"
---
# <a name="delete-contactfolder"></a><span data-ttu-id="52404-103">Excluir contactFolder</span><span class="sxs-lookup"><span data-stu-id="52404-103">Delete contactFolder</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="52404-104">Exclui uma contactFolder que não a padrão.</span><span class="sxs-lookup"><span data-stu-id="52404-104">Delete contactFolder other than the default contactFolder.</span></span>
## <a name="permissions"></a><span data-ttu-id="52404-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="52404-105">Permissions</span></span>
<span data-ttu-id="52404-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="52404-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="52404-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="52404-108">Permission type</span></span>      | <span data-ttu-id="52404-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="52404-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="52404-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="52404-110">Delegated (work or school account)</span></span> | <span data-ttu-id="52404-111">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="52404-111">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="52404-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="52404-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="52404-113">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="52404-113">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="52404-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="52404-114">Application</span></span> | <span data-ttu-id="52404-115">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="52404-115">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="52404-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="52404-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/contactFolders/{id}
DELETE /users/{id | userPrincipalName}/contactFolders/{id}
```
## <a name="request-headers"></a><span data-ttu-id="52404-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="52404-117">Request headers</span></span>
| <span data-ttu-id="52404-118">Nome</span><span class="sxs-lookup"><span data-stu-id="52404-118">Name</span></span>       | <span data-ttu-id="52404-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="52404-119">Type</span></span> | <span data-ttu-id="52404-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="52404-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="52404-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="52404-121">Authorization</span></span>  | <span data-ttu-id="52404-122">string</span><span class="sxs-lookup"><span data-stu-id="52404-122">string</span></span>  | <span data-ttu-id="52404-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="52404-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="52404-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="52404-125">Request body</span></span>
<span data-ttu-id="52404-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="52404-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="52404-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="52404-127">Response</span></span>

<span data-ttu-id="52404-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="52404-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="52404-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="52404-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="52404-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="52404-131">Request</span></span>
<span data-ttu-id="52404-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="52404-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_contactfolder"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/contactFolders/{id}
```
##### <a name="response"></a><span data-ttu-id="52404-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="52404-133">Response</span></span>
<span data-ttu-id="52404-134">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="52404-134">Here is an example of the response.</span></span> 
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
  "description": "Delete contactFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/contactfolder-delete.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
