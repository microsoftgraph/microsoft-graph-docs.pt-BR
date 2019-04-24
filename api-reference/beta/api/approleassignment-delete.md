---
title: Excluir appRoleAssignment
description: Exclua appRoleAssignment.
localization_priority: Normal
ms.openlocfilehash: 1c9855e05de9aa1773bb9de5f1c5e7f17c51df9a
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32458961"
---
# <a name="delete-approleassignment"></a><span data-ttu-id="8372c-103">Excluir appRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="8372c-103">Delete appRoleAssignment</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8372c-104">Exclua appRoleAssignment.</span><span class="sxs-lookup"><span data-stu-id="8372c-104">Delete appRoleAssignment.</span></span>
## <a name="permissions"></a><span data-ttu-id="8372c-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="8372c-105">Permissions</span></span>
<span data-ttu-id="8372c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8372c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8372c-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8372c-108">Permission type</span></span>      | <span data-ttu-id="8372c-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8372c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8372c-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8372c-110">Delegated (work or school account)</span></span> | <span data-ttu-id="8372c-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="8372c-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="8372c-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8372c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8372c-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8372c-113">Not supported.</span></span>    |
|<span data-ttu-id="8372c-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8372c-114">Application</span></span> | <span data-ttu-id="8372c-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8372c-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8372c-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8372c-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /users/{id | userPrincipalName}/appRoleAssignments/{id}
DELETE /servicePrincipals/{id}/appRoleAssignedTo
DELETE /groups/{id}/appRoleAssignments/{id}

```
## <a name="request-headers"></a><span data-ttu-id="8372c-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8372c-117">Request headers</span></span>
| <span data-ttu-id="8372c-118">Nome</span><span class="sxs-lookup"><span data-stu-id="8372c-118">Name</span></span>       | <span data-ttu-id="8372c-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="8372c-119">Type</span></span> | <span data-ttu-id="8372c-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="8372c-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="8372c-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="8372c-121">Authorization</span></span>  | <span data-ttu-id="8372c-122">string</span><span class="sxs-lookup"><span data-stu-id="8372c-122">string</span></span>  | <span data-ttu-id="8372c-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8372c-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8372c-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8372c-125">Request body</span></span>
<span data-ttu-id="8372c-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="8372c-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8372c-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="8372c-127">Response</span></span>

<span data-ttu-id="8372c-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8372c-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8372c-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8372c-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8372c-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8372c-131">Request</span></span>
<span data-ttu-id="8372c-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8372c-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_approleassignment"
}-->
```http
DELETE https://graph.microsoft.com/beta/appRoleAssignments/{id}
```
##### <a name="response"></a><span data-ttu-id="8372c-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="8372c-133">Response</span></span>
<span data-ttu-id="8372c-134">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8372c-134">Here is an example of the response.</span></span> 
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
  "description": "Delete appRoleAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/approleassignment-delete.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
