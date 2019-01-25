---
title: Excluir educationClass
description: Exclua uma aula. Como uma aula também é um grupo universal, excluir uma aula exclui o grupo.
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: a7d5f376bd6d70229d8058084946fd474a692212
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29508157"
---
# <a name="delete-educationclass"></a><span data-ttu-id="a59cc-104">Excluir educationClass</span><span class="sxs-lookup"><span data-stu-id="a59cc-104">Delete educationClass</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a59cc-105">Exclua uma aula.</span><span class="sxs-lookup"><span data-stu-id="a59cc-105">Delete a class.</span></span> <span data-ttu-id="a59cc-106">Como uma aula também é um grupo universal, excluir uma aula exclui o grupo.</span><span class="sxs-lookup"><span data-stu-id="a59cc-106">Because a class is also a universal group, deleting a class deletes the group.</span></span>

## <a name="permissions"></a><span data-ttu-id="a59cc-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="a59cc-107">Permissions</span></span>
<span data-ttu-id="a59cc-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a59cc-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a59cc-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a59cc-110">Permission type</span></span>      | <span data-ttu-id="a59cc-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a59cc-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a59cc-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a59cc-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="a59cc-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a59cc-113">Not supported.</span></span>  |
|<span data-ttu-id="a59cc-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a59cc-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="a59cc-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a59cc-115">Not supported.</span></span>  |
|<span data-ttu-id="a59cc-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a59cc-116">Application</span></span> | <span data-ttu-id="a59cc-117">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a59cc-117">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="a59cc-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a59cc-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /education/classes/{id}

```
## <a name="request-headers"></a><span data-ttu-id="a59cc-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a59cc-119">Request headers</span></span>
| <span data-ttu-id="a59cc-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a59cc-120">Header</span></span>       | <span data-ttu-id="a59cc-121">Valor</span><span class="sxs-lookup"><span data-stu-id="a59cc-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="a59cc-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="a59cc-122">Authorization</span></span>  | <span data-ttu-id="a59cc-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a59cc-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a59cc-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a59cc-125">Request body</span></span>
<span data-ttu-id="a59cc-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a59cc-126">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="a59cc-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="a59cc-127">Response</span></span>
<span data-ttu-id="a59cc-p105">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a59cc-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a59cc-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a59cc-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a59cc-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a59cc-131">Request</span></span>
<span data-ttu-id="a59cc-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="a59cc-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_educationclass"
}-->
```http
DELETE https://graph.microsoft.com/beta/education/classes/11022
```
##### <a name="response"></a><span data-ttu-id="a59cc-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="a59cc-133">Response</span></span>
<span data-ttu-id="a59cc-134">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="a59cc-134">The following is an example of the response.</span></span> 

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
  "description": "Delete educationClass",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/educationclass-delete.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
