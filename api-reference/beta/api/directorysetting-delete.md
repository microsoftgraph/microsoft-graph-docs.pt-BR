---
title: Excluir uma configuração de diretório
description: Exclua uma configuração de diretório.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: c66335ec863460c9b2167e25a7e78850846e105c
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29515822"
---
# <a name="delete-a-directory-setting"></a><span data-ttu-id="7312f-103">Excluir uma configuração de diretório</span><span class="sxs-lookup"><span data-stu-id="7312f-103">Delete a directory setting</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7312f-104">Exclua uma configuração de diretório.</span><span class="sxs-lookup"><span data-stu-id="7312f-104">Delete a directory setting.</span></span>

> <span data-ttu-id="7312f-105">**Observação**: A versão de /beta desse API é só se aplica aos grupos.</span><span class="sxs-lookup"><span data-stu-id="7312f-105">**Note**: The /beta version of this API is only applies to groups.</span></span> <span data-ttu-id="7312f-106">A versão de /v1.0 desse API foi renomeada para *Excluir groupSettings*.</span><span class="sxs-lookup"><span data-stu-id="7312f-106">The /v1.0 version of this API has been renamed to *Delete groupSettings*.</span></span>

## <a name="permissions"></a><span data-ttu-id="7312f-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="7312f-107">Permissions</span></span>
<span data-ttu-id="7312f-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7312f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7312f-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7312f-110">Permission type</span></span>      | <span data-ttu-id="7312f-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7312f-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7312f-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7312f-112">Delegated (work or school account)</span></span> | <span data-ttu-id="7312f-113">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="7312f-113">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="7312f-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7312f-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7312f-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7312f-115">Not supported.</span></span>    |
|<span data-ttu-id="7312f-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7312f-116">Application</span></span> | <span data-ttu-id="7312f-117">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7312f-117">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7312f-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7312f-118">HTTP request</span></span>
<span data-ttu-id="7312f-119"><!-- { "blockType": "ignored" } -->Excluir um locatário todo específico ou configuração de grupo</span><span class="sxs-lookup"><span data-stu-id="7312f-119"><!-- { "blockType": "ignored" } --> Delete a specific tenant-wide or group setting</span></span>
```http
DELETE /settings/{id}
DELETE /groups/{id}/settings/{id}

```
## <a name="request-headers"></a><span data-ttu-id="7312f-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7312f-120">Request headers</span></span>
| <span data-ttu-id="7312f-121">Nome</span><span class="sxs-lookup"><span data-stu-id="7312f-121">Name</span></span>       | <span data-ttu-id="7312f-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="7312f-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="7312f-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="7312f-123">Authorization</span></span>  | <span data-ttu-id="7312f-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7312f-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7312f-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7312f-126">Request body</span></span>
<span data-ttu-id="7312f-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7312f-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7312f-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="7312f-128">Response</span></span>

<span data-ttu-id="7312f-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7312f-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7312f-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7312f-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7312f-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7312f-132">Request</span></span>
<span data-ttu-id="7312f-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7312f-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_directorysetting"
}-->
```http
DELETE https://graph.microsoft.com/beta/settings/{id}
```
##### <a name="response"></a><span data-ttu-id="7312f-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="7312f-134">Response</span></span>
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
  "description": "Delete directorySetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/directorysetting-delete.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
